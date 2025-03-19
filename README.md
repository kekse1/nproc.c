<img src="https://kekse.biz/github.php?draw&override=github:nproc.c" />

# `nproc`
This tool is one of the [coreutils](https://www.gnu.org/software/coreutils/)
which outputs the amount of available processor cores/threads.

Once I had to deal with the 'Raptor Lake' bug of Intel processors,
which caused **segmentation faults** ('Speicherzugriffsfehler') when
I compiled some projects (with the [`gcc`](https://gcc.gnu.org/)).

I didn't find out how to adapt the core/thread count (this was a thing
of the `apt` util, **not** the regular `MAKEFLAGS` or so), and I already
knew the compilation worked with less cores/threads, so I implemented
this tiny helper (for my purposes).

## Description
Either it'll print out the real core/thread count as usual, or it can
also print a value you select for yourself by setting the **`NPROC`**
environment variable to your needs.

Unset this variable in your environment to see the original/real
values again. If value is lower than 1, it'll fallback to the
real ones. That's all.. :-)

### Implementation
I choosed regular **ANSI C** as programming language.

## Download
* [`nproc.c`](src/nproc.c) \[Version v**0.2.3**; updated **2025-03-19**\];

BTW., it was born **2024-04-15**.

# Contact
<img src="https://kekse.biz/github.php?override=github:nproc.c&draw&text=nproc.c@kekse.biz&angle=6&size=38pt&fg=150,20,90&font=OpenSans&ro&readonly&h=64&v=16" />

# Copyright and License
The Copyright is [(c) Sebastian Kucharczyk](./COPYRIGHT.txt),
and it's licensed under the [MIT](./LICENSE.txt) (also known as 'X' or 'X11' license).

<a href="https://kekse.biz/">
<img src="favicon.png" alt="Favicon" />
</a>

