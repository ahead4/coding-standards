# Linting PHP Files on Atom

For Atom you're going to want the Linter Plugin [found here](https://atom.io/packages/linter). Once Installed you'll want to grab phpcs if you don't already have it.

There are 2 ways to do this, you can either use the one included with this repo in the `bin/` folder or you can install it yourself. To install it yourself grab PHP & Pear and when they've been acquired (& Check they work using `which`) you'll want to grab PHP_CodeSniffer by running `pear install PHP_CodeSniffer` in your terminal (May need to add `sudo`). Now you can grab the linter-phpcs plugin [found here](https://atom.io/packages/linter-phpcs) and install that.

Lastly you'll want to edit the settings for the linter-phpcs. You can do this by either going to settings -> plugins and then editing the settings for the plugin changing the  Phpcs Executable Path to where you installed it above (Use `which phpcs` to find out where) & the Standard to point to the `phpcs-ruleset.xml` found in this folder. Otherwise you can edit your atom's config.cson file and editing the file to replace the linter-phpcs section like so:
```json
"linter-phpcs":
	phpcsExecutablePath: "[Path to phpcs]"
	standard: "[Path to phpcs-ruleset.xml]"
```
