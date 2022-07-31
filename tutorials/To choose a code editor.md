# To choose a code editor  
There can be various choices on how to choose a text editor, and the ultimate preference is up to the developer. And here is a guide to help it.  
# Professional  
## Atom  
### Owner: Microsoft, formerly GitHub  
### Written in: JavaScript  
### License: MIT License
### Speed: Slow to Medium  
### Supported Programming Language Syntaxes (by default): 68  
### Projects: Yes  
### Multiple Tabs: Yes  
### Packages: ~12,500 written in JavaScript  
### Themes: ~3,000 written in JSON  
### Manage Packages and Themes: Packages, Themes and Install tabs in Settings View  
### UI: Graphical  
This is a cross platform code editor written in Electron which has a highly customisable user interface and is highly extensible and has a large community.  It has a huge set of features like Git and GitHub integration, snippets, autocomplete, markdown preview, settings GUI etc. coming inbuilt through preinstalled packages. Packages add a good amount of functionality, which adds a lot of features in it, like keybindings, linting, syntax, live server, tabbed terminal, color picker, formatting JavaScript, markdown to PDF etc. and themes add style to its user interface. Its user interface is good, with a classic menu layout with File, Edit, View, Selection, Find, Packages and Help menus and at the left a pane to manage project files. Ctrl-Shift-P opens command palette.  
### Note: Sadly such a good editor and all its packages will be archived on December 15 2022 in favour of Visual Studio Code, vscode.dev and GitHub Codespaces.  
## Visual Studio Code  
### Written in: TypeScript, JavaScript  
### Owner: Microsoft  
### License: Binaries: Microsoft Software License Terms for Microsoft Visual Studio Code (nonFOSS, but allows commercial development free of cost), Source: MIT License, VSCodium unofficial builds: MIT License, Visual Studio Marketplace Extensions: _as per the developer of the extension_, OpenVSX Unofficial Marketplace: EPL-2.0  
### Speed: Medium  
### Supported Programming Language Syntaxes (by default): 75  
### Projects: Yes  
### Multiple Tabs: Yes  
### Extensions: ~30,000 written in JavaScript and TypeScript  
### Manage Extensions: Extensions tab in left ribbon  
### UI: Graphical  
This is a cross platform code editor written in Electron which has a very customisable user interface and is very extensible (both comparable to but not as much as Atom) and has a large community (larger than Atom). It has many features like Git and GitHub Integration (less than Atom), tabbed terminal, autocomplete, settings GUI etc. coming inbuilt. Extensions add a good amount of functionality, which adds a lot of features in it, like keybindings, themes, linting, live server, intellisense, color picker, formatting code, building program, markdown preview, markdown to PDF etc. Its user interface is excellent with a styled menu layout with File, Edit, Selection, View, Go, Run, Terminal and Help menus and at the left a ribbon with options to manage extensions, project files, git repositories and editor settings. F1 key or Ctrl-Shift-P opens command palette.  
## Sublime Text  
### Written in: C++, Python (according to Wikipedia)  
### Owner: Sublime HQ Proprietary Ltd.  
### License: Trialware with unlimited trial (keep closing a popup every x saves)  
### Supported Programming Language Syntaxes (by default): 84  
### Speed: Fast  
### Projects: Yes  
### Multiple Tabs: Yes  
### Packages: ~2,500 written in Python as .sublime-package(zip), .sublime-theme(JSON), .sublime-color-scheme  
### Manage Packages: Package Control  
### UI: Graphical  
This is a cross platform code editor written in C++ and Python (according to Wikipedia, since no source available) which is extraordinarily fast for a graphical editor with great useful features and has a big community. Despite being proprietary, it is very extensible. Packages add a good amount of functionality, which adds a lot of features in it, like themes, color schemes, syntax, autocomplete, linting, live server, markdown support, formatting code, sidebar enhancements, color picker etc. The key bindings can be customised using a JSON file. its user interface is a fair one with a classic menu layout with File, Edit, Selection, Find, View, Goto, Tools, Project, Preferences and Help menus and at the left a pane to manage project files.  
## Vim  
### Written in: C  
### Owner: Bram Moolenaar  
### License: Vim License  
### Speed: Fast  
### Projects: NerdTree plugin  
### Multiple Tabs: Yes  
### Plugins: ~19,000 written in Vim script  
### Manage Plugins: vim-plug, pathogen, vundle etc. + \~/.vimrc  
### UI: Text based  
This is a cross platform code editor written in C, as an improved version of Vi editor that is backwards compatible with it. This is one reason why it is very extensible, even more than Atom. Plugins can be and are written for everything, from simple commandlets to git integration, code completion, color picker, formatting code, snippets, linting etc. It is built to be used with keyboard, although there is a graphical version of it called gVim.  
## Neovim  
### Written in: C  
### Owner: Thiago de Arruda  
### License: Neovim License  
### Speed: Fast  
### Projects: project.nvim plugin  
### Multiple Tabs: Yes  
### Plugins: written in Vim script and Lua, all (at least almost all) Vim plugins are compatible  
### Manage Plugins: (Vim script) same as Vim + \~/.config/nvim/init.vim (\~/AppData/Local/nvim/init.vim on Windows), (Lua) packer, paq-nvim, NvChad etc. + /.config/init.lua (\~/AppData/Local/nvim/init.lua on Windows)  
### UI: Text based  
This is a cross platform code editor written in C, as an improved version of Vim editor. It is almost backwards compatible with Vim, and is slowly growing. It is highly extensible, maybe even the most extensible code editor. Like Vim, it uses plugin managers, the most popular of which is vim-plug. It can do everything with the help of plugins, everything which other editors like Visual Studio Code and Atom can do. Neovim also ships with nvim-qt, which can be used as a replacement to modern terminals for neovim.  
## Micro  
### Written in: Go  
### Owner: Zachary Yedidia  
### License: MIT License, Go License (Go), Apache License 2.0 (gdamore/encoding, zyedidia/tcell), BSD 3-clause (zyedidia/clipboard, golang/x), MPL (gopher-luar)  
### Speed: Fast  
### Projects: No  
### Multiple Tabs: Yes  
### Plugins: 30, written in Lua  
### UI: Text based  
Micro, written in Go, is an improvement over GNU Nano, which in turn is an improvement over Pico, a console based text editor.  
## GNU Emacs  
### Written in: C  
### Owner: GNU  
### License: GPLv3+  
### Speed: Medium to Fast  
### Projects: Via plugin  
### Multiple Tabs: Yes  
### Plugins: written in Emacs Lisp  
### Manage Plugins: For GnuELPA ESC+X (M-x) list-packages, others like MELPA, ELPA edit \~/.emacs.d/init.el (%HOME%/.emacs.d/init.el on Windows) (\~/.emacs or ~/.emacs.el or ~/.config/emacs/init.el can also be used) and then ESC+X (M-x) list-packages  
### UI: Text based and Graphical  
GNU Emacs is possibly the only popular editor in Emacs family being developed and used. Others like Gosling Emacs, XEmacs are no longer being developed. This editor is praised for being highly extensible. It also has a good user interface, and the command line and graphical ones resemble each other very much, with the same tabbed layout, the same command palette and the same options. The menu bar has options File, Edit, Options, Buffers, Tools and Help.  
## BlueFish  
### -----TODO-----
## Geany  
### -----TODO-----  
## Recommendation
### Graphical  
1. Visual Studio Code  
With all the appropriate extensions, which take the right advantage of its features like for programming, it can become almost an IDE of a programming language capable of intellisense, debugging, linting, building, prettifying and much more.  
2. Atom  
By far being possibly the most extensible graphical text editor (not command line text editor with(out) a GUI), with all the appropriate extensions, it can do almost everything Visual Studio Code can, maybe even more, except for maybe intellisense.  
3. Sublime Text  
Even though it is source unavailable proprietary, it is pretty extensible, and has a bunch of builtin features too, so it can do almost everything Atom and Visual Studio Code can do.
### Text based  
1. Neovim  
2. Emacs  
3. Vim
# Simple  
## Gedit  
### Written in: C  
### Owner: GNU  
### License: GPLv2+  
### Supported Programming Language Syntaxes (by default): 143  
### Projects: No  
### Multiple Tabs: Yes
### Plugins: 11  
### UI: Graphical  
This is a code editor for Linux and MacOS (and optionally for Windows through MSYS2) written in GTK 3 and is simple yet powerful. It has only 11 plugins bundled though. But they all provide basic important features like Python console, snippets, document statistics etc. And a customised style can also be added. Because of the GTK, it has a excellent user interface, with "New Window", "Quick Open...", "Save As...", "Save All", "Find...", "Find and Replace...", "Clear Highlight", "Go to Line...", "View", "Tools", "Preferences", "Keyboard Shortcuts", "Help" and "About Text Editor" options in the GTK menu (and refresh, print and fullscreen) and other options for opening files, new tabs and saving files on the bar at the top.  
## Notepad++  
### Written in: C++  
### Owner: Don Ho  
### License: GPLv3+, GPLv2+ (until v7.9.2)  
### Supported Programming Language Syntaxes (by default): 72  
### Projects: No  
### Multiple Tabs: Yes  
### Plugins: ~105 written in C and C++ as .dll  
### UI: Graphical  
This is a code editor for Windows (and optionally for Linux through Wine) written in C++, and is simple yet powerful and very fast. There are very few plugins which are merely some dynamic link libraries. Others have to be installed as DLLs separately and manually added, which has to be done in the 64-bit version to get a community maintained color picker (there is no inbuilt). It has a simple classic user interface with a classic menu layout with File, Edit, Search, View, Encoding, Language, Settings, Tools, Macro, Run, Plugins, Window and ? tabs and below that some icon shortcuts to them.  
## Notepadqq  
### Written in: C++, JavaScript  
### Owner: Daniel di Sarli  
### License: GPLv3+  
### Supported Programming Language Syntaxes (by default): 100+  
### Multiple Tabs: Yes  
### Plugins: written in JavaScript  
### UI: Graphical  
This is an almost complete replacement to Notepad++ for Linux and MacOS, with slight changes. written in C++ and JavaScript.  
## GNU Nano  
### Written in: C  
### Owner: GNU  
### License: GPL  
### Speed: Fast  
### Projects: No  
### Multiple Tabs: No  
### Plugins: \~/.nanorc  
### UI: Text based  
GNU Nano, written in C, which in turn is an improvement over Pico, a console based text editor. But this editor seems to be somewhat buggy.  
## Brackets  
### -----TODO-----  
# Cloud  
## OnlineGDB  
### -----TODO-----  
## Code Anywhere  
### -----TODO-----  
## Replit  
### -----TODO-----  
## Codesandbox  
### -----TODO-----  
## vscode.dev  
### -----TODO-----  
# Recommended Set of Extensions (or Plugins or Packages)  
## Visual Studio Code  
1. C/C++ (C/C++ Intellisense, debugging and code browsing) (Microsoft)  
2. Rust (Rust for Visual Studio Code (powered by Rust Language Server/Rust Analyzer), Provides lints, code completion and navigation, formatting and more.) (THe Rust Programming Language)  
3. Rust Syntax (Improved Rust syntax highlighting) (Dusty Pomerleau)  
4. Markdown PDF (Convert Markdown to PDF) (yzane)  
5. Markdown Preview GitHub Styling (Changes VSCode's built-in markdown preview to match GitHub's style) (Matt Bierner)  
6. Live Server Preview (Preview your HTML file with localhost server live-reloading enabled) (negokaz)  
7. IntelliCode (AI-assisted development) (Microsoft)  
8. HTML CSS Support (CSS Intellisense for HTML) (ecrnel)  
9. VS Color Picker (A tiny & smart color picker for web developer.) (lihui)
10. Code Runner (Run C, C++, Java, JS, PHP, Python, Perl, Ruby, Go, Lua, Groovy, PowerShell, CMD, BASH, F#, C#, VBScript, TypeScript, CoffeeScript, Scala, Swift, Julia, Crystal, OCaml, R, AppleScript, Elixir, VB.NET, Clojure, Haxe, Obj-C, Rust, Racket, Scheme, AutoHotkey, AutoIt, Kotlin, Dart, Pascal, Haskell, Nim) (Jun Han)  
11. Pylance (A performant, feature-rich language server for Python in VS Code) (Microsoft)  
12. Python (Intellisense (Pylance), Linting, Debugging (multi-threaded, remote), Jupyter Notebooks, code formatting, refactoring, unit tests and more.) (Microsoft)  
## Atom  
1. language-cpp14 (C++14 language support including new keywords, raw strings, digit separators, and binary literals) (jbw3)  
2. markdown-to-pdf (Atom package that converts markdown files to pdf) (jooola)  
3. linter (A Base Linter with Cow Powers) (steelbrain)  
4. linter-ui-default (Default UI for the Linter package) (steelbrain)  
5. intentions (Base package for showing intentions in Atom) (steelbrain)  
6. terminal-tab-fork (A simple terminal for panes and docks. Forked from terminal-tab) (bernd1995)  
7. atom-live-server (Launch a http server with live reload capability) (jas-chen)  
8. atom-path-intellisense (Path intellisense support for Atom) (apercova)  
9. color-picker (Right click or press CMD-SHIFT-C/CTRL-ALT-C to open it.) (thomaslindstrom)  
10. linter-python (Linter for python files. Lint operation based on pylama application.) (pchomik)  
11. busy-signal (A package that provides an easy to use API to show your package is performing a task) (steelbrain)  
