# pmux
A poor man's terminal multiplexer

Usage:

    pmux <name>

This project is meant as a lightweight and simple alternative to gnu screen and
tmux, by managing a set of dtach or obduco sessions with a user experience that
is similar (although simpler) to screen or tmux.

When running within the kitty terminal emulator pmux can manage tabs for each
session, making for a better user experience. Start pmux with the --kitty option
update your kitty config file with the following:

	map ctrl+a>a		goto_tab -1
	map ctrl+a>ctrl+a	goto_tab -1
	map ctrl+a>.		launch --type overlay --copy-env ~/src/pmux/pmux --kitty-rename-tab

	map ctrl+a>c		launch --type overlay --copy-env ~/src/pmux/pmux --kitty-create-tab
	map ctrl+a>n		next_tab
	map ctrl+a>p		prev_tab

	map ctrl+a>0		goto_tab 1
	map ctrl+a>1		goto_tab 2
	map ctrl+a>2		goto_tab 3
	map ctrl+a>3		goto_tab 4
	map ctrl+a>4		goto_tab 5
	map ctrl+a>5		goto_tab 6
	map ctrl+a>6		goto_tab 7
	map ctrl+a>7		goto_tab 8
	map ctrl+a>8		goto_tab 9
	map ctrl+a>9		goto_tab 10

	map ctrl+a>shift+0	goto_tab 11
	map ctrl+a>shift+1	goto_tab 12
	map ctrl+a>shift+2	goto_tab 13
	map ctrl+a>shift+3	goto_tab 14
	map ctrl+a>shift+4	goto_tab 15
	map ctrl+a>shift+5	goto_tab 16
	map ctrl+a>shift+6	goto_tab 17
	map ctrl+a>shift+7	goto_tab 18
	map ctrl+a>shift+8	goto_tab 19
	map ctrl+a>shift+9	goto_tab 20

