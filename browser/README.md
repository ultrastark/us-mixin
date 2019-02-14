# us-mixin - grid

contain scss mixin for different browser

## Installing

In the working repository

```
npm i @ultrastark/us-mixin --save
```

Then import it in you style.scss and everywhere where you need it

```
@import '~@ultrastark/us-mixin/browser/mixin';
```

## List of mixins

```
@include chrome {}
@include edge {}
@include ie {}
@include ios {}
@include safari {}
@include print {}
```

**Every mixin have is own not**
Exemple

```
@include ie {}
@include notIe {}
```

## How to use

When installed, simply use it in your scss file

`In angular, for exemple, you need to import it in every file where you want to use it`

`I recommend you to create a shared.scss file that contain every mixin you want to share`

**`@todo`** [`See the exemple`](https://github.com/rbalet/us-mixin)

```
body {
  @include ie {
    display: none;
  }

  @include notIos {
    width: 100vw;
  }
}

```

## Authors

- **Raphaël Balet** - _Initial work_ - [Ultrastark](https://ultrastark.ch)

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details

## Acknowledgments

- @TODO
