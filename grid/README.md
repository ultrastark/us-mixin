# us-mixin - grid

contain scss mixin for grid and different OS

## Installing

In the working repository

```
npm -i us-mixin --save
```

Then import it in you style.scss

```
import 'us-mixin/grid/mixin.scss';
```

or with angular, inside the **angular.json** file

```
"styles": [
    "node_modules/us-mixin/grid/mixin.scss",
    "src/theme/styles.scss"
  ],
```

## List f mixins

**included**

```
@include sm {}
@include md {}
@include lg {}
@include xl {}
@include edge {}
@include ie {}
@include ios {}
@include safari {}
@include print {}
```

**Not included**

```
@include notSm {}
@include notMd {}
@include notLg {}
@include notXl {}
@include notEdge {}
@include notIe {}
@include notIos {}
@include notSafari {}
@include notPrint {}
```

## How to use

```
body {

  @include notIos {
    width: 100vw;
  }
}

p {
  font-size: 2em;

  @include xl {
    font-size: 1.5em;
  }

  @include sm {
    font-size: 1em;
  }

}
```
