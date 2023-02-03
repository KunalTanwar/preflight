# Preflight

A modern alternative of CSS Resets.

## What does it do?

-   Corrects bugs and common browser inconsistencies.
-   Improves usability with subtle modifications.
-   Explains what code does using detailed comments.

## Some Features

-   All `elements` have `position: relative` by default. So, while using `position: absolute` on a child element you don't need to worry about origins.
-   Heading tags such as `h1, h2, h3, h4, h5, h6` have reponsive `font-size`.
-   Elements like `canvas, iframe, img, object, svg, video` will not get overflowed or chopped off from the screen or cause any vertical/horizontal scrollbars.

## Use with a CDN

To rapidly include the minified production file in your webpage.

```html
<link
    rel="stylesheet"
    href="https://cdn.jsdelivr.net/gh/KunalTanwar/preflight/dist/css/preflight.min.css"
/>
```

```css
@import url('https://cdn.jsdelivr.net/gh/KunalTanwar/preflight/dist/css/preflight.min.css');
```

### An Alternative Version

In this version [Inter](https://rsms.me/inter/) is set as default font with fallbacks. Also contains different character variant : `'cv07', 'cv08', 'cv10'`;

You can find more character variants [here](https://rsms.me/inter/#features/cvXX)

```html
<link
    rel="stylesheet"
    href="https://cdn.jsdelivr.net/gh/KunalTanwar/preflight/dist/css/preflight.inter.min.css"
/>
```

```css
@import url('https://cdn.jsdelivr.net/gh/KunalTanwar/preflight/dist/css/preflight.inter.min.css');
```

You can add **Inter** manually or just copy the below code and paste it before `preflight.inter.min.css`.

```html
<link rel="preconnect" href="https://rsms.me/" />
<link rel="stylesheet" href="https://rsms.me/inter/inter.css" />
```

## Raw Files

-   [`preflight.scss`](https://cdn.jsdelivr.net/gh/KunalTanwar/preflight/src/scss/preflight.scss)
-   [`preflight.inter.scss`](https://cdn.jsdelivr.net/gh/KunalTanwar/preflight/src/scss/preflight.inter.scss)
-   [`preflight.prefixed.css`](https://cdn.jsdelivr.net/gh/KunalTanwar/preflight/dist/css/preflight.prefixed.css)
-   [`preflight.inter.prefixed.css`](https://cdn.jsdelivr.net/gh/KunalTanwar/preflight/dist/css/preflight.inter.prefixed.css)
-   [`preflight.min.css`](https://cdn.jsdelivr.net/gh/KunalTanwar/preflight/dist/css/preflight.min.css)
-   [`preflight.inter.min.css`](https://cdn.jsdelivr.net/gh/KunalTanwar/preflight/dist/css/preflight.inter.min.css)

## Bug

In chrome some emojis will replace by symbols. In that case, you can wrap that emoji inside a `span` tag and apply :

```css
.emoji {
    font-family: var(--emoji-font); /* available globally */
}
```

There is an open [bug](https://bugs.chromium.org/p/chromium/issues/detail?id=964527) about this if you are interested.

## Contributing

Please read the [contribution guidlines](CONTRIBUTING.md) in order to make the contribution process easy and effective for everyone involved.
