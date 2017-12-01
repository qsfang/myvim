This project is abandoned. 

I'll add links to maintained forks here. Send me email (address listed on
GitHub profile page) or submit a PR with links to add.

# Go Explorer

Go Explorer is a Vim plugin for exploring Go code.

## GeDoc

The GeDoc command shows documentation for the package specified by `spec`. 

    :GeDoc spec 

If `spec` starts with '\', then `spec` is take as the name of a package
imported in the current file. Otherwise `spec` is taken as a package import
path. The GeDoc command supports command completion.

In the documentation viewer, use \<c-]> to jump to source code or
documentation.  If the identifier under the cursor is the name of a
declaration, then \<c-]> jumps to the source code for the declaration. If the
identifier under the cursor is a type, then \<c-]> jumps to the documentation
for the type. \<C-t> jumps back. Use \]] and \[\[ to move forward and back
through declarations in the documentation.

Documentation pages can be opened directly using the godoc:// prefix:

    :edit godoc://net/http

## Installation Instructions

To install this plugin with Pathogen, use:

     git clone https://github.com/garyburd/go-explorer.git ~/.vim/bundle/go-explorer

The plugin requires a Go helper program:

     go get github.com/garyburd/go-explorer/src/getool

The plugin and the getool program are tightly coupled. Update both at the
same time. 

## Other plugins

Go Explorer is compatible with [vim-go](https://github.com/fatih/vim-go).
