# grep-write.kak

This plugin is designed as the "replace" part of kakoune's "find & replace" workflow.

Special thanks to [occivink][1] for creating [kakoune-find][2] where this was implemented. (I just changed and trimmed it to my preference)

(I now typically use [grug][6] since it handles large grep-buffers and a higher volume of files and changes better)

## Installation

### With [kak-bundle][3]

The recommended way to install **grep-write.kak** is to use [kak-bundle][3] plugin manager.

To install **grep-write.kak** with [kak-bundle][3] add this to your `kakrc`:

``` kak
bundle grep-write https://github.com/jtrv/grep-write.kak
```

### With [plug.kak][4]

To install **grep-write.kak** with [plug.kak][4] add this to your `kakrc`:
``` kak
plug "jtrv/grep-write.kak"
```

## Finding

Call the builtin [`grep`][5] command.

## Replacing

Write the edits you would like to make in the `*grep*` buffer. Then, call `grep-write` and the changes will be applied to their respective files.

Any lines that were not modified are simply ignored.

(Upon completion it reports the # of changes applied and ignored)

## License

Unlicense


[1]: https://github.com/occivink
[2]: https://github.com/occivink/kakoune-find
[3]: https://github.com/jdugan6240/kak-bundle
[4]: https://github.com/andreyorst/plug.kak
[5]: https://github.com/mawww/kakoune/blob/master/rc/tools/grep.kak
[6]: https://github.com/jtrv/grug
