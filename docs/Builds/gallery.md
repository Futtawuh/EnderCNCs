# Builds from Other Users

**Have you built one? Want to add yours to the list?**

Post a picture or video in the Discord channel #serial-request or DM **Ravenkeeper** on Printables to get a serial!

<style>
.build-gallery {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(200px, 1fr));
  gap: 1rem;
  margin-top: 1rem;
}
.build-card {
  border: 1px solid #ccc;
  border-radius: 8px;
  padding: 0.5rem;
  text-align: center;
  background-color: var(--md-default-bg-color);
  box-shadow: 0 2px 5px rgba(0,0,0,0.1);
}
.build-card img {
  width: 100%;
  height: auto;
  border-radius: 4px;
  margin-bottom: 0.5rem;
}
.serial-badge {
  display: inline-block;
  background: var(--md-primary-fg-color);
  color: var(--md-primary-bg-color);
  font-size: 0.7rem;
  font-weight: 700;
  padding: 0.2rem 0.5rem;
  border-radius: 999px;
  margin-bottom: 0.3rem;
}
.picture-needed {
  opacity: 0.6;
  font-style: italic;
  font-size: 0.9rem;
  margin-top: 0.5rem;
}
.gallery-loading {
  grid-column: 1 / -1;
  text-align: center;
  padding: 2rem;
  opacity: 0.6;
  font-style: italic;
}
.gallery-error {
  grid-column: 1 / -1;
  text-align: center;
  padding: 2rem;
  color: #c00;
}
</style>

<div class="build-gallery" id="build-gallery">
  <div class="gallery-loading" id="gallery-loading">Loading builds...</div>
</div>

<script>
(function () {
  var gallery = document.getElementById('build-gallery');
  var loading = document.getElementById('gallery-loading');

  fetch('/EnderCNCs/serials.json')
    .then(function (r) {
      if (!r.ok) throw new Error('HTTP ' + r.status);
      return r.json();
    })
    .then(function (data) {
      if (loading) loading.remove();
      var builds = (data.issued || []).sort(function (a, b) {
        return a.serialNumber - b.serialNumber;
      });

      if (builds.length === 0) {
        var empty = document.createElement('div');
        empty.className = 'gallery-loading';
        empty.textContent = 'No builds found yet.';
        gallery.appendChild(empty);
        return;
      }

      builds.forEach(function (build) {
        var num = String(build.serialNumber).padStart(2, '0');
        var isPlaceholder = !build.imageUrl || build.imageUrl.indexOf('placeholder.com') !== -1;
        var img = isPlaceholder
          ? '<div class="picture-needed">Picture needed</div>'
          : '<a href="' + build.imageUrl + '" target="_blank" rel="noopener noreferrer">' +
            '<img src="' + build.imageUrl + '" alt="' + build.username + ' Build" loading="lazy">' +
            '</a>';
        var card = document.createElement('div');
        card.className = 'build-card';
        card.innerHTML =
          '<span class="serial-badge">E3CNC.' + num + '</span>' +
          '<h4>' + build.username + '</h4>' +
          img;
        gallery.appendChild(card);
      });
    })
    .catch(function (err) {
      if (loading) loading.remove();
      var errDiv = document.createElement('div');
      errDiv.className = 'gallery-error';
      errDiv.textContent = 'Could not load builds. Please try again later.';
      gallery.appendChild(errDiv);
    });
})();
</script>
