# SCSS

For our scss we follow [Bootstrap's SCSS Linter](https://raw.githubusercontent.com/twbs/bootstrap/v4-dev/scss/.scsslint.yml) but make our own modifications since we use tabs, ids, the `!important` rule and a few others.

Our scss linter is [found here](http://gitlab.ahead4.com/ahead4/coding-standards/blob/master/scss/.scss-lint.yml), you'll want to copy this to the root of the scss folder in your project.

## Installing a linter

### Pre-req

You'll want to make sure you have Ruby (Try `ruby -v` in your terminal). If you don't have a response install Ruby and once you've confirmed it's installed run `gem update --system && gem install scss-lint` to install the gem.

### Atom

For atom you'll want to install the [atom linter](https://atom.io/packages/linter) `apm install linter` & the [linter for scss](https://atom.io/packages/linter-scss-lint) `apm install linter-scss-lint`. Once that's installed you'll need to enter the path to the `scss-lint` executable in the settings. You can find this by running `which scss-lint` in your terminal. Once that's all set up upon saving a scss file it should lint it and provide feedback.

### Sublime

*soon*
