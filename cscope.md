# Cscope

## Step 1

	if has("cscope")

		set csprg=/usr/bin/cscope

		set csto=0

		set cst

		set nocsverb

		" add any database in current directory

		if filereadable("cscope.out")

		    cs add cscope.out

		" else add database pointed to by environment

		elseif $CSCOPE_DB != ""

		    cs add $CSCOPE_DB

		endif

		set csverb

	endif

	Above messages write into /etc/vim/vimrc

## Step 2

	Runing command: cscope -Rbq

	Open file: vim file
