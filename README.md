# mtnonline clone

This is a clone of the [mtnonline supplier page](https://www.mtnonline.com/contact-us/supplier). This clone was built with VueJS, bootstrap and the giphy public API. The deployed version can be found [here](https://mtnonline.netlify.app/)

## 💿 Project setup
 - Clone the repository to your local maching using
  ```bash
  git clone https://github.com/Abdulqudus001/mtn-online
  ```
 - Install dependencies using npm
  ```bash
  npm install
  ```

  or yarn
  ```bash
  yarn install
  ```

  - Head over to [giphy](https://developers.giphy.com/) to create an account and generate an API key.
  - Create a .env file at the root folder and add `VUE_APP_TOKEN=your_giphy_token` to the file to be able to use the giphy API 
### 🚀 Compiles and hot-reloads for development
To start up the server after installing dependencies, run
``` bash
yarn serve
```

### ⚒️ Compiles and minifies for production
```
yarn build
```

### 🛠️ Lints and fixes files
```
yarn lint
```

### Customize configuration
See [Configuration Reference](https://cli.vuejs.org/config/).
