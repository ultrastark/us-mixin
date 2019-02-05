# us-mixin - grid

contain scss mixin for colors and instantiate class name

## Installing

In the working repository

```
npm i @ultrastark/us-mixin --save
```

Then import it in you style.scss and everywhere where you need it

```
@import '~@ultrastark/us-mixin/color/mixin';
```

You need to create yourself a color map which have to look like the following (only the **base is needed**)
It's better to add this one in the main.scss file, (or if you follow the [sass 7-1 pattern]()`@todo` under base/colors).

```
$colors: (
  'primary': (
    light: #ffa,
    base: #ffb,
    dark: #ffc,
  ),
  'secondary': (
    light: #ffd,
    base: #ffe,
    dark: #fff,
  ),
  'default': (
    success: #28a745,
    danger: #dc3545,
    warning: #ffc107,
    dark: #343a40,
    light: #fff,
    muted: #6c757d,
  ),
);
```

## List of mixins

**included**

```
color: color(); //for primary
color: color('secondary');
color: color('secondary', 'light'); // Shade
color: color('secondary', 'light', 0.5); // Shade and alpha
```

## How to use

When installed, simply use it in your scss file

`In angular, for exemple, you need to import it in every file where you want to use it`

`I recommend you to create a shared.scss file that contain every mixin you want to share`

**`@todo`** [`See the exemple`](https://github.com/rbalet/us-mixin)

```
h1 {
  border: color();
  color: color('primary', 'light');
  background: color('secondary', 'light', 0.5);
}
<div class="bg-primary color-primary border-primary"></div>
<div class="bg-secondary-light color-secondary-dark border-default-warning"></div>
```

## Authors

- **Raphaël Balet** - _Initial work_ - [Ultrastark](https://ultrastark.ch)

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details

## Acknowledgments

- [Bootstrap Grid](https://getbootstrap.com/docs/4.0/layout/grid/)
