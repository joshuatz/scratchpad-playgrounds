<!-- Repo notes -->
# scratchpad-playgrounds
Collection of prebuilt workspaces so you can *quickly* try out different languages and frameworks!

For right now, these will mostly be links to online pre-configured sandboxes, like *repl.it*, *Glitch*, etc.

I wanted to put this together because of the number of times when I've needed a temporary workspace just to test an idea or reproduce an issue from StackOverflow to help answer a question, and it has taken me longer than I would have liked to setup a test environment.

## Help make this better:
PRs are welcome! However, no *unnecessary* self-promotion, and for adding links, please strip off tracking parameters and keep clean.

## Future thoughts:
In the future, I think it would be neat if this repo contained actual subdirectories with a scaffolding system. So you could clone the repo, and then to scaffold a playground / workspace for any given language framework, all you would have to do is either run a top-level CLI command, like `setup nodejs`, or navigate to the directory and run `npm run init`. Something like that. Might require a lot of scripting for advanced workspaces, like a WordPress env for theme testing.

---

<!-- Actual start of content -->

# Master Links
These are links to other *collections* of scratchpad scaffolding solutions.

Host | Link | Notes
--- | --- | ---
repl.it | [repl.it - Languages](https://repl.it/languages) | Create a repl based on language, framework, and more!
repl.it | [repl.it - Templates](https://repl.it/templates) | User-submitted templates
glitch | [glitch - hello worlds](https://glitch.com/@glitch/hello-worlds) | Various starter templates
CodeSandbox | [New Sandbox](https://codesandbox.io/s/) | Start with a template
CodeSandbox | [Template repo](https://github.com/codesandbox/codesandbox-templates) | The official CodeSandbox repo for templates. You can use this, or ***any*** public repo as a template source!


# Languages

## Standard Web (***HTML*** + CSS + JS)
Platform & Link | Hosted | Notes
--- | --- | ---
[CodePen](https://codepen.io/pen/) | Online | NA
[JSFiddle](https://jsfiddle.net/) | Online | NA
[repl.it](https://repl.it/languages/html) | Online | NA
[CodeSandbox](https://codesandbox.io/s/github/codesandbox-app/static-template) | Online | NA

## JavaScript
Platform & Link | Hosted | Notes
--- | --- | ---
[repl.it](https://repl.it/languages/javascript) | Online | Executes with Node
[CodeSandbox](https://codesandbox.io/s/vanilla) | Online | Includes HTML
[Chrome DevTools - Snippets](https://developers.google.com/web/tools/chrome-devtools/javascript/snippets) | Local | If you simply need to test a bit of JS, why not try using your web browser?! Chrome has support for "snippets", which are single file JS scratchpads which are saved and managed by the browser. Or you can always copy and paste into the browser console!
[Firefox DevTools - Scratchpad](https://developer.mozilla.org/en-US/docs/Tools/Scratchpad) | Local | You can press Shift + F4 to bring up a temporary JS scratchpad!<br><br> > Warning: This will be deprecated soon.

## JavaScript - NodeJS Flavored
Platform & Link | Hosted | Notes
--- | --- | ---
CLI | Local | There are multiple ways you can quickly test JS, or NodeJS flavored JS, locally and with a standard NodeJS install.<br><br>See "NodeJS - Quick Options" below.

### NodeJS - Quick Options
There are tons of ways you can quickly write and execute bits of JS with a locally installed version of NodeJS. I've written up a longer summary [in this post](https://joshuatz.com/posts/2019/nodejs-interacting-on-cmd-line-shell-without-creating-a-js-file/), but here are some bullet points:
 - REPL
	 - CLI: Type `node` and press enter to start REPL
	 - You can use `.editor` to write with line breaks and wait to execute until you are ready
 - Excute any JS file with Node
	 - CLI: `node {filepath}`
	 - Example: `echo console.log("hello!") > test.js && node test.js`
 - Eval with print
	 - CLI: `node -p "{javascriptAsString}"`
	 - Example: `node -p "Math.round(Math.random()*100)"`
 - Pipe non-js file to eval:
	 - CLI: `echo console.log("in txt file"); > test.txt && less -FX test.txt | node -p`
 - ... and many more methods!

## TypeScript
Platform & Link | Hosted | Notes
--- | --- | ---
[typescriptlang.org/play](https://www.typescriptlang.org/play/) | Online | Instance TS -> JS transpile
[repl.it](https://repl.it/languages/typescript) | Online | Executes with Node
[CodeSandbox](https://codesandbox.io/s/vanilla-ts) | Online | Includes HTML
[StackBlitz](https://stackblitz.com/fork/typescript) | Online | NA

## Sass
Platform & Link | Hosted | Notes
--- | --- | ---
[SassMeister](https://www.sassmeister.com/) | Online | NA
[fiddlesalad](http://fiddlesalad.com/sass/) | Online | Lots of ui cruft.

# Frameworks

## UI Frameworks

### React
Platform & Link | Notes
--- | ---
[repl.it](https://repl.it/languages/reactjs) | JS
[repl.it](https://repl.it/languages/reactts) | TS
[CodeSandbox](https://codesandbox.io/s/new) | JS
[CodeSandbox](https://codesandbox.io/s/react-ts) | TS
[StackBlitz](https://stackblitz.com/fork/react) | JS

### Vue
Platform & Link | Notes
--- | ---
[CodeSandbox](https://codesandbox.io/s/vue) | JS
[CodeSandbox](https://github.com/codesandbox/codesandbox-templates/tree/master/packages/client/vue-typescript-template) | TS - I think this needs fixes...