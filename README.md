<!-- Repo notes -->
# scratchpad-playgrounds
Collection of prebuilt workspaces so you can *quickly* try out different languages and frameworks!

For right now, these will mostly be links to online pre-configured sandboxes, like *replit*, *Glitch*, etc.

I wanted to put this together because of the number of times when I've needed a temporary workspace just to test an idea or reproduce an issue from StackOverflow to help answer a question, and it has taken me longer than I would have liked to setup a test environment.

## Help make this better:
PRs are welcome! However, no *unnecessary* self-promotion, and for adding links, please strip off tracking parameters and keep clean.

## Future thoughts:
In the future, I think it would be neat if this repo contained actual subdirectories with a scaffolding system. So you could clone the repo, and then to scaffold a playground / workspace for any given language framework, all you would have to do is either run a top-level CLI command, like `setup nodejs`, or navigate to the directory and run `npm run init`. Something like that.

---

<!-- Actual start of content -->

## Collection Links
These are links to other *collections* of scratchpad scaffolding solutions.

Host | Link | Notes
--- | --- | ---
VS Code - CodeSwing | [Extension Link](https://marketplace.visualstudio.com/items?itemName=codespaces-Contrib.codeswing) | An extension for Visual Studio Code that essentially provides the functionality of a regular web playground (such as CodePen), but in a local environment. No messing with environment, tooling, or dependencies - just pick a template and get coding with live preview!
replit | [replit - Languages](https://replit.com/languages) | Create a repl based on language, framework, and more!
replit | [replit - Templates](https://replit.com/templates) | User-submitted templates
glitch | [glitch - hello worlds](https://glitch.com/@glitch/hello-worlds) | Various starter templates
glitch | [glitch - starters](https://glitch.com/create#:~:text=Starters) | Various starter templates
CodeSandbox | [New Sandbox](https://codesandbox.io/s/) | Start with a template
CodeSandbox | [Template repo](https://github.com/codesandbox/codesandbox-templates) | The official CodeSandbox repo for templates. You can use this, or ***any*** public repo as a template source!

Options that have been retired:

Name & Link | What | Date Retired
--- | --- | ---
[Katacoda](https://www.katacoda.com/learn#playgrounds) | Dozens of different playground types, including NodeJS, Dotnet, and more. | June 15th, 2022

---

## Languages

### Standard Web (***HTML*** + CSS + JS)
Platform & Link | Hosted | Notes
--- | --- | ---
[CodePen](https://codepen.io/pen/) | Online | NA
[JSFiddle](https://jsfiddle.net/) | Online | NA
[replit](https://replit.com/languages/html) | Online | NA
[CodeSandbox](https://codesandbox.io/s/github/codesandbox-app/static-template) | Online | NA

### JavaScript
Platform & Link | Hosted | Notes
--- | --- | ---
[replit](https://replit.com/languages/javascript) | Online | Executes with Node
[CodeSandbox](https://codesandbox.io/s/vanilla) | Online | Includes HTML
[StackBlitz](https://stackblitz.com/fork/js) | Online | Includes HTML, mixes NodeJS
[Chrome DevTools - Snippets](https://developers.google.com/web/tools/chrome-devtools/javascript/snippets) | Local | If you simply need to test a bit of JS, why not try using your web browser?! Chrome has support for "snippets", which are single file JS scratchpads which are saved and managed by the browser. Or you can always copy and paste into the browser console!
[Firefox DevTools - Scratchpad](https://developer.mozilla.org/en-US/docs/Tools/Scratchpad) | Local | ~~You can press Shift + F4 to bring up a temporary JS scratchpad!<br><br> > Warning: This will be deprecated soon.~~ This is now fully deprecated 😞

### JavaScript - NodeJS Flavored

> Quick disclaimer: A lot of online sandboxes will mix together NodeJS environments (think `__dirname`) and web environments (think `document.location`). For example, Glitch will allow you to add a package.json file and start using NodeJS packages with JS, while also mixing in static HTML + vanilla JS serving. The boundaries between the two systems are not always clearly defined...

Platform & Link | Hosted | Notes
--- | --- | ---
[replit](https://replit.com/languages/nodejs) | Online | NA
[CodeSandbox](https://codesandbox.io/s/node) | Online | NA
[StackBlitz](https://stackblitz.com/fork/js) | Online | This is really just their "JS" starter, but it uses NodeJS to execute
[Glitch](https://glitch.com/edit/#!/remix/hello-express) | Online | NA
[Runkit](https://npm.runkit.com) | Online | Limited, meant for testing a single NPM package at a time.

#### NodeJS - Quick Options
There are tons of ways you can quickly write and execute bits of JS with a locally installed version of NodeJS. I've written up a longer summary [in this post](https://joshuatz.com/posts/2019/nodejs-interacting-on-cmd-line-shell-without-creating-a-js-file/), but here are some bullet points:
 - REPL
	 - CLI: Type `node` and press enter to start REPL
	 - You can use `.editor` to write with line breaks and wait to execute until you are ready
 - Execute any JS file with Node
	 - CLI: `node {filepath}`
	 - Example: `echo console.log("hello!") > test.js && node test.js`
 - Eval with print
	 - CLI: `node -p "{javascriptAsString}"`
	 - Example: `node -p "Math.round(Math.random()*100)"`
 - Pipe non-js file to eval:
	 - CLI: `echo console.log("in txt file"); > test.txt && less -FX test.txt | node -p`
 - ... and many more methods!

### C++
Platform & Link | Hosted | Notes
--- | --- | ---
[replit](https://replit.com/languages/cpp) | Online | NA
[OnlineGDB](https://www.onlinegdb.com/online_c++_compiler) | Online | NA
[paiza.io](https://paiza.io/en/projects/new?language=cpp) | Online | NA
[RCRL](https://github.com/onqtam/rcrl) | Local | Cross-Platform
[Cling](https://root.cern.ch/cling) | Local | Unix

### Python
Platform & Link | Hosted | Notes
--- | --- | ---
[replit](https://replit.com/languages/python3) | Online | NA
[CodeSandbox](https://codesandbox.io/p/sandbox/python-starter-in2qez) | Online | NA
[python.org shell](https://www.python.org/shell/) | Online | REPL mode only
[OnlineGDB](https://www.onlinegdb.com/online_python_compiler) | Online | NA
[paiza.io](https://paiza.io/en/projects/new?language=python3) | Online | NA
[trinket.io](https://trinket.io/python) | Online | Shareable, multi-file support. Similar to Glitch.
CLI | Local | There are many options for executing bits of Python locally, similar to NodeJS, which I'll explore below.

#### Python - Quick Options
This is a really good writeup of quick local execution options - [from realpython.com](https://realpython.com/interacting-with-python/).

Here is an additional summary of some options:
 - Use the Python interpreter binary as a REPL
	 - Either launch the binary, or call it via the registered path.
		 - On Windows, this means either launching `python.exe`, or from the Command Prompt, type `python` and hit enter
		 - You can end a line with `\` or `;\` to start a multiline entry
 - Execute a file containing Python with the interpreter:
	 - `python {filename}`
	 - The file does not have to end in `.py` extension
 - Use *IDLE*, the slim editor/shell combo that ships with Python
	 - It usually comes bundled with the Python installer
	 - You can use it in shell mode (like REPL), or write actual files
 - Use built-in IDE tools or extensions:
	 - [VSCode](https://marketplace.visualstudio.com/items?itemName=ms-python.python)
	 - [Visual Studio](https://docs.microsoft.com/en-us/visualstudio/python/python-interactive-repl-in-visual-studio)

### TypeScript
Platform & Link | Hosted | Notes
--- | --- | ---
[typescriptlang.org/play](https://www.typescriptlang.org/play/) | Online | Instant TS -> JS transpile
[replit](https://replit.com/languages/typescript) | Online | Executes with Node
[CodeSandbox](https://codesandbox.io/s/vanilla-ts) | Online | Includes HTML
[StackBlitz](https://stackblitz.com/fork/typescript) | Online | NA

### Sass
Platform & Link | Hosted | Notes
--- | --- | ---
[SassMeister](https://www.sassmeister.com/) | Online | NA
[fiddlesalad](http://fiddlesalad.com/sass/) | Online | Lots of ui cruft.

---

## Frameworks
### UI Frameworks
#### React
Platform & Link | Notes
--- | ---
[replit](https://replit.com/@templates/Create-React-App) | JavaScript
[CodeSandbox](https://codesandbox.io/s/new) | JavaScript
[CodeSandbox](https://codesandbox.io/s/react-ts) | TypeScript
[StackBlitz](https://stackblitz.com/fork/react) | JavaScript
[glitch](https://glitch.com/edit/#!/remix/starter-react) | JavaScript

#### Vue
Platform & Link | Notes
--- | ---
[CodeSandbox](https://codesandbox.io/s/vue) | JavaScript
[CodeSandbox](https://github.com/codesandbox/codesandbox-templates/tree/master/packages/client/vue-typescript-template) | TypeScript - I think this needs fixes...

#### Svelte
Platform & Link | Notes
--- | ---
[Svelte Official Repl](https://svelte.dev/repl/hello-world) | Supports multi-file, saving, and sharing!
[CodeSandbox](https://codesandbox.io/s/svelte) | JavaScript

### CMS
#### Wordpress
```sh
cd playgrounds
docker-compose -f wordpress/docker-compose.yml up -d
```
 > Code directory will be auto-created in `playgrounds/wordpress/src`, which you can edit.
