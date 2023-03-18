# :wave: Say hi to Galactic :wave:


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
## Also we need to create tailwind.config.js file. For that we use the following command.
`npx tailwindcss init`

## In order to use tailwind classes we need to set configure tailwind.config.js file. So here we populate content array according to our need: 
`content: [`

`"./config/*.json",`

 `"./layout/*.liquid",`

`"./assets/*.liquid",`

`"./sections/*.liquid",`

`"./snippets/*.liquid",`

`"./templates/*.liquid",`

`"./templates/*.json",`

`"./templates/customers/*.liquid",`

`]`


## Then create src folder and add tailwind.css file in it. Then create application.css file into assets folder using the following command.
`npx tailwindcss -i ./src/tailwind.css -o ./assets/application.css`

## We can do the above thing using webpack mix. First install webpack mix
`npx install laravel-mix --save-dev`

## Then create a webpack.mix.js file and add configuration
`let mix = require('laravel-mix');`
`mix.css('src/tailwind.css', 'assets/application.css')`





## JSON Template
### JSON templates must be valid JSON files. The root shoudl be an object with the following attributes:
name
layout: optional
wrapper: optional
sections
order

- create json file
- create a section in SECTIONS object and write SECTION ID
- add a TYPE
- add a SECTION ID to ORDER array
- Then create a Liquid page in sections folder and name it the same as the section type you named
- In this liquid page you can write the html and settings of this page.