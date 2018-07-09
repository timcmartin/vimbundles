# Vimbundles

These are the bundles that I am currently using.
They are submodules of this repository.

## Getting Started

* Clone into ~/.vimbundles

== or ==

* Clone and symlink ~/.vimbundles to your cloned location
* Use updatesubs alias to update submodules

```sh
git clone https://github.com/timcmartin/vimbundles.git .vimbundles
cd ~/.vimbundles
git submodule init
git submodule foreach --recursive git fetch
```

## To Add More Submodules

```sh
cd ~/.vimbundles
git submodule add github_address_of_submodule
```

## Change the Remote of a Submodule
1. Update .gitmodules and .git/config addresses.

```sh
git submodule sync --recursive
```

`git submodule sync --recursive`
