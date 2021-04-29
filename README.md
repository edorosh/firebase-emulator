# firebase-emulator
Docker build process for containerized Google Firebase Emulator

`docker pull edorosh/firebase-emulator-import:latest`

See [emulator documentation](https://firebase.google.com/docs/emulator-suite/install_and_configure) and sample docker-compose.yml for image usage.
To change default behavior, create a `firebase.json` and mount into the volume @ `/app/firebase.json` as shown in the included compose file.
Firebase imports backup data from the volume @ `/app` automatically on the startup.

```
curl -sL https://firebase.tools | bash
firebase login
firebase login:ci

```