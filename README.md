# TITLE

Inline::Guile

# SYNOPSIS

```
    use Inline::Guile;
    my $g = Inline::Guile.new();
    $g.run_i('(+ 3 5)');
    $g.run_s('"foo"');
```

# DESCRIPTION

Module for executing Guile code and accessing Guile libraries from Perl 6. 
Guile is a GNU implementation of the scheme language. See https://en.wikipedia.org/wiki/GNU_Guile.

# BUILDING

You will need guile and its headers installed, of course. The Debian packages
'guile-2.0' and 'guile-2.0-dev' contain all the binaries you shoudd need.

Guile itself links with its own libgc library, which is included in guile-2.0,
but I'm mentioning this in case it should become necessary to install this
separately.

```
    perl6 configure.pl6
    make test
    make install
```

# ACKNOWLEDGEMENTS

Heavily influenced by Inline::Python. Thanks, Stefan.

# AUTHOR

Jeffrey Goff <drforr@pobox.com>
