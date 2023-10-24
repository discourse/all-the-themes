# All the themes

A meta repository with links to every Discourse theme and theme component that kind of works and that we know about.

### Why this repo exists?

Occasionally we need to deprecate extensibility interfaces or migrate to newer and better patterns. We use this meta repository to search through all themes/components when doing such work.

### Getting started with the meta repo

```
git clone https://github.com/discourse/all-the-themes.git
cd all-the-themes
./reset-all-repos
```

### Contributing your own theme

If you have a theme you would like included in the meta repo create a PR to add the repository to third-party.txt

Also, please make sure you publish your theme at https://meta.discourse.org/c/theme

### Updating

To update your local copies of themes, run `./reset-all-repos`. The default branch of each repo will be checked out, reset to the latest commit on the origin, and all
local changes will be discarded. Any stale directories will be deleted.

If you want a totally clean slate, `rm -rf ./third-party ./official`, and then run `./reset-all-repos` again.

### Removing a theme

Delete the line from `third-party.txt` and commit your changes. To remove from your locally cloned repos, use `./reset-all-repos`.

### Update from meta script

At the root of the repo we have the `update_from_meta.rb` script, this can be used to pull all the github repos in the #theme category at https://meta.discourse.org/c/theme.

### See also

https://github.com/discourse/all-the-plugins
