# Same Bestie domain deployment

Publishes https://samebestie.app independently of https://tataportal.github.io/samebestie/.

The app source lives in [tataportal/samebestie](https://github.com/tataportal/samebestie). This repository only contains deployment configuration. The workflow builds that repository's main branch and checks for updates every 15 minutes. It can also be run manually from Actions.

Keep the custom domain configured only on this repository so the original GitHub Pages address remains usable without a redirect.

The custom publication uses `www.samebestie.app` as its canonical address, with the apex domain redirected by GitHub Pages. Both names are included in the certificate request. The scheduled workflow enables HTTPS enforcement automatically after GitHub approves the certificate, even when the app source has not changed.
