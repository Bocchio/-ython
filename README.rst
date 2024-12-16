λython
======

What's this?
------------

A Python fork that adds ``λ`` as an additional keyword that works in the exact same way ``lambda`` does.

Why?
----

Because reading and typing ``lambda`` is just too much work.

Why is the repo named ``-ython`` instead of ``λython``?
----

GitHub doesn't like non-ASCII names :(

Steps
-----

Before compiling, you can run::


    make regen-keyword && make regen-pegen


to ensure ``Lib/keywords.py`` and ``Parser/parser.c`` are properly generated.

Then you can compile as usual.

Please refer to the `cpython <https://github.com/python/cpython>`_ repo for any additional details.

What to try
-----------

Now you can write things like::

    f = λ a: a('hello')
    f(print)
