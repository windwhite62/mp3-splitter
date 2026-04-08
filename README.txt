Déploiement GitHub Pages - Découpeur MP3

1. Mets splitter.html à la racine de ton dossier publié.
2. Crée un dossier ffmpeg/ au même niveau.
3. Ajoute dans ffmpeg/ les fichiers suivants issus du package @ffmpeg/core et @ffmpeg/ffmpeg :
   - ffmpeg.esm.js
   - util.esm.js
   - ffmpeg-core.js
   - ffmpeg-core.wasm
   - ffmpeg-core.worker.js
4. Publie l'ensemble sur le même domaine GitHub Pages.
5. Ouvre splitter.html depuis ton site.

Arborescence attendue :

/ton-site/
  splitter.html
  /ffmpeg/
    ffmpeg.esm.js
    util.esm.js
    ffmpeg-core.js
    ffmpeg-core.wasm
    ffmpeg-core.worker.js

Important :
- Le HTML charge les fichiers localement via ./ffmpeg/...
- Cette approche évite l'erreur Worker cross-origin.
- Si besoin, adapte les noms exacts selon la version des fichiers téléchargés.
