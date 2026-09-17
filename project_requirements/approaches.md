## Utility Organization with SCSS/Less and BEM

When working with **SCSS or Less** and the **BEM methodology**, you can choose between two approaches for organizing utilities:

1. **Aggregated Approach**
2. **Granular Approach**

Choose one approach and apply it consistently throughout your project.

---

## 1. Aggregated Approach

The aggregated approach uses a single `utils.scss` or `utils.less` file to aggregate all utility files. This file is then imported into each block file.

### SCSS Example

#### `utils.scss`

```scss
@use './variables';
@use './mixins';
```

#### `_header.scss`

```scss
@use '../utils/utils';

.header {
  background-color: utils.$primary-color;
  @include utils.flex-center;
}
```

### Less Example

#### `utils.less`

```less
@import './variables';
@import './mixins';
```

#### `header.less`

```less
@import '../utils/utils';

.header {
  background-color: @primary-color;
  .flex-center();
}
```

---

## 2. Granular Approach

With the granular approach, each block file directly imports only the utility files it needs.

### SCSS Example

#### `_header.scss`

```scss
@use '../utils/variables';
@use '../utils/mixins';

.header {
  background-color: variables.$primary-color;
  @include mixins.flex-center;
}
```

### Less Example

#### `header.less`

```less
@import '../utils/variables';
@import '../utils/mixins';

.header {
  background-color: @primary-color;
  .flex-center();
}
```

---

## Notes

* Choose **one approach**—aggregated or granular—and apply it consistently.
* SCSS users should use `@use` for modular imports.
* Less users should use `@import`.
* Organize your `utils` folder to store utility files such as:

  * `_variables.scss`
  * `_mixins.scss`
  * `variables.less`
  * `mixins.less`
* If you're using the **granular approach**, you don't need a `utils` file because your partials are imported directly into the block stylesheets.

Following these guidelines will help keep your styles organized, reusable, and consistent with the **BEM methodology**.
