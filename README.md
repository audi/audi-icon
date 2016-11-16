# Audi Icon

## General Usage

All Audi Icons come in two sizes
- small: 24px
- large: 48px

## SVG

### Add the Audi Icon CSS
To style the Audi Icon SVGs, add the Audi Icon CSS to your website.

The CSS is located in the `dist/css` folder.

``` html
<link href="audi-icon.min.css" rel="stylesheet">
```

### Using Audi Icon SVGs
We like SVGs and we think they're the way to display icons on the web. Since Audi Icons are just basic SVGs, we suggest you display them like you would any other image (don't forget the alt attribute).

All SVGs are located in the `dist/svg/static` folder.

``` html
<img class="audiicon" src="icon-name-small.svg" alt="icon name">

<!-- or large -->
<img class="audiicon audiicon--large" src="icon-name-large.svg" alt="icon name">
```

### Using Audi Icon SVG Sprite

Audi Icons also come in a SVG sprite which allows you to display all the icons in the set with a single request. It's like an icon font, without being a hack.

Adding an icon from an SVG sprite is a little different than what you're used to, but it's still a piece of cake.

The SVG Sprite is located in the `dist/svg/sprite` folder.

``` html
<svg class="audiicon">
  <use xlink:href="sprite.svg#audiicon-icon-name-small"></use>
</svg>

<!-- or large -->
<svg class="audiicon audiicon--large">
  <use xlink:href="sprite.svg#audiicon-icon-name-large"></use>
</svg>

<!-- or both to switch between the two sizes -->
<style media="screen">
  @media (min-width: 1024px) {
    .audiicon {
      width: 48px;
      height: 48px;
    }
    .audiicon-small {
      visibility: hidden;
    }
    .audiicon-large {
      visibility: visible;
    }
  }
</style>
<svg class="audiicon">
  <use xlink:href="sprite.svg#audiicon-icon-name-small" class="audiicon-small"></use>
  <use xlink:href="sprite.svg#audiicon-icon-name-large" class="audiicon-large"></use>
</svg>
```

Coloring icons is really easy. Because all fills and strokes use `currentColor`, all you need to do is set the color rule on the `<svg>` tag.

``` css
.audiicon {
  color: white;
}
```

To learn more about SVG Sprites, read [Chris Coyier's guide](http://css-tricks.com/svg-sprites-use-better-icon-fonts/).

## PNG
You can find our default stylesheets in `dist/css` and the PNGs in `dist/png`.

``` html
<link href="audi-icon.min.css" rel="stylesheet">
```

``` html
<img class="audiicon" src="icon-name-small.png" alt="icon name">

<!-- or large -->
<img class="audiicon audiicon--large" src="icon-name-large.png" alt="icon name">

<!-- or double sized for high resolution displays -->
<img class="audiicon" src="icon-name-small.png" srcset="icon-name-small.png 1x, icon-name-small-2x.png 2x" alt="icon name">
<img class="audiicon audiicon--large" src="icon-name-large.png" srcset="icon-name-large.png 1x, icon-name-large-2x.png 2x" alt="icon name">
```

## Icon font
You can find our default stylesheets in `dist/css` and the fonts in `dist/font`.

``` html
<link href="audi-glyph.min.css" rel="stylesheet">
```

``` html
<span class="audiglyph audiglyph-icon-name" title="icon name" aria-hidden="true"></span>

<!-- or large -->
<span class="audiglyph audiglyph-icon-name audiglyph--large" title="icon name" aria-hidden="true"></span>
```

## Demo page

You can use [Browsersync](https://www.browsersync.io/) and the following one-liner to get a demo page with all Audi Icons in action.

```
npm install -g browser-sync
npm run demo
```

## License

© Audi, 2016.
