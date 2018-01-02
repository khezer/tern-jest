# tern-jest

[tern-jest](https://github.com/khezer/tern-jest) is a plugin which adds support for [Jest](http://facebook.github.io/jest) to the JavaScript code intelligence system [Tern](http://ternjs.net/).

## Installation

tern-jest works with the NodeJS [Tern Server](http://ternjs.net/doc/manual.html#server), and within a browser.
After installing Tern according the setup instructions of your desired [editor plugin](http://ternjs.net/doc/manual.html#editor),
go to the place where the [Tern package](https://www.npmjs.org/package/tern) was
installed (or the [Tern repo](https://github.com/ternjs/tern) was cloned) and run

```
$ npm install tern-jest
```
```
$ yarn add tern-jest
```
Or, if you're not sure where Tern was installed, you can try
```
$ npm install -g tern-jest
```
```
$ yarn global add tern-jest
```

## Configuration

In order for Tern to load the tern-jest plugin once it is installed, you must
include `jest` in the `plugins` section of your [Tern configuration file](http://ternjs.net/doc/manual.html#configuration).
The configuration file can be either a file named `.tern-project` in your
project's root directory, or `.tern-config` in your home directory.


```json
{
  "plugins": {
    "jest": {}
  }
}
```
