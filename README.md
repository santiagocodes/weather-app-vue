<img height="90px" align="left" src="https://santiagocodes.github.io/santiagocodes/images/octocat-santiagocodes.png" alt="santiagocodes octocat" />  

# Weather Web App

## Project setup

```
npm install
```

### Compiles and hot-reloads for development

```
npm run serve
```

### Compiles and minifies for production

```
npm run build
```

### Lints and fixes files

```
npm run lint
```

### Customize configuration

See [Configuration Reference](https://cli.vuejs.org/config/).

## API Key

Create `.env` file. You can create environment specific files as well with `.env.development.local` available only for development environment and `.env.production.local` for production environment. Make sure all your `.env` files are on your `.gitignore` file before committing anything to your repository.

### Getting a Key

Go to [openweathermap.org](https://openweathermap.org/) and create an account. Once you have signed in, go to [home.openweathermap.org/api_keys](https://home.openweathermap.org/api_keys) and on the `API keys` tap you have the option to create a new key for your project. Copy the generated key and go back to your editor.

### Adding Key

On `.env` file...

```
VUE_APP_WEATHER_KEY=************
```

### Accessing Key

```
data() {
    return {
    <!--variable : globalObject.environmentVariable -->
        api_key  :  process.env.VUE_APP_WEATHER_KEY
    }
}
```
