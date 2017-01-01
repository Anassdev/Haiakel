# Setup
1. Link to `haiakel.min.css` in your HTML document `<head>` :

  ``` HTML
  <link rel="stylesheet" href="haiakel.min.css">
  ```
  Now, you have `Haikal` in your Project.


# How to use:
  * All classes in `Haiakel` start with `h` letter, (You can change it in `haiakel.scss` file):
    #### Example:
    ``` HTML
    <div class="container">
      <div class="h-small-12 h-medium-6 h-large-4">
        // Your Element 1
      </div>
      <div class="h-small-12 h-medium-6 h-large-4">
        // Your Element 2
      </div>
    </div>
    ```

  * There are 3 different sizes in `Haiakel` :

| Device Tag | Breakpoint | Class (x = Column Size) |
| --- | --- | --- |
| small | < 576px | h-small-x |
| medium | < 992px | h-medium-x |
| large | > 992px | h-large-x |

  * You can remove gutter (space between columns) by add `t-no-gutter` class to `column` or `container` or `container-fluid` or `row` :
  #### Example:
    ``` HTML
    // Remove gutter to all elements in container
    <div class="container h-no-gutter">
      <div class="h-small-12 h-medium-6 h-large-4"></div>
    </div>

    // Remove gutter to all elements in row
    <div class="row t-no-gutter">
      <div class="h-small-12 h-medium-6 h-large-4"></div>
    </div>

    // Remove gutter to special element
    <div class="h-small-12 h-medium-6 h-large-4 h-no-gutter"></div>
    ```
  * Or remove gutter to special device size (`h-small-no-gutter`, `h-medium-no-gutter`, `h-large-no-gutter`) :
    #### Example:
    ``` HTML
    <div class="h-small-12 h-small-no-gutter h-medium-6 h-large-4"></div>
    ```

  * Offset & pull & push `h-x-offset-y`, `h-x-pull-y`, `h-x-push-y` (x = Device Tag, y = Column Size):
  #### Example:
    ``` HTML
    // Offset (Empty space before column)
    <div class="h-large-4 h-large-offset-4"></div>

    // Pull (Pull column to the left without affecting on the other columns)
    <div class="h-large-4 h-large-pull-4"></div>

    // Push (Push column to the right without affecting on the other columns)
    <div class="h-large-4 h-large-push-4"></div>
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
  
