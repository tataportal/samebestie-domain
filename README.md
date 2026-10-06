# Same Bestie domain deployment

Publishes https://samebestie.app independently of https://tataportal.github.io/samebestie/.

The app source lives in [tataportal/samebestie](https://github.com/tataportal/samebestie). This repository only contains deployment configuration. The workflow builds that repository's main branch and checks for updates every 15 minutes. It can also be run manually from Actions.

Keep the custom domain configured only on this repository so the original GitHub Pages address remains usable without a redirect.
