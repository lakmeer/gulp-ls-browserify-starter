
# gulp-livescript-browserify Starter Project

It's quite hard to work out how to get Gulp to work
correctly with this setup, and I got sick of figuring it
out every time. Here's a starter project that sets you up
with a simple Connect server (with livereload built-in) to
serve your files, and a browserify module system all
running neatly in Livescript.


## Changes

- Switch transformer to `browserify-livescript` instead of `liveify`
- Source maps now supported all the way back to LS source code
- Update to Livescript 1.4
- Much nicer error output


## Usage

Grab, this repo, run `npm i`, start the server with
`gulp` and start modifying the files to begin. The repo
contains a tiny proof-of-concept program to build from.

By default the `gulp` command will start the Connect
server at `localhost:8080` and start a livereload server
to go with it on the default port. The connect livereload
plugin automatically injects the LR snippet onto your page
so it works automatically with LR browser plugins.

If you find that gulp-watch is rebuilding your JS file
twice for every time you save, and you're using vim, it
may be because vim sometimes touches files twice when
working with backups enabled. To stop it, set
`nowritebackup` in your vimrc.


## Todo

- Stylesheet compilation as well maybe?

