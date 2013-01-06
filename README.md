
cninja
======

This is a perl wrapper script for ninja that will colorize its output without
turning off ninja's "smart terminal" features.

I'm an inexperienced perl user so this is probably crappy code but it seems to
work and I think the approach is promising.

How to use
----------

* Make sure `ninja` is in your path.
* Optionally, copy the `example_cninjarc.txt` to `~/.cninjarc` and edit.
* Call `cninja` just like you would call `ninja`.
* If you are using clang, call with the `--nogcc` option.

How it works
------------

`cninja` runs `ninja` in a pseudo terminal, parses the output with
copious regular expressions, and injects ascii color codes.

