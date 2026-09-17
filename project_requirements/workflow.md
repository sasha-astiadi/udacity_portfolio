## Design Workflow

For this project, you are encouraged to implement your own design workflow. If you get stuck, use the following guide to get up and running.

### 1. Review the Wireframe

* Carefully study the provided wireframe to understand the expected layout for the **Intro Banner** and **Latest Projects** sections.
* Pay close attention to:

  * Spacing
  * Alignment
  * Element placement
  * Overall proportions
* You will be evaluated on your ability to match the provided wireframe.

### 2. Decide on a Visual Theme

Think about the overall aesthetics of your site:

* Will you use a **light or dark theme**?
* What colors will you use?
* How will you maintain visual consistency?
* How will your buttons look?

  * Rounded
  * Flat
  * With shadows
  * Or another style

Apply your design choices consistently to create a cohesive visual experience.

### 3. Set Up Your Project

Clone or download the starter project and set up your folder structure:

* Create `base`, `blocks`, and `utils` folders within your `scss` or `less` directory.
* Within these folders, create your base stylesheets that will use your future partials:

  * `base.scss`
  * `blocks.scss`
  * `utils.scss`
* Compile your CSS into a `main.css` file.
* Ensure the compiled CSS is output directly into the `dist` folder.
* Use **Live Preview** in Visual Studio Code or a similar tool to view your changes in real time.

### 4. Build Out Your Components

* The starter code provides the basic structure of the webpage.
* Build out the inner content while considering how each component fits within the overall hierarchy.
* Assign classes to your components using the **BEM methodology**:

  * Assign a general **block** class to each section.
  * Use **element** classes for components within each block.
  * Use **modifiers** when variations are needed.

### 5. Implement Accessibility Standards

Refer to the accessibility checklist to ensure your site meets **A and AA accessibility standards**.

Make sure to:

* Use semantic HTML elements for page structure.
* Provide descriptive `alt` attributes for images.
* Use ARIA labels where necessary.
* Ensure interactive elements are keyboard accessible.
* Test your site using accessibility tools such as:

  * **Lighthouse**
  * **WAVE**

### 6. Style Your Components

Once your HTML components are built and their classes have been assigned:

* Create a partial SCSS/Less file for each block.
* Within each partial, recreate the appropriately nested structure using the **BEM methodology**.
* Create any mixins or variables you need.
* A good starting point is:

  * Variables for colors and other reusable values.
  * Mixins for media queries and repeated styling patterns.
* Once your structure, mixins, and variables are established, style each section as needed.
* As you add styles, look for repeated patterns in your code and consider refactoring them into reusable **mixins or variables**.

### 7. Test Responsiveness

Use your browser's developer tools to simulate:

* Mobile
* Tablet
* Desktop

Confirm that:

* The layout adapts correctly.
* Elements don't overlap.
* Content remains aligned.
* Navigation doesn't overflow.
* Images and text remain readable at different screen sizes.

### 8. Iterate and Refine

* Revisit the provided wireframe regularly.
* Compare your implementation against the expected layout.
* Adjust spacing, sizing, alignment, and other visual details as needed.
* Refine your design for both visual balance and responsive behavior.

The goal is to create a polished, accessible, responsive portfolio homepage while demonstrating your understanding of **BEM, SCSS/Less, responsive design, and accessibility**.
