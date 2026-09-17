## Project Instructions

### 1. Starter Code

* Download and unzip the provided [**starter code (opens in a new tab)**](https://github.com/udacity/cd14106-project-starter-code), which includes:

  * **Dist Folder**: Where your compiled CSS file (`main.css`) will live.
  * **Src Folder**:

    * `img`: Store all image files here. This folder contains a placeholder image for your Introduction Banner. You're welcome to use it, but you're encouraged to find your own image that better reflects your personality.
    * `scss_less`: Store all CSS preprocessor folders and files here. Rename this folder to match the preprocessor you're using (`scss` or `less`).
* Download the wireframes to guide the website layout for desktop and mobile views.

### 2. Folder Structure

Following the **BEM methodology**, your `scss` or `less` folder should contain `base`, `blocks`, and `utils` folders, along with a primary stylesheet that matches the preprocessor name.

* **Base**: Contains foundational styles such as resets, typography, and general element styles (e.g., `body`, headings, and links).
* **Blocks**: Houses styles for individual components, each in its own file, following the BEM methodology (e.g., `button.scss`, `header.scss`).
* **Utils**: Includes reusable helper styles such as variables, mixins, and utility classes that support the design system.
* Compile all preprocessor files into a single `main.css` file inside the `dist` folder.

### 3. Intro Banner

#### Content

Include:

* A background image for the banner.
* A bio section containing:

  * A profile image.
  * A main heading, such as `"[Your Name]'s Web Development Portfolio"`.
  * A short paragraph describing yourself.

> **Note:** If you don't feel comfortable using your own photo, you can use a placeholder image for this project. A professional headshot can positively contribute to your developer personal branding, but you don't have to make that decision just yet.

#### Responsive Behavior

* On larger screens, align the profile image and text content side by side.
* On mobile screens, stack the profile image above the text content.

### 4. Latest Projects Section

#### Content

Include:

* A heading, such as **"Latest Projects"**.
* Three project cards, each containing:

  * An image. Placeholder images are fine.
  * A title.
  * A short description.
* A centered button below the cards that links to a projects page.

#### Design

* Ensure all cards have equal width and height.
* Apply hover or keyboard-focus transitions to the project cards.

### 5. Navigation Header

Create a fixed navigation bar containing links for:

* Projects
* Skills
* Resume
* Contact

The navbar should:

* Stick to the top of the page.
* Shrink in height when the user scrolls.
* Display navigation links on desktop.
* Optionally collapse into a mobile-friendly **burger menu** on smaller screens.

> **Note:** If you choose not to incorporate a burger menu on mobile, you must still ensure the navigation is responsive and that the links do not overflow beyond the width of the header.

### 6. Footer

Create a footer at the bottom of the page containing copyright information, for example:

```html
&copy; [Your full name] 2025
```

### 7. Accessibility

Meet the **A and AA accessibility standards** outlined in the provided accessibility checklist.

## Example Style Folder Structure

```text
src
├── index.html
├── scss
│   ├── base
│   │   ├── _resets.scss
│   │   └── base.scss
│   ├── blocks
│   │   ├── _footer.scss
│   │   ├── _header.scss
│   │   ├── _any_block_partial.scss
│   │   └── blocks.scss
│   └── utils
│       ├── _mixins.scss
│       ├── _variables.scss
│       └── utils.scss
```

## Submission Instructions

### 1. Submission

Submit the entire project, including:

```text
dist/
└── main.css

src/
├── img/
├── scss/ or less/
└── index.html

package.json
```

The project should contain:

* **`dist`**: The compiled `main.css` file.
* **`src/img`**: Any images used in the project.
* **`src/scss` or `src/less`**: All preprocessor files and folders.
* **`src/index.html`**: The HTML file containing your web components.
* **`package.json`**: Allows reviewers to install dependencies if needed.

### 2. File Naming

Zip the complete project folder using the following naming convention:

```text
[first_name_lastname]_homepage
```

Then upload the resulting ZIP file for submission.
