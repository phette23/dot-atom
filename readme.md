# .atom

My configuration & customization for Atom.

# apm

On a new Atom instance, we can get all my packages—which might have corresponding settings in config.cson but not be installed—by running something like:

```sh
> # BASH
> for line in $(cat apm.txt); do apm install $line; done
> # FISH
> for line in (cat apm.txt); apm install $line; end
```

The list of packages in apm.txt may not be complete. To refresh the list, run:

```sh
> apm list -b --installed > apm.txt
```
