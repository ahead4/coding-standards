# Javascript

Generally we follow [Airbnb's Coding Standards](https://github.com/airbnb/javascript) with the exception of using tabs instead of spaces. We use tabs and set the spacings to be 4.

I have attached our [.jscsrc](.jshrc) which you can put in the root of your project (if it's not already there) which should get picked up by the linter in your text editor.

## Installing a linter

### Atom

If you're using the atom shell commands then you can run `apm install linter` and then `apm install linter-jscs` to get installed.

If you haven't got it installed then just browse the community packages for `Linter` and after that's installed `Linter-JSCS`.

It should activate straight away or you might need to do a quick restart.

#### Resources
- https://atom.io/packages/linter
- https://atom.io/packages/linter-jscs

### Sublime

To install the linter you'll need Sublime Text 3 and Package Control installed. Once you have all of that open the command palette (`ctrl+shift+p` on windows), type Install and click the `Package Control: Install Package` option and install SublimeLinter. Once it's finished, restart sublime.

Next grab Node/io.js if you don't already have one of them and run `npm install -g jscs` in your terminal. Run `jscs` to check if it works and then go through the steps over at: http://sublimelinter.readthedocs.org/en/latest/troubleshooting.html#finding-a-linter-executable to make it available to sublime.

Back in sublime you can now install `SublimeLinter-jscs` like you did with the SublimeLinter earlier.

Now you should be able to see you're JS being linted.

#### Resources
- http://sublimelinter.readthedocs.org/en/latest
- https://packagecontrol.io/packages/SublimeLinter
- https://packagecontrol.io/packages/SublimeLinter-jscs
