# All the themes

A meta repository with links to every Discourse theme and theme component that kind of works and that we know about.

### Why this repo exists?

Occasionally we need to deprecate extensibility interfaces or migrate to newer and better patterns. We use this meta repository to search through all themes/components when doing such work.

### Getting started with the meta repo

```
git clone https://github.com/discourse/all-the-themes.git
cd all-the-themes
git submodule update --init --recursive
```

### Contributing your own theme

If you have a theme you would like included in the meta repo create a PR with the new submodule.

To add it

```
git submodule add https://github.com/your-user/your-theme.git themes/your-theme
```

Ensure the submodule is cloned into the `themes` directory. Also, please make sure you publish your theme at:

https://meta.discourse.org/c/theme

### Updating a theme

Once in a while we will run

```
git submodule update --recursive --remote
```

If you would like to speed up our update process, submit a PR with updated submodules

### Update from meta script

At the root of the repo we have the `update_from_meta.rb` script, this can be used to pull all the github repos in the #theme category at https://meta.discourse.org/c/theme.

### See also

https://github.com/discourse/all-the-plugins
