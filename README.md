# Quasar App (quasar-example-app)

A Quasar Framework app

## Install the dependencies
```bash
yarn
```

### Start the app in development mode (hot-code reloading, error reporting, etc.)
```bash
quasar dev
```

### Lint the files
```bash
yarn run lint
```

### Build the app for production
```bash
quasar build -m pwa
```

### Customize the configuration
See [Configuring quasar.conf.js](https://quasar.dev/quasar-cli/quasar-conf-js).

## Create Docker image and upload to Docker Hub

```bash
docker build -t drighart/workbench-quasar-theia:latest .
docker push drighart/workbench-quasar-theia:latest
docker run -ti -p 3000:3000 -p 8080:8080 drighart/workbench-quasar-theia:latest
```
