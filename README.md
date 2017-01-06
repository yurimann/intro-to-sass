## Introduction to Sass
After doing this assignment, you should have an understanding of:

- Basic Sass features
  - variables
  - partials & imports
  - nesting
  - using mixins

In this exercise you'll take an existing stylesheet and use the power of Sass to make it more readable and maintainable.

You'll find a simple Rails app in this repo. This app has one controller and one view (`films#index`). The `index.html.erb` has the markup for the page and `app/assets/stylesheets/films.scss` has the existing styles.

You'll find a lot of help in the [Sass Documentation](http://sass-lang.com/documentation/file.SASS_REFERENCE.html)!

### Tasks
1. Move all of the `color` and `font-family` values into Sass variables at the top of `films.scss`
2. Refactor any repeated selectors into nested selectors
3. Use the provided `clearfix` mixin (with the `@include` syntax) instead of the `overflow` property in all places where it's being used to clear floated child elements
3. Split the styles into five (5) partials:
  - `_variables.scss` for all of the variables you defined in step 1
  - `_mixins.scss` for the clearfix mixin (and any others you invent!)
  - `_base.scss` for the basic tag level selectors
  - `_hero.scss` for all the styles related to the hero block
  - `_article.scss` for all the styles related to the article

    **Your `films.scss` should be empty by the end of this step!**
4. Import (using `@import`) your partials into `films.scss`
5. Make sure it still looks exactly the same!
6. Now make it your own!
