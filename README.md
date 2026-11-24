# DriveEase Motors

A single-page car showroom demo built with HTML and CSS. It works offline and
does not need a server or any installed packages.

## Open the project

1. Keep `index.html`, `style.css`, and the `images` folder together.
2. Double-click `index.html` to open the website in a browser.
3. Use the navigation links to jump to the page sections. The test-drive form
   demonstrates the browser's required-field checks, but is not connected to a
   booking service. Do not enter real personal details in this demo.

## Replace the placeholder illustrations

The `images` folder contains local SVG illustrations so the page works without
an internet connection. Replace them with your own car photos by putting image
files in `images` and updating the matching `src` in `index.html`:

- `car1.svg` through `car6.svg` are the six car-card illustrations.
- `hero.svg` is the large banner illustration.

For example, save your Swift photo as `images/car1.jpg` and change that card's
image path to `images/car1.jpg`. Repeat for `car2.jpg` through `car6.jpg` and
`hero.jpg`. Keep meaningful `alt` text describing each image.

## Change the colors

Open `style.css` and edit the variables near the top in the `:root` section.
For example, `--color-primary` controls the main buttons and highlights, while
`--color-ink` controls most text. Other variables set the page background,
spacing, card corners, and shadows.

## Flexbox in this project

- `display: flex` turns an element into a flexible container for its children.
- `flex-direction` chooses a row or column; small screens stack some content
  into columns.
- `justify-content` distributes items along the main direction, and
  `align-items` aligns them across it.
- `flex-wrap: wrap` lets cards and form fields move onto another line when
  there is not enough room.
- `gap` adds even space between flex items without adding margins to each one.
- `flex` controls how an item can grow or shrink and its starting width. For
  example, the car cards use `flex: 1 1 300px` so they wrap into columns that
  fit the available space.

The comparison table has its own horizontal scroll wrapper on narrow screens.
All page layouts use Flexbox; the table uses regular HTML table layout.

## Before presenting

Check the page at 360px, 768px, and 1280px widths. Click each navigation link,
scroll the comparison table on a phone-sized screen, tab through the controls
to check visible focus, and try submitting the form with required fields left
empty. The example prices and specifications are indicative; verify current
details and safety ratings before presenting them as buying advice.
