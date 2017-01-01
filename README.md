# Setup
1. Link to `haiakel.min.css` in your HTML document `<head>` :

  ``` HTML
  <link rel="stylesheet" href="haiakel.min.css">
  ```
  Now, you have `Haikal` in your Project.


# How to use:
  * All classes in `Haiakel` start with `t` letter, (You can change it in `haiakel.scss` file):
    #### Example:
    ``` HTML
    <div class="container">
      <div class="t-small-12 t-medium-6 t-large-4">
        // Your Element 1
      </div>
      <div class="t-small-12 t-medium-6 t-large-4">
        // Your Element 2
      </div>
    </div>
    ```

  * There are 3 different sizes in `Haiakel` :

| Device Tag | Breakpoint | Class (x = Column Size) |
| --- | --- | --- |
| small | < 576px | t-small-x |
| medium | < 992px | t-medium-x |
| large | > 992px | t-large-x |

  * You can remove gutter (space between columns) by add `t-no-gutter` class to `column` or `container` or `container-fluid` or `row` :
  #### Example:
    ``` HTML
    // Remove gutter to all elements in t-container
    <div class="container t-no-gutter">
      <div class="t-small-12 t-medium-6 t-large-4"></div>
    </div>

    // Remove gutter to all elements in t-row
    <div class="row t-no-gutter">
      <div class="t-small-12 t-medium-6 t-large-4"></div>
    </div>

    // Remove gutter to special element
    <div class="t-small-12 t-medium-6 t-large-4 t-no-gutter"></div>
    ```
  * Or remove gutter to special device size (`t-small-no-gutter`, `t-medium-no-gutter`, `t-large-no-gutter`) :
  #### Example:
    ``` HTML
    <div class="t-small-12 t-small-no-gutter t-medium-6 t-large-4"></div>
    ```
  * Offset & pull & push `t-x-offset-y`, `t-x-pull-y`, `t-x-push-y` (x = Device Tag, y = Column Size):
  #### Example:
    ``` HTML
    // Offset (Empty space before column)
    <div class="t-large-4 t-large-offset-4"></div>

    // Pull (Pull column to the left without affecting on the other columns)
    <div class="t-large-4 t-large-pull-4"></div>

    // Push (Push column to the right without affecting on the other columns)
    <div class="t-large-4 t-large-push-4"></div>
    ```
# Customize:
  * You can customize `Haiakel` on `haiakel.scss` file.
  * Change columns number & gutter width:
  ``` SASS
  $grid-columns: 12;
  $gutter-width: 30px;
  ```
  
  * Change breakpoints:
  ``` SASS
  $small-device-breakpoint: 576px;
  $medium-device-breakpoint: 992px;
  ```
  
  * Change the class intro:
  ``` SASS
  $class-intro: "h";
  ```
  
  * Change devices tag:
  ``` SASS
  $small-device-tag: "small";
  $medium-device-tag: "medium";
  $large-device-tag: "large";
  ```
  
  * Change LTR to RTL (true = RTL):
  ``` SASS
  $direction-rtl: false;
  ```
  
