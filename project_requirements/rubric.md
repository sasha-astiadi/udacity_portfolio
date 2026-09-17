# Project Rubric

Use this rubric to understand and assess the project criteria.

## Basic Requirements

### Follow Wireframes to Build a Project Layout

* The page structure matches the provided wireframes.
* The logo, if included, is positioned at the opposite end from the navbar.
* Proportions, alignment, and placement of elements are consistent with the design.

### Create a Responsive Design That Adapts to Different Screen Sizes

* Pages adjust appropriately for desktop, tablet, and mobile views.
* No elements overflow or break the layout when resizing the browser window.

---

## Methodology

### Organize Files with a Clear Structure Based on BEM Methodology

* The `scss`/`less` folder structure includes separate folders for:

  * `base`
  * `blocks`
  * `utils`
* Each folder has a main stylesheet matching the folder name (e.g., `base.scss`, `blocks.less`) unless using the **granular approach**, in which case no `utils` file is needed.
* Block names reflect the component's purpose (e.g., `header`, `button`, `bio`) rather than descriptive names (e.g., `large-text`).
* If using the **aggregated approach**, a `utils.scss` or `utils.less` file consolidates utilities such as `_variables` and `_mixins` for import into blocks.
* If using the **granular approach**, `_variables` and `_mixins` are imported directly into block files as needed.

### Apply the BEM Methodology to Structure CSS

* Class names created in preprocessor files use the **BEM methodology**.
* Class names are logical and consistent, reflecting the page's structure.

For more information, refer to the official [**BEM Methodology documentation**](https://en.bem.info/methodology/quick-start/).

---

## Preprocessors

### Compile Preprocessor Stylesheets into a Primary CSS File

* The `/dist` folder contains a `main.css` file.
* `main.css` is compiled using a preprocessor through console commands.

### Use Variables and Mixins for Reusable Styles

* Variables are defined for reusable values, such as:

  * `$primary-color`
  * `@font-size-base`
* Variables are applied consistently across SCSS/Less files.
* At least one mixin is created for common patterns, such as media queries or reusable styles.
* Mixins are used effectively across SCSS/Less files.

### Apply Nesting to Organize Related Styles Hierarchically

* BEM element and modifier selectors are declared in a nested format to avoid repetition.
* A `.block` selector should contain related `&__element` selectors.
* Modifiers should be nested under their respective blocks and elements using the `&_modifier` syntax.
* Avoid deep nesting to maintain readability and maintainability.

Example:

```scss
.block {
  &__element {
    // styles
  }

  &__element_modifier {
    // styles
  }
}
```

---

## CSS Techniques

### Implement Advanced CSS Properties

At least one of the following advanced CSS properties or techniques must be present:

* `calc()`
* Scroll Snap
* Inset text color
* Anchor
* Color Scheme Media Query
* `backdrop-filter`
* `min()`
* `max()`

### Enhance Interactivity with CSS Animations and Transitions

* Buttons change background color when hovered over or clicked/tapped.
* Button color transitions should be smooth.
* Include at least one additional transition or animation technique, such as:

  * Hover transitions affecting properties other than color.
  * Animations defined with `@keyframes`.
* Effects should be smooth, non-distracting, and appropriate to the design.

### Incorporate Responsive Animations and Dynamic Effects

The navigation header must minimize its height when the user scrolls down.

In addition to the navigation behavior, implement at least one of the following:

* On-scroll effects
* Animated backgrounds
* Turning off animations via media queries

---

## Accessibility

### Ensure Proper Semantic HTML and Relationships

* Use semantic HTML elements correctly:

  * `header`
  * `footer`
  * `main`
  * `section`
  * `h1`–`h6`
* Heading tags descend in the correct order.
* Labels are properly associated with input fields using the `for` attribute, if applicable.

### Provide Accessible Non-Text Content

* All images include meaningful `alt` attributes.
* Decorative images use `alt=""`.
* Icons or links without visible text use `aria-label` or are wrapped in a visually hidden class such as `sr-only`.
* Form buttons have descriptive text or appropriate `aria-label` attributes.

### Ensure Keyboard and Focus Accessibility

* All functionality is accessible via the keyboard.
* Users can tab through links and buttons.
* Focus order is logical and intuitive.
* Keyboard focus never becomes trapped.
* Focused elements are visibly highlighted.

### Use Color and Sensory Characteristics Accessibly

* Color is not the sole method of conveying information.
* Links are distinguishable from surrounding text without relying solely on color.
* Text and background colors meet a minimum contrast ratio of **4.5:1**.

---

# Suggestions to Make Your Project Stand Out

### Intro Animations

Consider adding animations that make elements appear when the page loads, such as:

* Fade-in effects
* Slide-in animations
* Subtle movement

Keep animations smooth and unobtrusive.

### Additional Sections

The suggested navbar items represent pages or sections commonly found on a portfolio website.

Consider creating:

* A dedicated **Projects** page
* A **Resume** page
* A **Skills** section
* A **Contact** section

Projects and resumes can have dedicated pages, while Skills and Contact could also be included directly on the homepage.

### Custom Background Images

You can find free background images at [**Pexels**](https://www.pexels.com/).

These images can help you:

* Customize your portfolio
* Establish a visual theme
* Inspire your color palette
* Create a more distinctive design
