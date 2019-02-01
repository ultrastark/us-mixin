# us-mixin

contain

- color

  - color-name, tone, alpha
  - Class generation
    - bg-{color-name}-{tone}
    - color-{color-name}-{tone}
    - border-{color-name}-{tone}

- shadow

  - normal
  - with animation
  - For svg (drop-shadow)

* grid & browser

  - sm, md, lg, xl
  - edge, ie, ios, safari, print

  **The following explanation help you to import all in one, for a granularity import see the readme inside each child folders**

## Installing

In the working repository

```
npm i @ultrastark/us-mixin --save
```

Then import it in you style.scss and everywhere where you need it

```
@import '~@ultrastark/us-mixin/mixin';
```

## List f mixins

### color

color: color();

color : color('secondary', 'light');

color : color('secondary', 'light', 0.5);

### shadow

@include box-shadow();

@include box-shadow(1,5);

@include drop-shadow();

@include drop-shadow(1,5);

### grid

@include sm, md, lg, xl { };

@include edge, ie, ios, safari, print { };

## How to use

When installed, simply use it in your scss file

`In angular, for exemple, you need to import it in every file where you want to use it`

`I recommend you to create a shared.scss file that contain every mixin you want to share`

**`@todo`** [`See the exemple`](https://github.com/rbalet/us-mixin)

```
// color
h1 {
  border: color();
  color: color('primary', 'light');
  background: color('secondary', 'light', 0.5);
}
<div class="bg-primary color-primary border-primary"></div>
<div class="bg-secondary-light color-secondary-dark border-default-warning"></div>

// shadow
.card {
  width: 95px;
  height: 95px;
  background: #f4f4f4;
  transition: all 250ms;
  @include box-shadow(); // No animation
}

.card-animated {
  @include box-shadow(1,3); // No animation
}

// grid
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

## Authors

- **Raphaël Balet** - _Initial work_ - [Ultrastark](https://ultrastark.ch)

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details

## Acknowledgments

- @see readme inside child folder
