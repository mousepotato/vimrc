<<<<<<< HEAD
# vim-go

Go (golang) support for Vim, which comes with pre-defined sensible settings (like
auto gofmt on save), with autocomplete, snippet support, improved syntax
highlighting, go toolchain commands, and more.  If needed vim-go installs all
necessary binaries for providing seamless Vim integration with current
commands. It's highly customizable and each individual feature can be
disabled/enabled easily.

![vim-go](https://dl.dropboxusercontent.com/u/174404/vim-go-2.png)
=======
# vim-go [![Build Status](http://img.shields.io/travis/fatih/vim-go.svg?style=flat-square)](https://travis-ci.org/fatih/vim-go)

<p align="center">
  <img style="float: right;" src="assets/vim-go.png" alt="Vim-go logo"/>
</p>
>>>>>>> amix_vimrc/master

## Features

This plugin adds Go language support for Vim, with the following main features:

* Build with `:GoBuild`, install with `:GoInstall` or test
  with `:GoTest` (run single tests via `:GoTestFunc`)
* Show test coverage with `:GoCoverage` or in browser with `:GoCoverageBrowser` 
* Goto definition with `:GoDef`
* Quick jump to declarations with `:GoDecls` or `:GoDeclsDir`
* Show documentation with `:GoDoc` inside or in browser with `:GoDocBrowser`
* Quickly execute your current file/files with `:GoRun`
<<<<<<< HEAD
* Automatic `GOPATH` detection based on the directory structure (i.e. `gb`
  projects, `godep` vendored projects)
* Change or display `GOPATH` with `:GoPath`
* Create a coverage profile and display annotated source code to see which
  functions are covered with `:GoCoverage`
* Call `gometalinter` with `:GoMetaLinter`, which invokes all possible linters
  (golint, vet, errcheck, deadcode, etc..) and shows the warnings/errors
* Lint your code with `:GoLint`
* Run your code through `:GoVet` to catch static errors
* Advanced source analysis tools utilizing oracle, such as `:GoImplements`,
  `:GoCallees`, and `:GoReferrers`
* Precise type-safe renaming of identifiers with `:GoRename`
* List all source files and dependencies
* Unchecked error checking with `:GoErrCheck`
* Integrated and improved snippets, supporting `ultisnips` or `neosnippet`
* Share your current code to [play.golang.org](http://play.golang.org) with `:GoPlay`
* On-the-fly type information about the word under the cursor. Plug it into
  your custom vim function.
* Go asm formatting on save
* Tagbar support to show tags of the source code in a sidebar with `gotags`
* Custom vim text objects such as `a function` or `inner function`
  list.
* Jump to function or type declarations with `:GoDecls` or `:GoDeclsDir`
* A async launcher for the go command is implemented for Neovim, fully async
  building and testing (beta).
* Integrated with the Neovim terminal, launch `:GoRun` and other go commands
  in their own new terminal. (beta)
* Alternate between implementation and test code with `:GoAlternate`

## Donation

People have asked for this for a long time, now you can be a fully supporter by [being a patron](https://www.patreon.com/fatih)! This is fully optional and is just a way to support vim-go's ongoing development directly. Thanks!
=======
* Advanced source analysis tools utilizing guru, such as `:GoImplements`,
  `:GoCallees`, and `:GoReferrers`
* Change or display `GOPATH` with `:GoPath`
* Multiple 3rd linter support with `:GoMetaLinter`
* Renaming identifiers with `:GoRename`
* Share your code to [play.golang.org](http://play.golang.org) with `:GoPlay`
* Switch between `*.go` and `*_test.go` code with `:GoAlternate`
* Add/Remove tags on struct fields with `:GoAddTags`
* Add import paths via `:GoImport` or remove them with `:GoDrop`
* Custom vim text objects such as `a function (af)` or `inner function (if)`
* ... and many more! Please see [doc/vim-go.txt](doc/vim-go.txt) for more information.
>>>>>>> amix_vimrc/master


## Install

Master branch is a **development** branch. Please use with caution.
I recommend to use the [**latest stable release**](https://github.com/fatih/vim-go/releases/latest)

Vim-go follows the standard runtime path structure. Below are some helper lines
for popular package managers:

*  [Pathogen](https://github.com/tpope/vim-pathogen)
    * `git clone https://github.com/fatih/vim-go.git ~/.vim/bundle/vim-go`
*  [vim-plug](https://github.com/junegunn/vim-plug)
    * `Plug 'fatih/vim-go'`
*  [Vim packages](http://vimhelp.appspot.com/repeat.txt.html#packages)
    * `git clone https://github.com/fatih/vim-go.git ~/.vim/pack/plugins/start/vim-go`

After installing, please install all necessary binaries. We have a handy
command for it:

```
:GoInstallBinaries
```

for more information please check out the [documentation](doc/vim-go.txt)

## Usage

Official documentation can be found under [doc/vim-go.txt](doc/vim-go.txt). You can display it from within Vim with:

```
:help vim-go
```

Depending on your installation, you may have to generate the plugin's [help
tags](https://github.com/vim/vim/blob/v8.0.0711/runtime/doc/helphelp.txt#L206-L227)
manually (eg. `:helptags ALL`).

We also have an [official vim-go
tutorial](https://github.com/fatih/vim-go-tutorial).

## License

The BSD 3-Clause License - see [`LICENSE`](LICENSE) for more details
