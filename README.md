# Peculiar

A free icon set drawn entirely in CSS — no images or fonts, and only one
extra HTTP request for the stylesheet. 43 icons, each built from plain
`<div>` elements on a 16×16px grid.

## Usage

Include the stylesheet:

```html
<link rel="stylesheet" href="peculiar.css">
```

Then compose an icon from its named parts:

```html
<div class="icon icon-minus">
  <div class="icon-minus-circle"></div>
  <div class="icon-minus-line"></div>
</div>
```

Every icon is an `.icon .icon-<name>` wrapper containing one element per
shape (`-circle`, `-line-1`, `-triangle`, …). The markup for all of them is
in `peculiar.html`.

## Icons

minus, plus, disc, clock, volume, pause, plasma, bulb, iphone, battery,
video, paper, smile, picture, comment, typing, screens, play, up, down,
back, forward, camera, yang, profile, folder, heart, cmd, mic, home,
olympic, hd, temp, off, cloud, coffee, eye, touch, repeat, eject, female,
feed, message.

The battery icon also has `red` and `green` variants:

```html
<div class="icon icon-battery red">…</div>
```

## Demo

Open `peculiar.html` in a browser to preview every icon.

## Notes

- Icons are 16×16px with a 16px margin on the wrapper; override `.icon` to
  place them differently.
- Colors are hard-coded black and white, so recolor an icon by overriding
  `background-color` or `border-color` on its inner classes.
