## Example

### Input

```scss
@import "~sass-mixin-important/important.scss";

$important-repeat-count: 100;

// Repeat ".color-red" $important-repeat-count times.
@include important(color-red) {
  color: red;
}

// Repeat ".color-yellow" 3 times.
@include important(color-yellow, 3) {
  color: yellow;
}

.color-blue {
  display: inline;

  // Make only specific properties equivalent to "!important".
  @include important("&.color-blue", 3) {
    color: blue;
  }
}
```

### Output

```css
.color-red.color-red.color-red.color-red.color-red.color-red.color-red.color-red.color-red.color-red.color-red.color-red.color-red.color-red.color-red.color-red.color-red.color-red.color-red.color-red.color-red.color-red.color-red.color-red.color-red.color-red.color-red.color-red.color-red.color-red.color-red.color-red.color-red.color-red.color-red.color-red.color-red.color-red.color-red.color-red.color-red.color-red.color-red.color-red.color-red.color-red.color-red.color-red.color-red.color-red.color-red.color-red.color-red.color-red.color-red.color-red.color-red.color-red.color-red.color-red.color-red.color-red.color-red.color-red.color-red.color-red.color-red.color-red.color-red.color-red.color-red.color-red.color-red.color-red.color-red.color-red.color-red.color-red.color-red.color-red.color-red.color-red.color-red.color-red.color-red.color-red.color-red.color-red.color-red.color-red.color-red.color-red.color-red.color-red.color-red.color-red.color-red.color-red.color-red.color-red {
  color: red;
}

.color-yellow.color-yellow.color-yellow {
  color: yellow;
}

.color-blue {
  display: inline;
}
.color-blue.color-blue.color-blue.color-blue {
  color: blue;
}
```
