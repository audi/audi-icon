# Audi Icons

## General Usage

All Audi Icons come in three sizes
- extra small: 16px
- small: 24px
- large: 48px

In addition, there is an active state for all icons in the size 'small'. They can be used, for example, in icon buttons or tags to support the indication of an active state.

## Icon font
The icon font comes in two styles: Regular (outlined icons) and Active (filled icons). You can find the font files in `dist/fonts`.

``` html
<link href="audi-glyph.min.css" rel="stylesheet">
```

``` html
<span class="audiglyph audiglyph-icon-name" title="icon name" aria-hidden="true"></span>

<!-- extra small -->
<span class="audiglyph audiglyph-icon-name audiglyph--xs" title="icon name" aria-hidden="true"></span>

<!-- large -->
<span class="audiglyph audiglyph-icon-name audiglyph--l" title="icon name" aria-hidden="true"></span>

<!-- active -->
<span class="audiglyph audiglyph-icon-name audiglyph--active-s" title="icon name" aria-hidden="true"></span>
```

## React
You can find our react icon files in `dist/react`.

## SVGs
We like SVGs and we think they're the way to display icons on the web. Since Audi Icons are just basic SVGs, we suggest you display them like you would any other image (don't forget the alt attribute).

All SVGs are located in `dist/svg`.

``` html
<img class="audiicon" src="icon-name-s.svg" alt="icon name">

<!-- extra small -->
<img class="audiicon audiicon--xs" src="icon-name-xs.svg" alt="icon name">

<!-- large -->
<img class="audiicon audiicon--l" src="icon-name-l.svg" alt="icon name">

<!-- active -->
<img class="audiicon audiicon--active-s" src="icon-name-active-s.svg" alt="icon name">
```

## Demo page

You can use [Browsersync](https://www.browsersync.io/) and the following one-liner to get a demo page with all Audi Icons in action.

```
npm install -g browser-sync
npm run demo
```
