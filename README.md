# us-mixin

More infos and example under https://docs.ultrastark.ch/docs/projects/us-mixin/description

**This repository is a beta version an may change in the future**

## 3.0.0 Release
**Removed feature**
The `Color()` mixin have been removed, in favor of the global variable.

**New feature**
* **$us-color-darkMode** together with **$isUsingDarkTheme: true;** let us set the new `--darkMode` or `--changeable` colors

### Example
`--darkMode-light` will set, when the user use dark mode, this color.   
To be used as follow -> `background-color: var(--darkMode-dark, var(--light));`  
Here, the color will be dark when the user us a dark mode.

`--changeable-light` will change automatically the color when turning into dark mode.  
To be used as follow -> `background-color: var(var(--changeable-light));`  
Here, the color will be the declared light from `$us-color-darkMode` on dark mode, and `$us-color-settings` on light mode.

`$us-color-darkMode` works the same as `$us-color-settings`

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

- **Raphaël Balet** - _Initial work_ - [Megaphone](https://megaphone.info)

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details
