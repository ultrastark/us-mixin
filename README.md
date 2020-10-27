# us-mixin

More infos and example under https://docs.ultrastark.ch/docs/projects/us-mixin/description

**This repository is a beta version an may change in the future**

## 2.0.0 Release
**Attention**
* **us-mixin/grid** have no another sizing, see https://docs.ultrastark.ch/docs/projects/us-mixin/mixins/grid for me informations.
* ex: @include `@include sm {}` should now be `@include md{}`, `@include md{}` should now be `@include lg{}`, ...
* ex: @include `@include sm-md {}` should now be `@include sm-lg{}`, ...

**Removed**
* `xs` doesn't exist anymore since it was equal to 0
* `@include smOnly{}` since it's equal to `@include sm{}`



## Quick start

In the working repository

```
npm i @ultrastark/us-mixin@latest
```

Then import in the following order in you main.scss style and where you need it

```scss
@import 'myColor.scss'; //https://docs.ultrastark.ch/docs/projects/us-mixin/classes/color#installing
@import '~@ultrastark/us-mixin/mixin';
@import '~@ultrastark/us-mixin/utilities';
```

**Note**
- `us-mixin/mixin` have to be imported in every scss file that needs they mixins
- us-mixin/utilities should be imported **only once**. If not, it's gonna create useless classes
- mixin and utilities work good together but you could only use one of the both if you need it

**Attention**
If you use the `color mixin` and want custom color, you need another step: [wiki](https://github.com/ultrastark/us-mixin/wiki/color)


## Authors

- **Raphaël Balet** - _Initial work_ - [Ultrastark](https://ultrastark.ch)

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details
