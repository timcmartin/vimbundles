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

git submodule foreach --recursive git pull

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

## Remove a Submodule
1. Remove from .gitmodules
2. Stage the change: `git add .gitmodules`
3. Delete from .git/config (~/Dotfiles/.git/modules/vimbundles/config)
4. `git rm --cached <path_to_submodule>`
5. From vimbundles dir: `rm -rf ../.git/modules/vimbundles/modules/<path_to_submodule>`
5. From vimbundles dir: `rm -rf <path_to_submodule>`
6. `git commit -m "Removed Submodule"`
7. Delete the now untracked submodule files: `rm -rf <path_to_submodule`

