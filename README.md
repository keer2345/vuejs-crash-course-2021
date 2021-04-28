# demo01

- [Vue JS Crash Course 2021](https://youtu.be/qZXt1Aom3Cs)

## Project setup
```
yarn install
```

### Compiles and hot-reloads for development
```
yarn serve
```

### Compiles and minifies for production
```
yarn build
```

### Run for production
```
sudo yarn global add serve
serve -s dist
```

### Run json-server for backend
```
npm i json-server
```

*package.json*:
```
  "scripts": {
    // ...
    "backend": "json-server --watch db.json --port 5000"
  },
```
```
yarn backend
```
### Vue Router 4
```
npm install vue-router@4
```

### Lints and fixes files
```
yarn lint
```

### Customize configuration
See [Configuration Reference](https://cli.vuejs.org/config/).
