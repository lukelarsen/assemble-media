[Assemble]:                http://assemblecss.com
[Assemble Base]:           https://github.com/lukelarsen/assemble-base

# Assemble Media
Assemble Media is a component of the [Assemble] CSS Framework. It will give you a solid base for using media players in your project. It has some default styles that can easily be overridden so you can add your own look.

## Requirements
Assemble Media requires [Assemble Base].

## Installation
npm install assemble-media --save-dev

## Usage
Import the _assemble-media.css file from your css file.
```css
@import '../node_modules/assemble-base/base';

/*
Override variables here before the Assemble Components are loaded.
*/

@import '../node_modules/assemble-media/assemble-media';
```
### HTML
```html
<div class="media">
    <iframe src="https://www.youtube.com/embed/9_lyJt2T3GY" frameborder="0" webkitallowfullscreen="" mozallowfullscreen="" allowfullscreen=""></iframe>
</div>


<div class="media">
    <iframe frameborder="0" scrolling="no" marginheight="0" marginwidth="0" src="http://maps.google.co.uk/maps?q=glasgow&amp;ie=UTF8&amp;hq=&amp;hnear=Glasgow,+Glasgow+City,+United+Kingdom&amp;gl=uk&amp;t=m&amp;z=11&amp;iwloc=A&amp;output=embed"></iframe>
    <br>
    <small><a href="http://maps.google.co.uk/maps?q=glasgow&amp;ie=UTF8&amp;hq=&amp;hnear=Glasgow,+Glasgow+City,+United+Kingdom&amp;gl=uk&amp;t=m&amp;z=11&amp;iwloc=A&amp;source=embed" style="color: #0000FF; text-align: left">View Larger Map</a></small>
</div>
```

## Options
Options are set with variables. These variables are already set with their default values so they will just work out of the box. If you wish to change them just define the variable you want to change before you load the _assemble-media.css file. You may wish you see [Assemble Base] for more examples and directions for setting up a Assemble project.

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
Usage
```html
<div class="media media--vimeo">
    <iframe src="http://player.vimeo.com/video/132181019" frameborder="0" webkitallowfullscreen="" mozallowfullscreen="" allowfullscreen=""></iframe>
</div>
```

##### $media--instagram
- Turn on/off the Instagram player. If true a class of .media--instagram will be generated.
- Default: false;
- Type: Boolean
```css
$media--instagram: true;
```
Usage
```html
<div class="media media--instagram">
    <iframe src="http://instagram.com/p/dJJvzMI4X8/embed/" frameborder="0" scrolling="no" allowtransparency="true"></iframe>
</div>
```

##### $media--vine
- Turn on/off the Vine player. If true a class of .media--vine will be generated.
- Default: false;
- Type: Boolean
```css
$media--vine: true;
```
Usage
```html
<div class="media media--vine">
    <iframe src="https://vine.co/v/bYwPIluIipH/embed/simple" frameborder="0" scrolling="no" allowtransparency="true"></iframe>
</div>
```