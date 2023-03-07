# :wave: Say hi to Galactic :wave:

<!-- ## How to use

To use this repository for making Shopify themes, use the following command of Shopify CLI.
```sh
shopify theme init [ NAME OF YOUR THEME ] --clone-url https://github.com/polidario/Elizabeth_Clean
```

If you don't have Shopify CLI installed to your computer, navigate to the [installation page of Shopify CLI](https://shopify.dev/themes/tools/cli/installation).
 -->


# To use tailwind

## First initialize npm
`npm init -y`
## Install tailwindcss, postcss, autoprefixer
`npm install -D tailwindcss postcss autoprefixer`
## Then initialize tailwindcss to create tailwind.config.js
## Also create postcss.config.js file, add tailwindcss and autoprefixer plugin
`module.exports = {
    plugins: {
        tailwindcss: {},
        autoprefixer: {}
    }
}`
## Then create src folder and add tailwind.css file in it. Then create application.css file into assets folder using the following command.
`npx tailwindcss -i ./src/tailwind.css -o ./assets/application.css`


