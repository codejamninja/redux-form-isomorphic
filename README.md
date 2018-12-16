# redux-form-isomorphic

[![GitHub stars](https://img.shields.io/github/stars/codejamninja/redux-form-isomorphic.svg?style=social&label=Stars)](https://github.com/codejamninja/redux-form-isomorphic)

> handle early input to isomorphically rendered forms

Please ★ this repo if you found it useful ★ ★ ★


## Features

* hydrate form inputs collected before client payload loads
* compatible with redux-form


## Installation

```sh
npm install --save redux-form-isomorphic
```


## Dependencies

* [NodeJS](https://nodejs.org)
* [redux-form](https://redux-form.com)


## Usage

Run the following code BEFORE the initial client render

```js

class App extends Component {
  componentWillMount() {
    const isomorphicForm = new IsomorphicForm(this.context.store, {
      login: ['username', 'password']
    });
    isomorphicForm.rehydrate();
  }
}
```


## Support

Submit an [issue](https://github.com/codejamninja/redux-form-isomorphic/issues/new)


## Screenshots

[Contribute](https://github.com/codejamninja/redux-form-isomorphic/blob/master/CONTRIBUTING.md) a screenshot


## Contributing

Review the [guidelines for contributing](https://github.com/codejamninja/redux-form-isomorphic/blob/master/CONTRIBUTING.md)


## License

[MIT License](https://github.com/codejamninja/redux-form-isomorphic/blob/master/LICENSE)

[Jam Risser](https://codejam.ninja) © 2018


## Changelog

Review the [changelog](https://github.com/codejamninja/redux-form-isomorphic/blob/master/CHANGELOG.md)


## Credits

* [Jam Risser](https://codejam.ninja) - Author


## Support on Liberapay

A ridiculous amount of coffee ☕ ☕ ☕ was consumed in the process of building this project.

[Add some fuel](https://liberapay.com/codejamninja/donate) if you'd like to keep me going!

[![Liberapay receiving](https://img.shields.io/liberapay/receives/codejamninja.svg?style=flat-square)](https://liberapay.com/codejamninja/donate)
[![Liberapay patrons](https://img.shields.io/liberapay/patrons/codejamninja.svg?style=flat-square)](https://liberapay.com/codejamninja/donate)
