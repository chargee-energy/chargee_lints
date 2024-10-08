[![pub package](https://img.shields.io/pub/v/chargee_lints.svg)](https://pub.dev/packages/chargee_lints)

This package contains a recommended set of lints for [Flutter] apps, packages,
and plugins created by Chargee.

This package is built on top of Flutter's `flutter.yaml` set of lints from
[package:flutter_lints].

Lints are surfaced by the [dart analyzer], which statically checks dart code.
[Dart-enabled IDEs] typically present the issues identified by the analyzer in
their UI. Alternatively, the analyzer can be invoked manually by running
`flutter analyze`.

## Usage

Flutter apps, packages, and plugins can use these lints by following
these instructions:

1. Depend on this package as a **dev_dependency** by running
   `flutter pub add dev:chargee_lints`.
2. Create an `analysis_options.yaml` file at the root of the package (alongside
   the `pubspec.yaml` file) and `include: package:chargee_lints/chargee.yaml`
   from it.

Example `analysis_options.yaml` file:

```yaml
# This file configures the analyzer, which statically analyzes Dart code to
# check for errors, warnings, and lints.
#
# The issues identified by the analyzer are surfaced in the UI of Dart-enabled
# IDEs (https://dart.dev/tools#ides-and-editors). The analyzer can also be
# invoked from the command line by running `flutter analyze`.

# The following line activates a set of recommended lints for Flutter apps,
# packages, and plugins designed to encourage good coding practices.
include: package:chargee_lints/chargee.yaml

linter:
  # The lint rules applied to this project can be customized in the
  # section below to disable rules from the `package:chargee_lints/chargee.yaml`
  # included above or to enable additional rules. A list of all available lints
  # and their documentation is published at https://dart.dev/tools/linter-rules.
  #
  # Instead of disabling a lint rule for the entire project in the
  # section below, it can also be suppressed for a single line of code
  # or a specific dart file by using the `// ignore: name_of_lint` and
  # `// ignore_for_file: name_of_lint` syntax on the line or in the file
  # producing the lint.
  rules:
    # avoid_print: false  # Uncomment to disable the `avoid_print` rule
    # prefer_single_quotes: true  # Uncomment to enable the `prefer_single_quotes` rule
# Additional information about this file can be found at
# https://dart.dev/tools/analysis
```
