# Technology Stack

## File structure

MacPaw Site created using [Laravel](https://laravel.com/). Accordingly, we use the file structure proposed by the framework. All source files are in /resources/assets folder. Localizations are in /resources/lang folder. Templates are in /resources/view

## Compiling assets

For compiling assets we are using Laravel Mix. All available information you can find [here](https://laravel.com/docs/master/mix). Also we have added few things to improve development experience like automated svg sprites generation.

### Styles

We are using [SASS](https://sass-lang.com/) for writing styles. Also BEM as a naming system.

```css
.block            (<div class="post"></div>)
.bock-element     (<div class="post-head"></div>)
.-modifier        (<div class="post -slim"></div>)
```

### Templates

We are using [Blade](https://laravel.com/docs/master/blade) template engine for creating templates.

### Java Script

Currently, we are using ES6 standart. For handling legacy browsers we have configured Babel compiler. we also have a customized ESLint to stick to the same coding style \(extended from [eslint:recommended](https://eslint.org/docs/rules/) config + few own rules\). It can be checked in .eslintrc file

