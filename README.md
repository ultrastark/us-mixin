# us-mixin

More infos and example under https://docs.ultrastark.ch/docs/en/projects/us-mixin/description/

## Quick start

In the working repository

```
npm i @ultrastark/us-mixin@latest --save
```

Then import in the following order in you main.scss style and where you need it

```
@import 'myColor.scss';
@import '~@ultrastark/us-mixin/mixin';
@import '~@ultrastark/us-mixin/utilities';
```

**Note**
- myColor.scss and us-mixin/mixin have to be imported in every scss file that needs they mixins
- us-mixin/utilities should be imported **only once**. If not, it's gonna create useless classes
- mixin and utilities work good together but you could only use one of the both if you need it

**Attention**
If you use the `color mixin` and want custom color, you need another step: [wiki](https://github.com/ultrastark/us-mixin/wiki/color)


## Authors

- **Raphaël Balet** - _Initial work_ - [Ultrastark](https://ultrastark.ch)

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details
