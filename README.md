[Material design] components for [AngularDart]. Powering some of Google's most
sophisticated and mission-critical [applications].

The [AngularDart Components Gallery] contains live examples and documentation.

This productive and stable set of widgets, contributed to by hundreds of
Googlers, make debugging and deploying your app easier. Strict latency and
testing policies make these widgets an excellent fit for projects using the
Angular package.

[Material design]: https://material.io/guidelines
[AngularDart]: https://webdev.dartlang.org/angular
[applications]: https://news.dartlang.org/2016/03/the-new-adwords-ui-uses-dart-we-asked.html
[AngularDart Components Gallery]: https://dart-lang.github.io/angular_components_example/

This is a continually growing set of widgets. Recent additions include:

* Material Slider
* Material Datepicker
* Material Menu

At this time we are not taking pull requests, but please
[file an issue](https://github.com/dart-lang/angular_components/issues)
and we will work with you.

**Officially supported browsers:** The last two versions of Chrome, Edge,
Firefox, and Safari.

## Package `build_runner` support

As of angular: 5.0.0-alpha+5 the pub transformer has been removed in favor of
code generation through package [build]. To build your project with
[build_runner]:

1. Add two dev dependencies to your `pubspec.yaml` file:

  ```yaml
  dev_dependencies:
    build_runner: ^0.7.8
    build_web_compilers: ^0.2.1
  ```

2. Run `pub get` on your package.
3. Build your package:

  ```
  pub run build_runner build
  ```

  Or run a local development server with a file watcher and incremental
  rebuilds:

  ```
  pub run build_runner serve
  ```

[build_runner]: https://pub.dartlang.org/packages/build_runner
[build]: https://pub.dartlang.org/packages/build

## Useful links

* **[AngularDart Components Gallery](https://dart-lang.github.io/angular_components_example/)**
* AngularDart Components resources:
  * [About AngularDart Components](https://webdev.dartlang.org/components)
  * [Google I/O 2017 codelab](https://codelabs.developers.google.com/codelabs/your-first-angulardart-web-app)
  * [AngularDart Components launch codelab](https://webdev.dartlang.org/codelabs/angular_components)
  * [API reference](https://webdev.dartlang.org/components/api)
* AngularDart resources:
  * [AngularDart documentation](https://webdev.dartlang.org/angular/guide)
  * [angular pub package](https://pub.dartlang.org/packages/angular)
* [Material Design site](https://material.io)

## Required Icon Font

For icons to appear, add the following icon font download to your page.
[Example](https://github.com/dart-lang/angular_components_example/blob/ae323a593cbb5508fa6fbe33afb7f5d40ea96a7e/angular_gallery/lib/builder/template/index.html.mustache#L8)

```html
<link
  rel="stylesheet"
  type="text/css"
  href="https://fonts.googleapis.com/icon?family=Material+Icons">
```

## Custom component styles

The styles of these components can be customized in your project with a
component's provided [Sass mixins](http://sass-lang.com/guide#topic-6).

1. Add a dev dependency on the
[sass_builder](https://pub.dartlang.org/packages/sass_builder) package to your
`pubspec.yaml`:

  ```yaml
  dev_dependencies:
    sass_builder: ^1.2.0 # update for the latest version
  ```

2. Now you can import styles and mixins from this package via dart style package
imports in your Sass files.

  In your `.scss` files:

  ```scss
  @import 'package:angular_components/css/material/material';

  .blue {
    color: $mat-blue;
  }
  ```

## Project Roadmap

Our current work is summarized in the
[roadmap for this quarter](https://github.com/dart-lang/angular_components/issues/251).
