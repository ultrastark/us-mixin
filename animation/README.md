# us-mixin - animation

contain scss mixin for different kind of animation

`This is an early version. This may change a lot in the future and some mixin could be broken.`

## Installing

In the working repository

```
npm i @ultrastark/us-mixin --save
```

Then import it in you style.scss and everywhere where you need it

```
@import '~@ultrastark/us-mixin/animation/mixin';
```

## List of mixins

**pulse**
@include pulse(); // Default values : pulse($duration: 2.5s, $scale: 1.1, $curve: ease, $infinite: true)

@include pulse(3s, 2, ease-in-out, false); // no animation (default forwards)

@include pulse(3s, 2, ease-in-out, backwards);

**spin**
@include spin(); // Default values : spin($velocity: 1.5s, $curve: ease, \$mode: infinite)

@include spin(3s, ease-in-out, false); // no animation (default forwards)

## How to use

When installed, simply use it in your scss file

`In angular, for exemple, you need to import it in every file where you want to use it`

`I recommend you to create a shared.scss file that contain every mixin you want to share`

**`@todo`** [`See the exemple`](https://github.com/rbalet/us-mixin)

```
.logo {
  @include pulse();
  @include spin();
}
```

## Authors

- **Raphaël Balet** - _Initial work_ - [Ultrastark](https://ultrastark.ch)

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details

## Acknowledgments

- [Glenn McComb](https://glennmccomb.com/articles/creating-smooth-sequential-animations-with-sass/)
