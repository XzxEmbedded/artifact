# Vim learning

## ctags
	ctags -R .

## Strip trailing whitespace
	:%s/\s\+$//e

	line tail space -> \s\+$
	line head space -> \s\+^

## Delete single or mutil words
	dw
	ndw: n is line number, eg. 3dw will delete 3 lines

## Delete or copy mutil lines
	dd: delete one line
	ndd: delete n lines

	yy: copy one line
	nyy: copy n lines

## Repeat operating
	.(point)

## Mode switch: Visual to Insert
	Visual/Visual block mode -> Insert mode: I(insert in front of cursor), A(append after cursor)

## The commandline window use history command
	q/ -> Open the commandline window with history of searches
	q: -> Open the commandline window with history of commands
	ctrl-f -> Switch from commandline mode to the commandline window(in terminal open other file)

	notes: You can move up and down through them with the k and j keys,
	       and when you press <enter> it executes the command underneath the cursor.

## Head line add the same strings
	1. ctrl-v enter visual block mode.
	2. j select modify blocks.
	3. input add strings
	4. input ESC key

## String replace
	:%s/string1/string2/
