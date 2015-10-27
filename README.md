# `compile`: functions module for [shellfire]

This module provides a simple set of wrapper functions for making it more pleasant to work with `make` and `gcc`.

## Compatibility

* Current `HEAD` is compatible with [shellfire] release [`release_2015.0117.1750-1`](https://github.com/shellfire-dev/shellfire/releases/tag/release_2015.0117.1750-1).

## Overview

Usage couldn't be simpler. Just pick a function. Please note that most functions are not currently documented.

## Importing

To import this module, add a git submodule to your repository. From the root of your git repository in the terminal, type:-

```bash
mkdir -p lib/shellfire
cd lib/shellfire
git submodule add "https://github.com/shellfire-dev/compile.git"
cd -
git submodule init --update
```

You may need to change the url `https://github.com/shellfire-dev/compile.git` above if using a fork.

You will also need to add paths - include the module [paths.d], and the dependencies [git] and [cpucount].


## Namespace `compile`

This namespace contains useful functions wrapping `compile`.

### To use in code

If calling from another [shellfire] module, add to your shell code the line
```bash
core_usesIn compile
```
in the global scope (ie outside of any functions). A good convention is to put it above any function that depends on functions in this module. If using it directly in a program, put this line _inside_ the `_program()` function:-

```bash
_program()
{
	core_usesIn compile
	…
}
```

### Functions

Not yet documented.


[swaddle]: https://github.com/raphaelcohn/swaddle "Swaddle homepage"
[shellfire]: https://github.com/shellfire-dev "shellfire homepage"
[core]: https://github.com/shellfire-dev/core "shellfire core module homepage"
[paths.d]: https://github.com/shellfire-dev/paths.d "paths.d shellfire module homepage"
[github api]: https://github.com/shellfire-dev/github "github shellfire module homepage"
[jsonwriter]: https://github.com/shellfire-dev/jsonwriter "jsonwriter shellfire module homepage"
[jsonreader]: https://github.com/shellfire-dev/jsonreader "jsonreader shellfire module homepage"
[urlencode]: https://github.com/shellfire-dev/urlencode "urlencode shellfire module homepage"
[unicode]: https://github.com/shellfire-dev/unicode "unicode shellfire module homepage"
[version]: https://github.com/shellfire-dev/version "version shellfire module homepage"
[git]: https://github.com/shellfire-dev/git "git shellfire module homepage"
[cpucount]: https://github.com/shellfire-dev/cpucount "cpucount shellfire module homepage"
[compile]: https://github.com/shellfire-dev/compile "compile shellfire module homepage"
