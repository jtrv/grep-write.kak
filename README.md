# kakoune-grep-write

This plugin is designed as the "replace" part of kakoune's "find & replace" workflow.

Special thanks to [occivink][1] for creating [kakoune-find][2] where this was implemented. (I just trimmed it to my preference)

## Installation

### With [plug.kak][3]

The recommended way to install **kakoune-write-grep** is to use [plug.kak][3] plugin manager.

To install **kakoune-write-grep** add this to the `kakrc`:

``` kak
plug "JacobTravers/kakoune-grep-write"
```

Then reload the configuration file or restart Kakoune and run `:plug-install`.

## Finding

Call the builtin [`grep`][4] command.

## Replacing

Write the edits you would like to make in the `*grep*` buffer. Then, call `grep-write` and the changes will be applied to their respective files.

Any lines that were not modified are simply ignored.

(Upon completion it reports the # of changes applied and ignored)

## License

Unlicense



[1]: https://github.com/occivink
[2]: https://github.com/occivink/kakoune-find
[3]: https://github.com/andreyorst/plug.kak
[4]: https://github.com/mawww/kakoune/blob/master/rc/tools/grep.kak
