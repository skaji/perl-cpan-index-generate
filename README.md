# perl-cpan-index-generate

Generate CPAN index files

# Install

```console
❯ cpm install -g https://github.com/skaji/perl-cpan-index-generate.git
```

# Usage

```console
❯ cpm install LWP
...
DONE install libwww-perl-6.77 (using prebuilt)
18 distributions installed.

❯ perl-cpan-index-generate ./local/lib/perl5 | tee index.txt
# This file was generated by perl-cpan-index-generate.

Clone 0.47 A/AT/ATOOMIC/Clone-0.47.tar.gz
Date::Format 2.24 A/AT/ATOOMIC/TimeDate-2.33.tar.gz
Date::Format::Generic 2.24 A/AT/ATOOMIC/TimeDate-2.33.tar.gz
Date::Language 1.10 A/AT/ATOOMIC/TimeDate-2.33.tar.gz
...
```

You can use `index.txt` with cpm:

```console
❯ cpm install --resolver 02packages,file://index.txt,https://cpan.metacpan.org LWP
```
