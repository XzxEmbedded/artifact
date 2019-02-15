# Makefile directory functions

	Usage: $(<function> <arguments>) or ${<function> <arguments>}

## dir

	$(dir <names...>)

	eg. $(dir src/foo.c hacks) return 'src/ ./'

## notdir

	$(notdir <names...>)

	eg. $(notdir src/foo.c hacks) return 'foo.c hacks'

## suffix

	$(suffix <names...>)

	eg. $(suffix src/foo.c src-1.0/bar.c hacks) return '.c .c'

## basename

	$(basename <names...>)

	eg. $(basename src/foo.c src-1.0/bar.c hacks) return 'src/foo src-1.0/bar hacks'

## addsuffix

	$(addsuffix <suffix>,<names...>)

	eg. $(addsuffix .c,foo bar) return 'foo.c bar.c'

## addprefix

	$(addprefix <prefix>,<names...>)

	eg. $(addprefix src/,foo bar) return 'src/foo src/bar'

## join

	$(join <list1>,<list2>)

	eg. $(join aaa bbb , 111 222 333) return 'aaa111 bbb222 333'
