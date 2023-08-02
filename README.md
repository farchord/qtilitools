# Qtilitools

Scripts/commands used in the Qtilities organization.

- **qtls-translate**: shell script based on `lxqt-transupdate` plus some additions
  to update and compile translations.

- **AppStream.cmake**: converts a given string to a freedesktop'
  desktop entry specification compliant name.

- **QtAppResources.cmake**: configures and installs various application' resources,
  including translations.

- **Translate.cmake**: modified version of `LXQtTranslateTs.cmake` merged with
  `LXQtTranslateDesktop.cmake`, to work also with Qt6.

- **TranslateDesktop.pl**: Renamed `LXQtTranslateDesktopYaml.pl`
  used by `Translate.cmake`.

## Build

```bash
cmake -B build -D CMAKE_BUILD_TYPE=None -D CMAKE_INSTALL_PREFIX=/usr -W no-dev
DESTDIR="$(pwd)/package" cmake --install build
```

## Packages

[![Packages]](https://repology.org/project/qtilitools/versions)


[Packages]: https://repology.org/badge/vertical-allrepos/qtilitools.svg
