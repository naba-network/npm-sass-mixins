# Naba Network - SCSS-Mixins

## 1. Description

This project offers a bunch of easy to use and reusable cross browser scss mixins.

## 2 Dependencies

- [SCSS/SASS](https://sass-lang.com/)

## 3. How to install

### 3.1 Include it via npm

Install it via command line:

```
npm i @naba-network/scss-mixins
```

Or add it to your package.json manually:

```
"@naba-network/scss-mixins": "<VERSION>",
```

And run

```
npm install
```

### 3.2 Update version in your npm

Update the version in your package.json.

Then run:

```
npm update @naba-network/scss-mixins
```

## 4. Documentation

### How to include it

Once the package is installed you can include it in your SCSS files. As this is a set of mixins and functions this package will not increase your CSS file size so we recommend to include it in a very generic way like on top of your e.g. `_variables.scss` so you do not have to include it over and over again.

Simply add this line to include all mixins:

```
@import '~@naba-network/scss-mixins/scss/mixins';
```

If you only need the flexbox mixins:

```
@import '~@naba-network/scss-mixins/scss/flexbox-mixins';
```

### How to use it

Once the package is included you can use each mixin and function wherever and as often as you want. Simply add a mixin to your class like this:

```
.foo-bar {
    @include transition(all 0.25ms ease-in-out);
}
```

The code above will produce a cross browser valid css code like this:

```
.foo-bar {
    -webkit-transition: all 0.25ms ease-in-out;
    -moz-transition: all 0.25ms ease-in-out;
    -ms-transition: all 0.25ms ease-in-out;
    -o-transition: all 0.25ms ease-in-out;
    transition: all 0.25ms ease-in-out;
}
```
