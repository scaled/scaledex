# Scaled Package Directory

This project contains a directory of Scaled packages. The Scaled Package Manager checks out this
project and uses it to enable installation of packages by name and simple searching based on name
and description.

## `packages` file

The `packages` file contains a very simple index of all known packages of the format:

```
name source descrip
```

  * `name` must match `name` in your `packages.scaled` file (and contain no spaces)
  * `source` must match `source` in your `packages.scaled` file (and contain no spaces)
  * `descrip` can be any text you like, though the contents of `descrip` from your
    `packages.scaled` is probably just the ticket

## Adding your Scaled package

If you create a new Scaled package that you wish to have included in the directory, fork this
project, add your package to `packages` and submit a pull request. Ditto for updates or removals.

Note: if your package is used only as a dependency of other user-facing packages, there's no need to
add it to this directory. When a package is installed that depends on your package, your package
will automatically be installed. Only packages that users might need to search for by name or
description and manually install need be registered in the directory.
