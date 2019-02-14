# Makefile functions

	Usage: $(<function> <arguments>) or ${<function> <arguments>}

	eg. $(subst a,b,$(x))

## subst: string replace

	$(subst <from>,<to>,<text>)

## patsubst: mode string replace

	$(patsubst <pattern>,<replacement>,<text>)

	eg. $(patsubst %.c,%.o,x.c bar.c), result: x.o bar.o

## strip: delete null characters including the starting and ending

	$(strip <string>)

## findstring: find string in other string

	$(findstring <find>,<in>)

## filer: reserve pattern strings

	$(filter <pattern...>,<text>)

## filter-out: reverse filer function

	$(filter-out <pattern...>,<text>)

## sort

	$(sort <list>)

## word

	$(word <n>,<text>)

	eg. $(word 2, foo bar baz) return 'bar'

## wordlist

	$(wordlist <s>,<e>,<text>)

	eg. $(wordlist 2, 3, foo bar baz) return 'bar baz'

## words: words count

	$(words <text>)

## firstword

	$(firstword <text>)
