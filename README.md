# contemporary_perl
Notes on contemporary Perl.

Things should be in Perl:
1. A style guide
2. Doctests
3. Exceptions
4. MRO (it is there)
5. Iterators (first pp, then XS)

# A style guide

- mandatory uses and pragmas

use 5.014;
use strict;
use warnings;
use Data::Dumper 'Dumper'

- you should code in subs
- every sub should be max 100 characters wide and no more than 40 rows
- longer subs should be refactored to represent their structure: by means of class hierarchy, or closures, or other
- regular expressions should be avoided
- for testing subs use doctests

throw Exception(message => "This shouldn't happen")
