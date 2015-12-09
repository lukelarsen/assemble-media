[Assemble]:                http://assemblecss.com
[Assemble Core]:           https://github.com/lukelarsen/assemble-core

# Assemble Media
Assemble Media is a component of the [Assemble] CSS Framework. It will give you a solid base for using media players in your project. It has some default styles that can easily be overridden so you can add your own look.

## Requirements
Assemble Media requires [Assemble Core].

## Installation
npm install assemble-media --save-dev

## Usage
### Gulp
```js
var gulp = require('gulp');
var postcss = require('gulp-postcss');
var assembleCore = require('assemble-core');
var assembleMedia = require('assemble-media');

gulp.task('css', function () {
    var processors = [
        assembleCore,
        assembleMedia
    ];
    return gulp.src('./src/*.css')
        .pipe(postcss(processors))
        .pipe(gulp.dest('./dest'));
});
```

## Options
Options are set with variables. These variables are already set with their default values so they will just work out of the box. If you wish to change them just define the variable you want to change before you load the _assemble-media.css file. You may wish you see [Assemble Core] for more examples and directions for setting up a Assemble project.

### Modifier Variables

##### $media--scroll
- Turn on/off scrolling in the media player. If true a class of .media--scroll will be generated.
- Default: false;
- Type: Boolean
```css
$media--scroll: true;
```

##### $media--vimeo
- Turn on/off the Vimeo media player. If true a class of .media--vimeo will be generated.
- Default: false;
- Type: Boolean
```css
$media--vimeo: true;
```

##### $media--instagram
- Turn on/off the Instagram player. If true a class of .media--instagram will be generated.
- Default: false;
- Type: Boolean
```css
$media--instagram: true;
```

##### $media--vine
- Turn on/off the Vine player. If true a class of .media--vine will be generated.
- Default: false;
- Type: Boolean
```css
$media--vine: true;
```