# us-mixin

More infos and example under https://docs.ultrastark.ch/docs/en/projects/us-mixin/description/

**This repository is a beta version an may change in the future**

## 1.0.0 Release
**Attention**
* **us-mixin/mixin** doesn't need colors anymore (the `color()` have been remove in favor of the global variable (ex: `var(--primary)`)
* A lot of default variables have been added to the us-mixin colors look [here](https://docs.ultrastark.ch/docs/projects/us-mixin/classes/color) form more informations

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
- `us-mixin/mixin` have to be imported in every scss file that needs they mixins
- us-mixin/utilities should be imported **only once**. If not, it's gonna create useless classes
- mixin and utilities work good together but you could only use one of the both if you need it

**Attention**
If you use the `color mixin` and want custom color, you need another step: [wiki](https://github.com/ultrastark/us-mixin/wiki/color)


## Authors

- **Raphaël Balet** - _Initial work_ - [Ultrastark](https://ultrastark.ch)

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details
