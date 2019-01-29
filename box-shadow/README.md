# us-mixin - box-shadow

contain scss mixin for box shadow

## Example

[See it on codepen](https://codepen.io/rbalet/pen/VgKvyZ)

## Installing

In the working repository

```
npm -i @ultrastark/us-mixin --save
```

Then import it in you style.scss

```
@import '~@ultrastark/us-mixin/box-shadow/mixin';
```

or with angular, inside the **angular.json** file

```
"styles": [
    "node_modules/@ultrastark/us-mixin/box-shadow/mixin.scss",
    "src/theme/styles.scss"
  ],
```

## List of mixins

**included**

```
 @include box-shadow();
 @include box-shadow(2);
 @include box-shadow(3);
 @include box-shadow(4);
 @include box-shadow(5);
```

## How to use

When installed, simply use it in your scss file

`In angular, for exemple, you need to import it in every file where you want to use it`

`I recommend you to create a shared.scss file that contain every mixin you want to share`

**`@todo`** [`See the exemple`](https://github.com/rbalet/us-mixin)

```

```

## Authors

- **Raphaël Balet** - _Initial work_ - [Ultrastark](https://ultrastark.ch)

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details

## Acknowledgments

- [Florian Kutschera](https://medium.com/@Florian/freebie-google-material-design-shadow-helper-2a0501295a2d)

- [Samuel Thornton](https://codepen.io/sdthornton/pen/wBZdXq)
