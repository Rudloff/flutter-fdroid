# flutter-froid

This is a script inspired by [gradlew-fdroid](https://github.com/f-droid/fdroidserver/blob/master/gradlew-fdroid)
that automatically detects and downloads the version of `flutter` required by a [Flutter](https://flutter.dev/) app.

It can be used in [fdroiddata](https://gitlab.com/fdroid/fdroiddata/) recipes
so we don't have to hardcode the Flutter version.

## Requirements

* [node-semver](https://github.com/npm/node-semver): in order to parse Flutter versions
* [yq](https://github.com/mikefarah/yq): in order to parse YAML files.
  (Without it, it will always default to the latest Flutter release.)

## How to use it

You can have a look at [this example recipe](examples/sterrenburg.github.flutterhole.yml).
