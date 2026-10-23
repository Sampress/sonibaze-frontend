# Personal Portfolio Website

A responsive personal portfolio website built with HTML and CSS. The
project focuses on presenting work samples and organizing page content
into reusable sections and cards.

## Overview

This project includes a portfolio-style layout with navigation, content
sections, work cards, and a footer. Styling is organized through CSS
custom properties to keep colors, typography, spacing, and transitions
consistent across the site.

## Features

-   **Navigation:** Styled navigation links with hover states.
-   **Portfolio section:** Work cards for projects such as Interior
    Design, Web Development, and Personal Development.
-   **Reusable layout classes:** Grid-style columns using `.row`,
    `.col-1-3`, and `.col-1-2`.
-   **Design tokens:** CSS custom properties for colors, typography,
    spacing, and other shared values.
-   **Interactive visual effects:** Hover transitions and image scaling
    on work cards.
-   **Consistent typography:** Open Sans and Raleway font stacks with
    system fallbacks.
-   **Responsive image sizing:** Images are intended to remain within
    their card containers.

## Technologies

-   HTML5
-   CSS3
-   CSS custom properties (variables)
-   Flexibility with standard browser features; no JavaScript framework
    is required for the styling described here

## Project Structure

The project structure may vary depending on the files in your local
repository. Based on the files and paths used in the project, the
relevant files are expected to follow a structure similar to:

``` text
.
├── index.html
├── images/
│   ├── pic-work-01.jpg
│   ├── pic-work-02.jpg
│   └── pic-work-03.jpg
└── styles/
    ├── 2-style.css
    ├── 3-style.css
    └── 10-style.css
```

Update this tree if your repository contains additional pages,
stylesheets, scripts, or assets.

## Getting Started

### Prerequisites

-   A modern web browser
-   A code editor such as Visual Studio Code

### Run Locally

1.  Clone or download the repository.
2.  Open the project folder in Visual Studio Code.
3.  Confirm that the HTML file references the correct stylesheet and
    image paths.
4.  Open `index.html` in a browser, or use a local development extension
    such as Live Server if it is installed.

No build step is described for this project; if your repository includes
a package manager or build tooling, follow the scripts defined in its
configuration files.

## Styling Notes

The CSS uses shared custom properties for consistent design values. The
project has used tokens for colors such as:

-   Primary: `#d73953`
-   Black: `#090909`
-   White: `#ffffff`
-   Light grey: `#f3f3f3`
-   Dark grey: `#353535`

The work cards use a nested structure similar to:

``` html
<li class="col-1-3">
  <article class="card-work">
    <div class="card-outer">
      <div class="card-image">
        <img src="images/pic-work-01.jpg" alt="Interior Design">
      </div>
      <div class="card-inner">
        <h3 class="card-title">
          <a href="#">Interior Design</a>
        </h3>
      </div>
    </div>
  </article>
</li>
```

For images to stay within their card, a common baseline is:

``` css
.card-image img {
  display: block;
  max-width: 100%;
  height: auto;
}
```

If each image should fill the card width, use `width: 100%` as well.
Ensure the column and its descendants do not have conflicting fixed
widths.

## Development Guidelines

-   Keep HTML semantic and accessible.
-   Use descriptive `alt` text for meaningful images; use empty `alt=""`
    only for decorative images.
-   Reuse CSS custom properties instead of repeating design values.
-   Keep class names consistent with the existing project conventions.
-   Check the layout at different viewport widths.
-   Verify that image paths and stylesheet links are correct before
    committing changes.

## Testing Checklist

-   [ ] The page loads without missing stylesheets or images.
-   [ ] Navigation links are visible and usable.
-   [ ] Work cards align as intended.
-   [ ] Images remain within their card containers.
-   [ ] Hover effects work without causing unwanted overflow.
-   [ ] The layout remains usable at narrower viewport widths.
-   [ ] Meaningful images have appropriate alternative text.

## Contributing

1.  Create a branch for your change.
2.  Make focused updates that follow the existing HTML and CSS
    conventions.
3.  Test the page in a browser.
4.  Submit a pull request with a clear description of the change.

## License

No license information was available in the project context. Add a
license before distributing or reusing the project if needed.
