# VIM

## Moving the cursor

```h```                        :    key to move left
```j```                        :    key to scroll down
```k```                        :    key to scroll up
```l```                        :    key to move right

```nvim FILENAME```            :    start vim from the shell
```<Esc>```                    :    return to Normal mode

## Exiting vIM

```:q!```                      :    this exits the editor, discarding any changes you have made
```:q```                       :    close this window

## Text editing -deletion

```x```                        :    to delete the character under the cursor

## Text editing insertion

```i```                        :    insert before the cursor

## Text editing appending

```a```                        :    append after the cursor
```A```                        :    append after the line

## Editing a file

```:wq```                      :    to save a file, text and exit

## Deletion command

```dw```                       :    delete a word

## More deletion commands

```d$```                       :    delete to the end of the line

## On operators and motions

```de```                       :    will delete grom the cursor to the end of the word

## Using a count for a motions

```2w```                       :    move the cursor two words forward
```3e```                       :    move the cursor to the end of the third word forward
```0```                        :    move to the start of the line

## Using a count to delete more

```d2w```                      :    delete the two UPPER CASE words

## Operating on lines

```dd```                       :    delete a whole line
```2dd```                      :    delete two lines

## The undo command

```u```                        :    undo the last commands
```U```                        :    fix a whole line
```<C-r>```                    :    few times to redo the commands (undo the undos)

## The put command

```p```                        :    put previously deleted text after the cursor

## The replace command

```rx```                       :    replace the character at the cursor with x

## The changer operator

```ce```                       :    change until the end of a word

## More changes using ```c```

```c$```                       :    type the rest of the line like the second and press

## Cursor location and file status

```<C-g>```                    :    show your location in a file and the file status
```G```                        :    move to a line in the file

## The search command

```/```                        :    followed by a phrase to search for the phrase
```n```                        :    search for the same phrase again
```N```                        :    search for the same phrase in the opposite direction
```?```                        :    search for a phrase in the backward direction
```<C-o>```                    :    go back to where you came
```<C-i>```                    :    goes forward

## Matching parentheses search

```%```                        :    find a matching ), ] or }

## The substitute command

```:s```                       :    substitute command

## How to execute an external

```!```                        :    this allows you to execute any external shell command
```:```                        :    set the cursor at the bottom of the screen, this allows you to enter a command-line command
```!ls```                      :    get a listing of your directory

## More on writing files

```:w```                       :    save
```:w <FILENAME>```            :    save changes made to get a listing of your directory
```!rm <FILENAME>```           :    removing the file

## Selecting text to write

```v```                        :    starts Visual-mode

## Retrieving and merging files

```:r <FILENAME>```            :    insert the contents of a file

## The open command

```o```                        :    open a line bellow the cursor and place you in insert mode

## The append command

```a```                        :    insert text after the cursor
```e```                        :    cursor at the and of word

## Another way to replace

```R```                        :    replace mode

## Copy and paste text

```y```                        :    operator to copy text
```p```                        :    paste
```j$```                       :    move the cursor to the end of the line
```yw```                       :    yanks one word

## Set option

```:set ic```                       :    set ignore case option
```:set hls is```                   :    set the 'hlsearch' and 'incsearch'
```:set noic```                     :    disable ignoring case enter
```:set invic```                    :    toggle the value of a setting
```nohlsearch```                    :    remove the highlighting of matches enter

## Getting help

```<HELP>```                        :    Vim has a comprehesive on-line help system
```<F1>```                          :    Vim has a comprehesive on-line help system
```<C-w><C-w>```                    :    jump from one window to another
```:help <argument>```              :    you can find help on just about any subject, by giving an argument

## Completion

```<C-d>```                         :    command line completion
```<Tab>```                         :    command line completion


```<number-G>```               :    moves to that line number
```gg```                       :    move you to the start of the file


```<C-j>```                    :    jump to a subject
```<C-o>```                    :    jump back
```<C-d>```                    :    see matching search
```<C-t>```                    :    

## Basic

quickref                              :            overview of the most common commands you will use
tutor                                    :            20 minutes training course for beginners
copying                               :            about copyrights
iccf                                      :            helping poor children in Uganda
sponsor                                :            sponsor Vim development, become a registered Vim user
www                                    :           Vim on the World Wide Web
bugs                                     :            where to send bug reports

usr_toc.txt                            :            table of contents

## Getting Started
usr_01.txt                             :            about the manuals
usr_02.txt                             :            the first steps in Vim
usr_03.txt                             :            moving around
usr_04.txt                             :            making small changes
usr_05.txt                             :            set your settings
usr_06.txt                             :            using syntax highlighting
usr_07.txt                             :            editing more than one file
usr_08.txt                             :            spliting windows
usr_09.txt                             :            using the GUI
usr_10.txt                             :            making big changes
usr_11.txt                             :            recovering from a crash
usr_12.txt                             :            clever tricks

## Editing Effectively

usr_20.txt                             :            typing command-line commands quickly
usr_21.txt                             :            go away and come back
usr_22.txt                             :            finding the file to edit
usr_23.txt                             :            editing other files
usr_24.txt                             :            inserting quickly
usr_25.txt                             :            editing formatted text
usr_26.txt                             :            repeating
usr_27.txt                             :            search commands and patterns
usr_28.txt                             :            folding
usr_29.txt                             :            moving through programs
usr_30.txt                             :            editing programs
usr_31.txt                             :            exploiting the GUI
usr_32.txt                             :            the undo tree

## Tuning Vim

usr_40.txt                             :            make new commands
usr_41.txt                             :            write a Vim script
usr_42.txt                             :            add new menus
usr_43.txt                             :            using filetypes
usr_44.txt                             :            your own syntax highlighted
usr_45.txt                             :            select your language

## General subjects

### Nvim *ref* *reference* *intro.txt*

[]		Characters in square brackets are optional.

						    *count* *[count]*
[count]		An optional number that may precede the command to multiply
		or iterate the command.  If no number is given, a count of one
		is used, unless otherwise noted.  Note that in this manual the
		[count] is not mentioned in the description of the command,
		but only in the explanation.  This was done to make the
		commands easier to look up.  If the 'showcmd' option is on,
		the (partially) entered count is shown at the bottom of the
		window.  You can use <Del> to erase the last digit (|N<Del>|).

							*[quotex]*
["x]		An optional register designation where text can be stored.
		See |registers|.  The x is a single character between 'a' and
		'z' or 'A' and 'Z' or '"'', and in some cases (with the put
		command) between '0' and '9', '%', '#', or others.  The
		uppercase and lowercase letter designate the same register,
		but the lowercase letter is used to overwrite the previous
		register contents, while the uppercase letter is used to
		append to the previous register contents.  Without the ""x" or
		with """" the stored text is put into the unnamed register.

							*{}*
{}		Curly braces denote parts of the command which must appear,
		but which can take a number of different values.  The
		differences between Vim and Vi are also given in curly braces
		(this will be clear from the context).

							*{char1-char2}*
{char1-char2}	A single character from the range char1 to char2.  For
		example: {a-z} is a lowercase letter.  Multiple ranges may be
		concatenated.  For example, {a-zA-Z0-9} is any alphanumeric
		character.

						*{motion}* *movement*
{motion}	A command that moves the cursor.  These are explained in
		|motion.txt|.  Examples:
			w		to start of next word
			b		to begin of current word
			4j		four lines down
			/The<CR>	to next occurrence of "The"
		This is used after an |operator| command to move over the text
		that is to be operated upon.
		- If the motion includes a count and the operator also has a
		  count, the two counts are multiplied.  For example: "2d3w"
		  deletes six words.
		- The motion can be backwards, e.g. "db" to delete to the
		  start of the word.
		- The motion can also be a mouse click.  The mouse is not
		  supported in every terminal though.
		- The ":omap" command can be used to map characters while an
		  operator is pending.
		- Ex commands can be used to move the cursor.  This can be
		  used to call a function that does some complicated motion.
		  The motion is always charwise exclusive, no matter
		  what ":" command is used.  This means it's impossible to
		  include the last character of a line without the line break
		  (unless 'virtualedit' is set).
		  If the Ex command changes the text before where the operator
		  starts or jumps to another buffer the result is
		  unpredictable.  It is possible to change the text further
		  down.  Jumping to another buffer is possible if the current
		  buffer is not unloaded.

							*{Visual}*
{Visual}	A selected text area.  It is started with the "v", "V", or
		CTRL-V command, then any cursor movement command can be used
		to change the end of the selected text.
		This is used before an |operator| command to highlight the
		text that is to be operated upon.
		See |Visual-mode|.

							*<character>*
<character>	A special character from the table below, optionally with
		modifiers, or a single ASCII character with modifiers.

							*'character'*
'c'		A single ASCII character.

							*CTRL-{char}*
CTRL-{char}	{char} typed as a control character; that is, typing {char}
		while holding the CTRL key down.  The case of {char} does not
		matter; thus CTRL-A and CTRL-a are equivalent.  But on some
		terminals, using the SHIFT key will produce another code,
		don't use it then.

							*'option'*
'option'	An option, or parameter, that can be set to a value, is
		enclosed in single quotes.  See |options|.

							*quotecommandquote*
"command"	A reference to a command that you can type is enclosed in
		double quotes.
`command`	New style command, this distinguishes it from other quoted
		text and strings.

	*Normal* *Normal-mode* *command-mode*
Normal mode		In Normal mode you can enter all the normal editor
			commands.  If you start the editor you are in this
			mode (unless you have set the 'insertmode' option,
			see below).  This is also known as command mode.

Visual mode		This is like Normal mode, but the movement commands
			extend a highlighted area.  When a non-movement
			command is used, it is executed for the highlighted
			area.  See |Visual-mode|.
			If the 'showmode' option is on "-- VISUAL --" is shown
			at the bottom of the window.

Select mode		This looks most like the MS-Windows selection mode.
			Typing a printable character deletes the selection
			and starts Insert mode.  See |Select-mode|.
			If the 'showmode' option is on "-- SELECT --" is shown
			at the bottom of the window.

Insert mode		In Insert mode the text you type is inserted into the
			buffer.  See |Insert-mode|.
			If the 'showmode' option is on "-- INSERT --" is shown
			at the bottom of the window.

Command-line mode	In Command-line mode (also called Cmdline mode) you
Cmdline mode		can enter one line of text at the bottom of the
			window.  This is for the Ex commands, ":", the pattern
			search commands, "?" and "/", and the filter command,
			"!".  |Cmdline-mode|

Ex mode			Like Command-line mode, but after entering a command
			you remain in Ex mode.  Very limited editing of the
			command line.  |Ex-mode|

							*Terminal-mode*
Terminal mode		In Terminal mode all input (except CTRL-\) is sent to
			the process running in the current |terminal| buffer.

	*Operator-pending* *Operator-pending-mode*
Operator-pending mode	This is like Normal mode, but after an operator
			command has started, and Vim is waiting for a {motion}
			to specify the text that the operator will work on.

Replace mode		Replace mode is a special case of Insert mode.  You
			can do the same things as in Insert mode, but for
			each character you enter, one character of the existing
			text is deleted.  See |Replace-mode|.
			If the 'showmode' option is on "-- REPLACE --" is
			shown at the bottom of the window.

Virtual Replace mode	Virtual Replace mode is similar to Replace mode, but
			instead of file characters you are replacing screen
			real estate.  See |Virtual-Replace-mode|.
			If the 'showmode' option is on "-- VREPLACE --" is
			shown at the bottom of the window.

Insert Normal mode	Entered when CTRL-O is typed in Insert mode (see
			|i_CTRL-O|).  This is like Normal mode, but after
			executing one command Vim returns to Insert mode.
			If the 'showmode' option is on "-- (insert) --" is
			shown at the bottom of the window.

Insert Visual mode	Entered when starting a Visual selection from Insert
			mode, e.g., by using CTRL-O and then "v", "V" or
			CTRL-V.  When the Visual selection ends, Vim returns
			to Insert mode.
			If the 'showmode' option is on "-- (insert) VISUAL --"
			is shown at the bottom of the window.

Insert Select mode	Entered when starting Select mode from Insert mode.
			E.g., by dragging the mouse or <S-Right>.

help.txt                                 :            overview and quick reference (this file)
helphelp.txt                          :            about using the help files
index.txt                               :            alphabetical index of all commands
help-tags                               :           all the tags you can jump to (index of tags)
tips.txt                                   :           various tips on using Vim
message.txt                           :           (error) messages and explanations
develop.txt                            :           development of Nvim
debug.txt                               :           debugging Vim itself
uganda.txt                             :           Vim distribution conditions and what to do with your money

## Basic editing

### Starting Vim *starting* starting.txt

```nvim [option | filename]```         :    more generally, Nvim is started with option arguments and file name arguments can be mixed, and any number of them can be given.
```filename```                         :    one or more file names.The first one will be the current file and read into the buffer.
```-```                                :    alias for stdin (standart input)
```-t{tag}```                          :    a tag. "tag" is locked up in the tags file, the associated file becomes the current file, and the associated command is executed.
```-q[errorfile]```                    :    quickfix mode. The file with the name [errorfile] is read and the first is displayed.
```(nothing)```                        :    without one of the four items above, Vim will start editing a new buffer.

```--help, -?, -h```                   :    give usage (help) message and exit.
```--version, -v```                    :    print version information and exit.
```--clean```                          :    mimics a fresh install of Nvim.
```--noplugin```                       :    skip loading plugins. Reset the 'loadplugins' option.
```--startuptime {fname}```            :    during startup write timing messages to the file {fname}. This can be used to find out where time is spent while loading your config, plugins and opening the first file.
```+[num]```                           :    the cursor will be positioned on line "num" for the first file being edited. If "num" is missing, the cursor will be positioned on the last line.
```+/{pat}```                          :    the cursor will be positioned on the first line containing "pat" in the first file being edited (see |pattern| for the available search patterns).
```+{command}, -c {command}```         :    {command} will be executed after the first file has been read (and after autocommands and moderlines for that file have been processed).
```--cmd {command}```                  :    {command} will be executed before processing any vimrc file.
```-S {file}```                        :    the {file} will be sourced after the first file has been read.
```-S```                               :    works like "-S Session.vim".
```-L, -r```                           :    recovery mode. Without a file name argument, a list of existing swap files is given. With a file name, a swap file is read to recover a crashed editing session.
```-R```                               :    readonly mode. The 'readonly' option will be set for all the files being edited. You can still edit the buffer, but will be prevented from accidentally overwriting a file.
```-m```                               :    modifications not allowed to be written. The 'write' option will be reset, so that writing files is disabled.
```-M```                               :    modifications not allowed. The 'modifiable' option will be reset, so that changes are not allowed.
```-e, -E```                           :    start Nvim in Ex mode.
```-es, -Es```                         :    silient mode (no UI), for scripting. Unrelated to |-s|.
```-b```                               :    binary mode. File I/O will only recognize <NL> to separate lines.
```-l```                               :    lisp mode.
```-A```                               :    arabic mode.
```-H```                               :    hebrew mode.
```-V[N]```                            :    verbose. Set the 'verbose' option to [N] (default: 10).
```-V[N]{filename}```                  :    like -V and set 'verbosefile' to {filename}. Message are not displayed; instead they are written to the file {filename}.
```-D```                               :    debugging. go to debugging mode when executing the first command from a script.
```-n```                               :    no |swap-file| will be used. Recovery after a crash will be imposible.
```-o[N]```                            :    open N windows, split horizontely. If [N] is not given, one window is opened for every file given as argument.
```-O[N]```                            :    open N window, split vertically. Otherwise it's like -o.
```-p[N]```                            :    open N tab pages. If [N] is not given, one tab page is opened for every file as argument.
```-d```                               :    start in |diff-mode|.
```-u {vimrc}```                       :    the file {vimrc} is read for initializations.
```i {shida}```                        :    the file {shada} is used instead of the default ShaDa file.
```-s {scriptin}```                    :    read script file {scriptin}, interpreting characters as Normal-mode input.
```-w{number}```                       :    set the 'window' option to {number}.
```-w {scriptout}```                   :    all keys that you type are recorded in the file "scriptout", until you exit Vim.
```-W {scriptout}```                   :    like -w, but do not append, overwrite an existing file.
```--api-info```                       :    print msgpack-encoded |api-metadata| and exit.
```--embed```                          :    use stdin/stdout as a msgpack-RPC channel, so applications can embed and control Nvim via the RPC |API|.
```--headless```                       :    start without UI, and do not wait for `nvim_ui_attach`.
```--listen {addr}```                  :    start |RPC| server on pipe or TCP address {addr}.

```<C-z>```                            :    suspend Nvim, like ":stop".
```:sus[pend][!] or :st[op][!]```      :    suspend Nvim using OS "job control"; it will continue if you make it the foreground job again.

```:mk[exrc][file]```                  :    write current key mapping and changed options to [file] (default ".exrc" in the current directory), unless it already exists.
```:mk[exrc]! [file]```                :    always write current key mapping and changed options to [file] (default ".exrc" in the current directory).
```:mk[imrc][!] [file]```              :    like ":mkexrc", but the default is ".nvimrc" in the current directory.
```:mkvie[w][!] [file]```              :    write a Vim script that restores the contents of the current window.
```:lo[adview] [nr]```                 :    load the view for the current file. When [nr] is omitted, the view stored with ":mkview" is loaded.

```:rsh[ada][!] [file]```              :    read from ShaDa file [file] (default: see above).
```:wsh[ada][!] [file]```              :    write to ShaDa file [file] (default: see above).
```:o[ldfiles]```                      :    list the files that have marks stored in the ShaDa file.
```bro[wse] o[ldfiles][!]```           :    list file names as with |:oldfiles|, and then prompt for a number.

### Editing files *edit-files* *editing.txt*

*:keepalt* *:keepa*
:keepalt {cmd}		Execute {cmd} while keeping the current alternate file
			name.
	
	CTRL-G		or				*CTRL-G* *:f* *:fi* *:file*
:f[ile]			Prints the current file name (as typed, unless ":cd"
			was used), the cursor position (unless the 'ruler'
			option is set), and the file status (readonly,
			modified, read errors, new file).  See the 'shortmess'
			option about how to make this message shorter.

:f[ile]!		like |:file|, but don't truncate the name even when
			'shortmess' indicates this.

{count}CTRL-G		Like CTRL-G, but prints the current file name with
			full path.  If the count is higher than 1 the current
			buffer number is also given.

					*g_CTRL-G* *word-count* *byte-count*
g CTRL-G		Prints the current position of the cursor in five
			ways: Column, Line, Word, Character and Byte.  If the
			number of Characters and Bytes is the same then the
			Character position is omitted.

			If there are characters in the line that take more
			than one position on the screen (<Tab> or special
			character), or characters using more than one byte per
			column (characters above 0x7F when 'encoding' is
			utf-8), both the byte column and the screen column are
			shown, separated by a dash.

			Also see the 'ruler' option and the |wordcount()|
			function.

							*v_g_CTRL-G*
{Visual}g CTRL-G	Similar to "g CTRL-G", but Word, Character, Line, and
			Byte counts for the visually selected region are
			displayed.
			In Blockwise mode, Column count is also shown.  (For
			{Visual} see |Visual-mode|.)

							*:file_f*
:f[ile][!] {name}	Sets the current file name to {name}.  The optional !
			avoids truncating the message, as with |:file|.
			If the buffer did have a name, that name becomes the
			|alternate-file| name.  An unlisted buffer is created
			to hold the old name.

							*:0file*
:0f[ile][!]		Remove the name of the current buffer.  The optional !
			avoids truncating the message, as with |:file|.

:buffers
:files
:ls			List all the currently known file names.  See
			|windows.txt| |:files| |:buffers| |:ls|.

	:e[dit] [++opt] [+cmd]	Edit the current file.  This is useful to re-edit the
			current file, when it has been changed outside of Vim.
			This fails when changes have been made to the current
			buffer and 'autowriteall' isn't set or the file can't
			be written.
			Also see |++opt| and |+cmd|.

							*:edit!* *discard*
:e[dit]! [++opt] [+cmd]
			Edit the current file always.  Discard any changes to
			the current buffer.  This is useful if you want to
			start all over again.
			Also see |++opt| and |+cmd|.

							*:edit_f*
:e[dit] [++opt] [+cmd] {file}
			Edit {file}.
			This fails when changes have been made to the current
			buffer, unless 'hidden' is set or 'autowriteall' is
			set and the file can be written.
			Also see |++opt| and |+cmd|.

							*:edit!_f*
:e[dit]! [++opt] [+cmd] {file}
			Edit {file} always.  Discard any changes to the
			current buffer.
			Also see |++opt| and |+cmd|.

:e[dit] [++opt] [+cmd] #[count]
			Edit the [count]th buffer (as shown by |:files|).
			This command does the same as [count] CTRL-^.  But ":e
			#" doesn't work if the alternate buffer doesn't have a
			file name, while CTRL-^ still works then.
			Also see |++opt| and |+cmd|.

							*:ene* *:enew*
:ene[w]			Edit a new, unnamed buffer.  This fails when changes
			have been made to the current buffer, unless 'hidden'
			is set or 'autowriteall' is set and the file can be
			written.
			If 'fileformats' is not empty, the first format given
			will be used for the new buffer.  If 'fileformats' is
			empty, the 'fileformat' of the current buffer is used.

							*:ene!* *:enew!*
:ene[w]!		Edit a new, unnamed buffer.  Discard any changes to
			the current buffer.
			Set 'fileformat' like |:enew|.

							*:fin* *:find*
:fin[d][!] [++opt] [+cmd] {file}
			Find {file} in 'path' and then |:edit| it.

:{count}fin[d][!] [++opt] [+cmd] {file}
			Just like ":find", but use the {count} match in
			'path'.  Thus ":2find file" will find the second
			"file" found in 'path'.  When there are fewer matches
			for the file in 'path' than asked for, you get an
			error message.

							*:ex*
:ex [++opt] [+cmd] [file]
			Same as |:edit|.

							*:vi* *:visual*
:vi[sual][!] [++opt] [+cmd] [file]
			When used in Ex mode: Leave |Ex-mode|, go back to
			Normal mode.  Otherwise same as |:edit|.

							*:vie* *:view*
:vie[w][!] [++opt] [+cmd] file
			When used in Ex mode: Leave |Ex-mode|, go back to
			Normal mode.  Otherwise same as |:edit|, but set
			'readonly' option for this buffer.

							*CTRL-^* *CTRL-6*
CTRL-^			Edit the alternate file.  Mostly the alternate file is
			the previously edited file.  This is a quick way to
			toggle between two files.  It is equivalent to ":e #",
			except that it also works when there is no file name.

			If the 'autowrite' or 'autowriteall' option is on and
			the buffer was changed, write it.
			Mostly the ^ character is positioned on the 6 key,
			pressing CTRL and 6 then gets you what we call CTRL-^.
			But on some non-US keyboards CTRL-^ is produced in
			another way.

{count}CTRL-^		Edit [count]th file in the buffer list (equivalent to
			":e #[count]").  This is a quick way to switch between
			files.
			See |CTRL-^| above for further details.

							*gf* *E446* *E447*
[count]gf		Edit the file whose name is under or after the cursor.
			Mnemonic: "goto file".
			Uses the 'isfname' option to find out which characters
			are supposed to be in a file name.  Trailing
			punctuation characters ".,:;!" are ignored. Escaped
			spaces "\ " are reduced to a single space.
			Uses the 'path' option as a list of directory names to
			look for the file.  See the 'path' option for details
			about relative directories and wildcards.
			Uses the 'suffixesadd' option to check for file names
			with a suffix added.
			If the file can't be found, 'includeexpr' is used to
			modify the name and another attempt is done.
			If a [count] is given, the count'th file that is found
			in the 'path' is edited.
			This command fails if Vim refuses to |abandon| the
			current file.
			If you want to edit the file in a new window use
			|CTRL-W_CTRL-F|.
			If you do want to edit a new file, use:
				:e <cfile>
 			To make gf always work like that:
				:map gf :e <cfile><CR>
 			If the name is a hypertext link, that looks like
			"type://machine/path", you need the |netrw| plugin.
			For Unix the '~' character is expanded, like in
			"~user/file".  Environment variables are expanded too
			|expand-env|.

							*v_gf*
{Visual}[count]gf	Same as "gf", but the highlighted text is used as the
			name of the file to edit.  'isfname' is ignored.
			Leading blanks are skipped, otherwise all blanks and
			special characters are included in the file name.
			(For {Visual} see |Visual-mode|.)

							*gF*
[count]gF		Same as "gf", except if a number follows the file
			name, then the cursor is positioned on that line in
			the file.
			The file name and the number must be separated by a
			non-filename (see 'isfname') and non-numeric
			character. " line " is also recognized, like it is
			used in the output of `:verbose command UserCmd`
			White space between the filename, the separator and
			the number are ignored.
			Examples:
				eval.c:10 
				eval.c @ 20 
				eval.c (30) 
				eval.c 40 

							*v_gF*
{Visual}[count]gF	Same as "v_gf".

*:ar* *:arg* *:args*
:ar[gs]			Print the argument list, with the current file in
			square brackets.

:ar[gs] [++opt] [+cmd] {arglist}			*:args_f*
			Define {arglist} as the new argument list and edit
			the first one.  This fails when changes have been made
			and Vim does not want to |abandon| the current buffer.
			Also see |++opt| and |+cmd|.

:ar[gs]! [++opt] [+cmd] {arglist}			*:args_f!*
			Define {arglist} as the new argument list and edit
			the first one.  Discard any changes to the current
			buffer.
			Also see |++opt| and |+cmd|.

:[count]arge[dit][!] [++opt] [+cmd] {name} ..		*:arge* *:argedit*
			Add {name}s to the argument list and edit it.
			When {name} already exists in the argument list, this
			entry is edited.
			This is like using |:argadd| and then |:edit|.
			Spaces in filenames have to be escaped with "\".
			[count] is used like with |:argadd|.
			If the current file cannot be |abandon|ed {name}s will
			still be added to the argument list, but won't be
			edited. No check for duplicates is done.
			Also see |++opt| and |+cmd|.

:[count]arga[dd] {name} ..			*:arga* *:argadd* *E479*
:[count]arga[dd]
			Add the {name}s to the argument list.  When {name} is
			omitted add the current buffer name to the argument
			list.
			If [count] is omitted, the {name}s are added just
			after the current entry in the argument list.
			Otherwise they are added after the [count]'th file.
			If the argument list is "a b c", and "b" is the
			current argument, then these commands result in:
				command		new argument list 
				:argadd x	a b x c
				:0argadd x	x a b c
				:1argadd x	a x b c
				:$argadd x	a b c x
			And after the last one:
				:+2argadd y	a b c x y
			There is no check for duplicates, it is possible to
			add a file to the argument list twice.
			The currently edited file is not changed.
			Note: you can also use this method:
				:args ## x
 			This will add the "x" item and sort the new list.

:argd[elete] {pattern} ..		*:argd* *:argdelete* *E480* *E610*
			Delete files from the argument list that match the
			{pattern}s.  {pattern} is used like a file pattern,
			see |file-pattern|.  "%" can be used to delete the
			current entry.
			This command keeps the currently edited file, also
			when it's deleted from the argument list.
			Example:
				:argdel *.obj

:[range]argd[elete]	Delete the [range] files from the argument list.
			Example:
				:10,$argdel
 			Deletes arguments 10 and further, keeping 1-9.
				:$argd
 			Deletes just the last one.
				:argd
				:.argd
 			Deletes the current argument.
				:%argd
 			Removes all the files from the arglist.
			When the last number in the range is too high, up to
			the last argument is deleted.

							*:argu* *:argument*
:[count]argu[ment] [count] [++opt] [+cmd]
			Edit file [count] in the argument list.  When [count]
			is omitted the current entry is used.  This fails
			when changes have been made and Vim does not want to
			|abandon| the current buffer.
			Also see |++opt| and |+cmd|.

:[count]argu[ment]! [count] [++opt] [+cmd]
			Edit file [count] in the argument list, discard any
			changes to the current buffer.  When [count] is
			omitted the current entry is used.
			Also see |++opt| and |+cmd|.

:[count]n[ext] [++opt] [+cmd]			*:n* *:ne* *:next* *E165* *E163*
			Edit [count] next file.  This fails when changes have
			been made and Vim does not want to |abandon| the
			current buffer.  Also see |++opt| and |+cmd|.

:[count]n[ext]! [++opt] [+cmd]
			Edit [count] next file, discard any changes to the
			buffer.  Also see |++opt| and |+cmd|.

:n[ext] [++opt] [+cmd] {arglist}			*:next_f*
			Same as |:args_f|.

:n[ext]! [++opt] [+cmd] {arglist}
			Same as |:args_f!|.

:[count]N[ext] [count] [++opt] [+cmd]			*:Next* *:N* *E164*
			Edit [count] previous file in argument list.  This
			fails when changes have been made and Vim does not
			want to |abandon| the current buffer.
			Also see |++opt| and |+cmd|.

:[count]N[ext]! [count] [++opt] [+cmd]
			Edit [count] previous file in argument list.  Discard
			any changes to the buffer.  Also see |++opt| and
			|+cmd|.

:[count]prev[ious] [count] [++opt] [+cmd]		*:prev* *:previous*
			Same as :Next.  Also see |++opt| and |+cmd|.

							*:rew* *:rewind*
:rew[ind] [++opt] [+cmd]
			Start editing the first file in the argument list.
			This fails when changes have been made and Vim does
			not want to |abandon| the current buffer.
			Also see |++opt| and |+cmd|.

:rew[ind]! [++opt] [+cmd]
			Start editing the first file in the argument list.
			Discard any changes to the buffer.  Also see |++opt|
			and |+cmd|.

							*:fir* *:first*
:fir[st][!] [++opt] [+cmd]
			Other name for ":rewind".

							*:la* *:last*
:la[st] [++opt] [+cmd]
			Start editing the last file in the argument list.
			This fails when changes have been made and Vim does
			not want to |abandon| the current buffer.
			Also see |++opt| and |+cmd|.

:la[st]! [++opt] [+cmd]
			Start editing the last file in the argument list.
			Discard any changes to the buffer.  Also see |++opt|
			and |+cmd|.

							*:wn* *:wnext*
:[count]wn[ext] [++opt]
			Write current file and start editing the [count]
			next file.  Also see |++opt| and |+cmd|.

:[count]wn[ext] [++opt] {file}
			Write current file to {file} and start editing the
			[count] next file, unless {file} already exists and
			the 'writeany' option is off.  Also see |++opt| and
			|+cmd|.

:[count]wn[ext]! [++opt] {file}
			Write current file to {file} and start editing the
			[count] next file.  Also see |++opt| and |+cmd|.

:[count]wN[ext][!] [++opt] [file]		*:wN* *:wNext*

:[count]wp[revious][!] [++opt] [file]		*:wp* *:wprevious*
			Same as :wnext, but go to previous file instead of
			next.
	
	*:arglocal*
:argl[ocal]		Make a local copy of the global argument list.
			Doesn't start editing another file.

:argl[ocal][!] [++opt] [+cmd] {arglist}
			Define a new argument list, which is local to the
			current window.  Works like |:args_f| otherwise.

							*:argglobal*
:argg[lobal]		Use the global argument list for the current window.
			Doesn't start editing another file.

:argg[lobal][!] [++opt] [+cmd] {arglist}
			Use the global argument list for the current window.
			Define a new global argument list like |:args_f|.

	*:argdo*
:[range]argdo[!] {cmd}	Execute {cmd} for each file in the argument list or,
			if [range] is specified, only for arguments in that
			range.
	
	*:w* *:write*
					*E502* *E503* *E504* *E505*

					*E512* *E514* *E667* *E796* *E949*
:w[rite] [++opt]	Write the whole buffer to the current file.  This is
			the normal way to save changes to a file.  It fails
			when the 'readonly' option is set or when there is
			another reason why the file can't be written.
			For ++opt see |++opt|, but only ++bin, ++nobin, ++ff
			and ++enc are effective.

:w[rite]! [++opt]	Like ":write", but forcefully write when 'readonly' is
			set or there is another reason why writing was
			refused.
			Note: This may change the permission and ownership of
			the file and break (symbolic) links.  Add the 'W' flag
			to 'cpoptions' to avoid this.

:[range]w[rite][!] [++opt]
			Write the specified lines to the current file.  This
			is unusual, because the file will not contain all
			lines in the buffer.

							*:w_f* *:write_f*
:[range]w[rite] [++opt]	{file}
			Write the specified lines to {file}, unless it
			already exists and the 'writeany' option is off.

							*:w!*
:[range]w[rite]! [++opt] {file}
			Write the specified lines to {file}.  Overwrite an
			existing file.

						*:w_a* *:write_a* *E494*
:[range]w[rite][!] [++opt] >>
			Append the specified lines to the current file.

:[range]w[rite][!] [++opt] >> {file}
			Append the specified lines to {file}.  '!' forces the
			write even if file does not exist.

							*:w_c* *:write_c*
:[range]w[rite] [++opt] !{cmd}
			Execute {cmd} with [range] lines as standard input
			(note the space in front of the '!').

	*:sav* *:saveas*
:sav[eas][!] [++opt] {file}
			Save the current buffer under the name {file} and set
			the filename of the current buffer to {file}.  The
			previous name is used for the alternate file name.
			The [!] is needed to overwrite an existing file.
			When 'filetype' is empty filetype detection is done
			with the new name, before the file is written.
			When the write was successful 'readonly' is reset.

							*:up* *:update*
:[range]up[date][!] [++opt] [>>] [file]
			Like ":write", but only write when the buffer has been
			modified.

WRITING WITH MULTIPLE BUFFERS				*buffer-write*

							*:wa* *:wall*
:wa[ll]			Write all changed buffers.  Buffers without a file
			name cause an error message.  Buffers which are
			readonly are not written.

:wa[ll]!		Write all changed buffers, even the ones that are
			readonly.

	*:q* *:quit*
:q[uit]			Quit the current window.  Quit Vim if this is the last
			|edit-window|.  This fails when changes have been made
			and Vim refuses to |abandon| the current buffer, and
			when the last file in the argument list has not been
			edited.
			If there are other tab pages and quitting the last
			window in the current tab page the current tab page is
			closed |tab-page|.
			Triggers the |QuitPre| autocommand event.
			See |CTRL-W_q| for quitting another window.

:conf[irm] q[uit]	Quit, but give prompt when changes have been made, or
			the last file in the argument list has not been
			edited.  See |:confirm| and 'confirm'.

:q[uit]!		Quit without writing, also when the current buffer has
			changes.  The buffer is unloaded, also when it has
			'hidden' set.
			If this is the last window and there is a modified
			hidden buffer, the current buffer is abandoned and the
			first changed hidden buffer becomes the current
			buffer.
			Use ":qall!" to exit always.

:cq[uit]		Quit always, without writing, and return an error
			code.  See |:cq|.

							*:wq*
:wq [++opt]		Write the current file and close the window.  If this
			was the last |edit-window| Vim quits.
			Writing fails when the file is read-only or the buffer
			does not have a name.  Quitting fails when the last
			file in the argument list has not been edited.

:wq! [++opt]		Write the current file and close the window.  If this
			was the last |edit-window| Vim quits.  Writing fails
			when the current buffer does not have a name.

:wq [++opt] {file}	Write to {file} and close the window.  If this was the
			last |edit-window| Vim quits.  Quitting fails when the
			last file in the argument list has not been edited.

:wq! [++opt] {file}	Write to {file} and close the current window.  Quit
			Vim if this was the last |edit-window|.

:[range]wq[!] [++opt] [file]
			Same as above, but only write the lines in [range].

							*:x* *:xit*
:[range]x[it][!] [++opt] [file]
			Like ":wq", but write only when changes have been
			made.
			When 'hidden' is set and there are more windows, the
			current buffer becomes hidden, after writing the file.

							*:exi* *:exit*
:[range]exi[t][!] [++opt] [file]
			Same as :xit.

							*ZZ*
ZZ			Write current file, if modified, and close the current
			window (same as ":x").
			If there are several windows for the current file,
			only the current window is closed.

							*ZQ*
ZQ			Quit without checking for changes (same as ":q!").

MULTIPLE WINDOWS AND BUFFERS				*window-exit*

							*:qa* *:qall*
:qa[ll]		Exit Vim, unless there are some buffers which have been
		changed.  (Use ":bmod" to go to the next modified buffer).
		When 'autowriteall' is set all changed buffers will be
		written, like |:wqall|.

:conf[irm] qa[ll]
		Exit Vim.  Bring up a prompt when some buffers have been
		changed.  See |:confirm|.

:qa[ll]!	Exit Vim.  Any changes to buffers are lost.
		Also see |:cquit|, it does the same but exits with a non-zero
		value.

							*:quita* *:quitall*
:quita[ll][!]	Same as ":qall".

:wqa[ll] [++opt]				*:wqa* *:wqall* *:xa* *:xall*
:xa[ll]		Write all changed buffers and exit Vim.  If there are buffers
		without a file name, which are readonly or which cannot be
		written for another reason, Vim will not quit.

:conf[irm] wqa[ll] [++opt]
:conf[irm] xa[ll]
		Write all changed buffers and exit Vim.  Bring up a prompt
		when some buffers are readonly or cannot be written for
		another reason.  See |:confirm|.

:wqa[ll]! [++opt]
:xa[ll]!	Write all changed buffers, even the ones that are readonly,
		and exit Vim.

	*:confirm* *:conf*
:conf[irm] {command}	Execute {command}, and use a dialog when an
			operation has to be confirmed.  Can be used on the
			|:q|, |:qa| and |:w| commands (the latter to override
			a read-only setting), and any other command that can
			fail in such a way, such as |:only|, |:buffer|,
			|:bdelete|, etc.

Examples:
  :confirm w foo
 	Will ask for confirmation when "foo" already exists.
  :confirm q
 	Will ask for confirmation when there are changes.
  :confirm qa
 	If any modified, unsaved buffers exist, you will be prompted to save
	or abandon each one.  There are also choices to "save all" or "abandon
	all".

If you want to always use ":confirm", set the 'confirm' option.

			*:browse* *:bro* *E338* *E614* *E615* *E616*
:bro[wse] {command}	Open a file selection dialog for an argument to
			{command}.

	*:cd* *E747* *E472*
:cd[!]			On non-Unix systems when 'cdhome' is off: Print the
			current directory name.
			Otherwise: Change the current directory to the home
			directory.  Clear any window-local directory.
			Use |:pwd| to print the current directory on all
			systems.

:cd[!] {path}		Change the current directory to {path}.
			If {path} is relative, it is searched for in the
			directories listed in |'cdpath'|.
			Does not change the meaning of an already opened file,
			because its full path name is remembered.  Files from
			the |arglist| may change though!
			On MS-Windows this also changes the active drive.
			To change to the directory of the current file:
				:cd %:h

							*:cd-* *E186*
:cd[!] -		Change to the previous current directory (before the
			previous ":cd {path}" command).

							*:chd* *:chdir*
:chd[ir][!] [path]	Same as |:cd|.

							*:tc* *:tcd*
:tc[d][!] {path}	Like |:cd|, but only set the directory for the current
			tab.  The current window will also use this directory.
			The current directory is not changed for windows in
			other tabs and for windows in the current tab that
			have their own window-local directory.

							*:tcd-*
:tc[d][!] -		Change to the previous current directory (before the
			previous ":tcd {path}" command).

							*:tch* *:tchdir*
:tch[dir][!]		Same as |:tcd|.

							*:lc* *:lcd*
:lc[d][!] {path}	Like |:cd|, but only set the current directory for the
			current window.  The current directory for other
			windows or tabs is not changed.

							*:lch* *:lchdir*
:lch[dir][!]		Same as |:lcd|.

							*:lcd-*
:lc[d][!] -		Change to the previous current directory (before the
			previous ":lcd {path}" command).

							*:pw* *:pwd* *E187*
:pw[d]			Print the current directory name.
			Also see |getcwd()|.

	*:checkt* *:checktime*
:checkt[ime]		Check if any buffers were changed outside of Vim.
			This checks and warns you if you would end up with two
			versions of a file.
			If this is called from an autocommand, a ":global"
			command or is not typed the actual check is postponed
			until a moment the side effects (reloading the file)
			would be harmless.
			Each loaded buffer is checked for its associated file
			being changed.  If the file was changed Vim will take
			action.  If there are no changes in the buffer and
			'autoread' is set, the buffer is reloaded.  Otherwise,
			you are offered the choice of reloading the file.  If
			the file was deleted you get an error message.
			If the file previously didn't exist you get a warning
			if it exists now.
			Once a file has been checked the timestamp is reset,
			you will not be warned again.

:[N]checkt[ime] {filename}
:[N]checkt[ime] [N]
			Check the timestamp of a specific buffer.  The buffer
			may be specified by name, number or with a pattern.

### Cursor motions *cursor-motions* *navigation* *motion.txt*

	|c|	c	change
	|d|	d	delete
	|y|	y	yank into register (does not change the text)
	|~|	~	swap case (only if 'tildeop' is set)
	|g~|	g~	swap case
	|gu|	gu	make lowercase
	|gU|	gU	make uppercase
	|!|	!	filter through an external program
	|=|	=	filter through 'equalprg' or C-indenting if empty
	|gq|	gq	text formatting
	|gw|	gw	text formatting with no cursor movement
	|g?|	g?	ROT13 encoding
	|>|	>	shift right
	|<|	<	shift left
	|zf|	zf	define a fold
	|g@|	g@	call function set with the 'operatorfunc' option

	v *o_v*		When used after an operator, before the motion command: Force
		the operator to work charwise, also when the motion is
		linewise. 
	V *o_V*		When used after an operator, before the motion command: Force
		the operator to work linewise, also when the motion is
		charwise.
	CTRL-V *o_CTRL-V*		When used after an operator, before the motion command: Force
		the operator to work blockwise.
	
	h		or					*h*

<Left>		or					*<Left>*

CTRL-H		or					*CTRL-H* *<BS>*
<BS>			[count] characters to the left.  |exclusive| motion.
			Note: If you prefer <BS> to delete a character, use
			the mapping:
				:map CTRL-V<BS>		X
			(to enter "CTRL-V<BS>" type the CTRL-V key, followed
			by the <BS> key)

l		or					*l*

<Right>		or					*<Right>* *<Space>*
<Space>			[count] characters to the right.  |exclusive| motion.
			See the 'whichwrap' option for adjusting the behavior
			at end of line

							*0*
0			To the first character of the line.  |exclusive|
			motion.

							*<Home>* *<kHome>*
<Home>			To the first character of the line.  |exclusive|
			motion.  When moving up or down next, stay in same
			TEXT column (if possible).  Most other commands stay
			in the same SCREEN column.  <Home> works like "1|",
			which differs from "0" when the line starts with a
			<Tab>.

							*^*
^			To the first non-blank character of the line.
			|exclusive| motion.  Any count is ignored.

							*$* *<End>* *<kEnd>*
$  or <End>		To the end of the line.  When a count is given also go
			[count - 1] lines downward, or as far is possible.
			|inclusive| motion.  If a count of 2 or larger is
			given and the cursor is on the last line, that is an
			error and the cursor doesn't move.
			In Visual mode the cursor goes to just after the last
			character in the line.
			When 'virtualedit' is active, "$" may move the cursor
			back from past the end of the line to the last
			character in the line.

							*g_*
g_			To the last non-blank character of the line and
			[count - 1] lines downward |inclusive|.

							*g0* *g<Home>*
g0 or g<Home>		When lines wrap ('wrap' on): To the first character of
			the screen line.  |exclusive| motion.  Differs from
			"0" when a line is wider than the screen.
			When lines don't wrap ('wrap' off): To the leftmost
			character of the current line that is on the screen.
			Differs from "0" when the first character of the line
			is not on the screen.

							*g^*
g^			When lines wrap ('wrap' on): To the first non-blank
			character of the screen line.  |exclusive| motion.
			Differs from "^" when a line is wider than the screen.
			When lines don't wrap ('wrap' off): To the leftmost
			non-blank character of the current line that is on the
			screen.  Differs from "^" when the first non-blank
			character of the line is not on the screen.

							*gm*
gm			Like "g0", but half a screenwidth to the right (or as
			much as possible).

							*gM*
gM			Like "g0", but to halfway the text of the line.
			With a count: to this percentage of text in the line.
			Thus "10gM" is near the start of the text and "90gM"
			is near the end of the text.

							*g$* *g<End>*
g$ or g<End>		When lines wrap ('wrap' on): To the last character of
			the screen line and [count - 1] screen lines downward
			|inclusive|.  Differs from "$" when a line is wider
			than the screen.
			When lines don't wrap ('wrap' off): To the rightmost
			character of the current line that is visible on the
			screen.  Differs from "$" when the last character of
			the line is not on the screen or when a count is used.
			Additionally, vertical movements keep the column,
			instead of going to the end of the line.
			When 'virtualedit' is enabled moves to the end of the
			screen line.

							*bar*
|			To screen column [count] in the current line.
			|exclusive| motion.  Ceci n'est pas une pipe.

							*f*
f{char}			To [count]'th occurrence of {char} to the right.  The
			cursor is placed on {char} |inclusive|.
			{char} can be entered as a digraph |digraph-arg|.
			When 'encoding' is set to Unicode, composing
			characters may be used, see |utf-8-char-arg|.
			|:lmap| mappings apply to {char}.  The CTRL-^ command
			in Insert mode can be used to switch this on/off
			|i_CTRL-^|.

							*F*
F{char}			To the [count]'th occurrence of {char} to the left.
			The cursor is placed on {char} |exclusive|.
			{char} can be entered like with the |f| command.

							*t*
t{char}			Till before [count]'th occurrence of {char} to the
			right.  The cursor is placed on the character left of
			{char} |inclusive|.
			{char} can be entered like with the |f| command.

							*T*
T{char}			Till after [count]'th occurrence of {char} to the
			left.  The cursor is placed on the character right of
			{char} |exclusive|.
			{char} can be entered like with the |f| command.

							*;*
;			Repeat latest f, t, F or T [count] times. See |cpo-;|

							*,*
,			Repeat latest f, t, F or T in opposite direction
			[count] times. See also |cpo-;|
	
	k		or					*k*

<Up>		or					*<Up>* *CTRL-P*
CTRL-P			[count] lines upward |linewise|.

j		or					*j*

<Down>		or					*<Down>*

CTRL-J		or					*CTRL-J*

<NL>		or					*<NL>* *CTRL-N*
CTRL-N			[count] lines downward |linewise|.

gk		or					*gk* *g<Up>*
g<Up>			[count] display lines upward.  |exclusive| motion.
			Differs from 'k' when lines wrap, and when used with
			an operator, because it's not linewise.

gj		or					*gj* *g<Down>*
g<Down>			[count] display lines downward.  |exclusive| motion.
			Differs from 'j' when lines wrap, and when used with
			an operator, because it's not linewise.

							*-*
-  <minus>		[count] lines upward, on the first non-blank
			character |linewise|.

+		or					*+*

CTRL-M		or					*CTRL-M* *<CR>*
<CR>			[count] lines downward, on the first non-blank
			character |linewise|.

							*_*
_  <underscore>		[count] - 1 lines downward, on the first non-blank
			character |linewise|.

							*G*
G			Goto line [count], default last line, on the first
			non-blank character |linewise|.  If 'startofline' not
			set, keep the same column.
			G is one of the |jump-motions|.

							*<C-End>*
<C-End>			Goto line [count], default last line, on the last
			character |inclusive|.

<C-Home>	or					*gg* *<C-Home>*
gg			Goto line [count], default first line, on the first
			non-blank character |linewise|.  If 'startofline' not
			set, keep the same column.

							*:[range]*
:[range]		Set the cursor on the last line number in [range].
			[range] can also be just one line number, e.g., ":1"
			or ":'m".
			In contrast with |G| this command does not modify the
			|jumplist|.

							*N%*
{count}%		Go to {count} percentage in the file, on the first
			non-blank in the line |linewise|.  To compute the new
			line number this formula is used:
			    ({count} * number-of-lines + 99) / 100
			See also 'startofline' option.

:[range]go[to] [count]					*:go* *:goto* *go*
[count]go		Go to [count] byte in the buffer.  Default [count] is
			one, start of the file.

	<S-Right>	or					*<S-Right>* *w*
w			[count] words forward.  |exclusive| motion.

<C-Right>	or					*<C-Right>* *W*
W			[count] WORDS forward.  |exclusive| motion.

							*e*
e			Forward to the end of word [count] |inclusive|.
			Does not stop in an empty line.

							*E*
E			Forward to the end of WORD [count] |inclusive|.
			Does not stop in an empty line.

<S-Left>	or					*<S-Left>* *b*
b			[count] words backward.  |exclusive| motion.

<C-Left>	or					*<C-Left>* *B*
B			[count] WORDS backward.  |exclusive| motion.

							*ge*
ge			Backward to the end of word [count] |inclusive|.

							*gE*
gE			Backward to the end of WORD [count] |inclusive|.

							*(*
(			[count] |sentence|s backward.  |exclusive| motion.

							*)*
)			[count] |sentence|s forward.  |exclusive| motion.

							*{*
{			[count] |paragraph|s backward.  |exclusive| motion.

							*}*
}			[count] |paragraph|s forward.  |exclusive| motion.

							*]]*
]]			[count] |section|s forward or to the next '{' in the
			first column.  When used after an operator, then also
			stops below a '}' in the first column.  |exclusive|
			Note that |exclusive-linewise| often applies.

							*][*
][			[count] |section|s forward or to the next '}' in the
			first column.  |exclusive|
			Note that |exclusive-linewise| often applies.

							*[[*
[[			[count] |section|s backward or to the previous '{' in
			the first column.  |exclusive|
			Note that |exclusive-linewise| often applies.

							*[]*
[]			[count] |section|s backward or to the previous '}' in
			the first column.

	aw			"a word", select [count] words (see |word|).
			Leading or trailing white space is included, but not
			counted.
			When used in Visual linewise mode "aw" switches to
			Visual charwise mode.

							*v_iw* *iw*
iw			"inner word", select [count] words (see |word|).
			White space between words is counted too.
			When used in Visual linewise mode "iw" switches to
			Visual charwise mode.

							*v_aW* *aW*
aW			"a WORD", select [count] WORDs (see |WORD|).
			Leading or trailing white space is included, but not
			counted.
			When used in Visual linewise mode "aW" switches to
			Visual charwise mode.

							*v_iW* *iW*
iW			"inner WORD", select [count] WORDs (see |WORD|).
			White space between words is counted too.
			When used in Visual linewise mode "iW" switches to
			Visual charwise mode.

							*v_as* *as*
as			"a sentence", select [count] sentences (see
			|sentence|).
			When used in Visual mode it is made charwise.

							*v_is* *is*
is			"inner sentence", select [count] sentences (see
			|sentence|).
			When used in Visual mode it is made charwise.

							*v_ap* *ap*
ap			"a paragraph", select [count] paragraphs (see
			|paragraph|).
			Exception: a blank line (only containing white space)
			is also a paragraph boundary.
			When used in Visual mode it is made linewise.

							*v_ip* *ip*
ip			"inner paragraph", select [count] paragraphs (see
			|paragraph|).
			Exception: a blank line (only containing white space)
			is also a paragraph boundary.
			When used in Visual mode it is made linewise.

a]						*v_a]* *v_a[* *a]* *a[*
a[			"a [] block", select [count] '[' ']' blocks.  This
			goes backwards to the [count] unclosed '[', and finds
			the matching ']'.  The enclosed text is selected,
			including the '[' and ']'.
			When used in Visual mode it is made charwise.

i]						*v_i]* *v_i[* *i]* *i[*
i[			"inner [] block", select [count] '[' ']' blocks.  This
			goes backwards to the [count] unclosed '[', and finds
			the matching ']'.  The enclosed text is selected,
			excluding the '[' and ']'.
			When used in Visual mode it is made charwise.

a)							*v_a)* *a)* *a(*

a(							*vab* *v_ab* *v_a(* *ab*
ab			"a block", select [count] blocks, from "[count] [(" to
			the matching ')', including the '(' and ')' (see
			|[(|).  Does not include white space outside of the
			parenthesis.
			When used in Visual mode it is made charwise.

i)							*v_i)* *i)* *i(*

i(							*vib* *v_ib* *v_i(* *ib*
ib			"inner block", select [count] blocks, from "[count] [("
			to the matching ')', excluding the '(' and ')' (see
			|[(|).
			When used in Visual mode it is made charwise.

a>						*v_a>* *v_a<* *a>* *a<*
a<			"a <> block", select [count] <> blocks, from the
			[count]'th unmatched '<' backwards to the matching
			'>', including the '<' and '>'.
			When used in Visual mode it is made charwise.

i>						*v_i>* *v_i<* *i>* *i<*
i<			"inner <> block", select [count] <> blocks, from
			the [count]'th unmatched '<' backwards to the matching
			'>', excluding the '<' and '>'.
			When used in Visual mode it is made charwise.

						*v_at* *at*
at			"a tag block", select [count] tag blocks, from the
			[count]'th unmatched "<aaa>" backwards to the matching
			"</aaa>", including the "<aaa>" and "</aaa>".
			See |tag-blocks| about the details.
			When used in Visual mode it is made charwise.

						*v_it* *it*
it			"inner tag block", select [count] tag blocks, from the
			[count]'th unmatched "<aaa>" backwards to the matching
			"</aaa>", excluding the "<aaa>" and "</aaa>".
			See |tag-blocks| about the details.
			When used in Visual mode it is made charwise.

a}							*v_a}* *a}* *a{*

a{							*v_aB* *v_a{* *aB*
aB			"a Block", select [count] Blocks, from "[count] [{" to
			the matching '}', including the '{' and '}' (see
			|[{|).
			When used in Visual mode it is made charwise.

i}							*v_i}* *i}* *i{*

i{							*v_iB* *v_i{* *iB*
iB			"inner Block", select [count] Blocks, from "[count] [{"
			to the matching '}', excluding the '{' and '}' (see
			|[{|).
			When used in Visual mode it is made charwise.

a"							*v_aquote* *aquote*

a'							*v_a'* *a'*

a`							*v_a`* *a`*
			"a quoted string".  Selects the text from the previous
			quote until the next quote.  The 'quoteescape' option
			is used to skip escaped quotes.
			Only works within one line.
			When the cursor starts on a quote, Vim will figure out
			which quote pairs form a string by searching from the
			start of the line.
			Any trailing white space is included, unless there is
			none, then leading white space is included.
			When used in Visual mode it is made charwise.
			Repeating this object in Visual mode another string is
			included.  A count is currently not used.

i"							*v_iquote* *iquote*

i'							*v_i'* *i'*

i`							*v_i`* *i`*
			Like a", a' and a`, but exclude the quotes and
			repeating won't extend the Visual selection.

	"dl"	delete character (alias: "x")		|dl|

	"diw"	delete inner word			*diw*

	"daw"	delete a word				*daw*

	"diW"	delete inner WORD (see |WORD|)		*diW*

	"daW"	delete a WORD (see |WORD|)		*daW*

	"dgn"   delete the next search pattern match    *dgn*
	"dd"	delete one line				|dd|

	"dis"	delete inner sentence			*dis*

	"das"	delete a sentence			*das*

	"dib"	delete inner '(' ')' block		*dib*

	"dab"	delete a '(' ')' block			*dab*

	"dip"	delete inner paragraph			*dip*

	"dap"	delete a paragraph			*dap*

	"diB"	delete inner '{' '}' block		*diB*

	"daB"	delete a '{' '}' block			*daB*

	1. With ` (backtick):	  The cursor is positioned at the specified location
			  and the motion is |exclusive|.
2. With '' (single quote): The cursor is positioned on the first non-blank
			  character in the line of the specified location and
			  the motion is linewise.

						*m* *mark* *Mark*
m{a-zA-Z}		Set mark {a-zA-Z} at cursor position (does not move
			the cursor, this is not a motion command).

						*m'* *m`*
m'  or  m`		Set the previous context mark.  This can be jumped to
			with the "''"' or "``" command (does not move the
			cursor, this is not a motion command).

						*m[* *m]*
m[  or  m]		Set the |'[| or |']| mark.  Useful when an operator is
			to be simulated by multiple commands.  (does not move
			the cursor, this is not a motion command).

						*m<* *m>*
m<  or  m>		Set the |'<| or |'>| mark.  Useful to change what the
			`gv` command selects.  (does not move the cursor, this
			is not a motion command).
			Note that the Visual mode cannot be set, only the
			start and end position.

						*:ma* *:mark* *E191*
:[range]ma[rk] {a-zA-Z'}
			Set mark {a-zA-Z'} at last line number in [range],
			column 0.  Default is cursor line.

						*:k*
:[range]k{a-zA-Z'}	Same as :mark, but the space before the mark name can
			be omitted.

						*'* *'a* *`* *`a*
'{a-z}  `{a-z}		Jump to the mark {a-z} in the current buffer.

						*'A* *'0* *`A* *`0*
'{A-Z0-9}  `{A-Z0-9}	To the mark {A-Z0-9} in the file where it was set (not
			a motion command when in another file).

						*g'* *g'a* *g`* *g`a*
g'{mark}  g`{mark}
			Jump to the {mark}, but don't change the jumplist when
			jumping within the current buffer.  Example:
				g`"
 			jumps to the last known position in a file.
			See also |:keepjumps|.

						*:marks*
:marks			List all the current marks (not a motion command).
			The |'(|, |')|, |'{| and |'}| marks are not listed.
			The first column has number zero.

						*E283*
:marks {arg}		List the marks that are mentioned in {arg} (not a
			motion command).  For example:
				:marks aB
 			to list marks 'a' and 'B'.

							*:delm* *:delmarks*
:delm[arks] {marks}	Delete the specified marks.  Marks that can be deleted
			include A-Z and 0-9.  You cannot delete the '' mark.
			They can be specified by giving the list of mark
			names, or with a range, separated with a dash.  Spaces
			are ignored.  Examples:
			   :delmarks a	      deletes mark a
			   :delmarks a b 1    deletes marks a, b and 1
			   :delmarks Aa       deletes marks A and a
			   :delmarks p-z      deletes marks in the range p to z
			   :delmarks ^.[]     deletes marks ^ . [ ]
			   :delmarks \"	      deletes mark "
 
:delm[arks]!		Delete all marks for the current buffer, but not marks
			A-Z or 0-9.  Also clear the |changelist|.

	*'[* *`[*
'[  `[			To the first character of the previously changed
			or yanked text.

							*']* *`]*
']  `]			To the last character of the previously changed or
			yanked text.
	
	*'<* *`<*
'<  `<			To the first line or character of the last selected
			Visual area in the current buffer.  For block mode it
			may also be the last character in the first line (to
			be able to define the block).

							*'>* *`>*
'>  `>			To the last line or character of the last selected
			Visual area in the current buffer.  For block mode it
			may also be the first character of the last line (to
			be able to define the block).  Note that 'selection'
			applies, the position may be just after the Visual
			area.

							*''* *``*
''  ``			To the position before the latest jump, or where the
			last "m'"' or "m`" command was given.  Not set when the
			|:keepjumps| command modifier was used.
			Also see |restore-position|.

							*'quote* *`quote*
'"'  `"			To the cursor position when last exiting the current
			buffer.  Defaults to the first character of the first
			line.  See |last-position-jump| for how to use this
			for each opened file.
			Only one position is remembered per buffer, not one
			for each window.  As long as the buffer is visible in
			a window the position won't be changed.  Mark is also 
			reset when |:wshada| is run.

							*'^* *`^*
'^  `^			To the position where the cursor was the last time
			when Insert mode was stopped.  This is used by the
			|gi| command.  Not set when the |:keepjumps| command
			modifier was used.

							*'.* *`.*
'.  `.			To the position where the last change was made.  The
			position is at or near where the change started.
			Sometimes a command is executed as several changes,
			then the position can be near the end of what the
			command changed.  For example when inserting a word,
			the position will be on the last character.
			To jump to older changes use |g;|.

							*'(* *`(*
'(  `(			To the start of the current sentence, like the |(|
			command.

							*')* *`)*
')  `)			To the end of the current sentence, like the |)|
			command.

							*'{* *`{*
'{  `{			To the start of the current paragraph, like the |{|
			command.

							*'}* *`}*
'}  `}			To the end of the current paragraph, like the |}|
			command.

	*]'*
]'			[count] times to next line with a lowercase mark below
			the cursor, on the first non-blank character in the
			line.

							*]`*
]`			[count] times to lowercase mark after the cursor.

							*['*
['			[count] times to previous line with a lowercase mark
			before the cursor, on the first non-blank character in
			the line.

							*[`*
[`			[count] times to lowercase mark before the cursor.

:loc[kmarks] {command}				*:loc* *:lock* *:lockmarks*
			Execute {command} without adjusting marks.  This is
			useful when changing text in a way that the line count
			will be the same when the change has completed.
			WARNING: When the line count does change, marks below
			the change will keep their line number, thus move to
			another text line.
			These items will not be adjusted for deleted/inserted
			lines:
			- lower case letter marks 'a - 'z
			- upper case letter marks 'A - 'Z
			- numbered marks '0 - '9
			- last insert position '^
			- last change position '.
			- last affected text area '[ and ']
			- the Visual area '< and '>
			- line numbers in placed signs
			- line numbers in quickfix positions
			- positions in the |jumplist|
			- positions in the |tagstack|
			These items will still be adjusted:
			- previous context mark ''
			- the cursor position
			- the view of a window on a buffer
			- folds
			- diffs

:kee[pmarks] {command}				*:kee* *:keep* *:keepmarks*
			Currently only has effect for the filter command
			YXXY:range!|:
			- When the number of lines after filtering is equal to
			  or larger than before, all marks are kept at the
			  same line number.
			- When the number of lines decreases, the marks in the
			  lines that disappeared are deleted.
			In any case the marks below the filtered text have
			their line numbers adjusted, thus stick to the text,
			as usual.
			When the 'R' flag is missing from 'cpoptions' this has
			the same effect as using ":keepmarks".

							*:keepj* *:keepjumps*
:keepj[umps] {command}
			Moving around in {command} does not change the |''|,
			|'.| and |'^| marks, the |jumplist| or the
			|changelist|.

	*CTRL-O*
CTRL-O			Go to [count] Older cursor position in jump list
			(not a motion command).

<Tab>		or					*CTRL-I* *<Tab>*
CTRL-I			Go to [count] newer cursor position in jump list
			(not a motion command).

							*:ju* *:jumps*
:ju[mps]		Print the jump list (not a motion command).

							*:cle* *:clearjumps*
:cle[arjumps]		Clear the jump list of the current window.

	*g;* *E662*
g;			Go to [count] older position in change list.
			If [count] is larger than the number of older change
			positions go to the oldest change.
			If there is no older change an error message is given.
			(not a motion command)

							*g,* *E663*
g,			Go to [count] newer cursor position in change list.
			Just like |g;| but in the opposite direction.

	:changes		Print the change list.  A ">" character indicates the
			current position.
	
	*%*
%			Find the next item in this line after or under the
			cursor and jump to its match. |inclusive| motion.
			Items can be:
			([{}])		parenthesis or (curly/square) brackets
					(this can be changed with the
					'matchpairs' option)
			/* */		start or end of C-style comment
			#if, #ifdef, #else, #elif, #endif
					C preprocessor conditionals (when the
					cursor is on the # or no ([{
					is following)
			For other items the matchit plugin can be used, see
			|matchit|.  This plugin also helps to skip matches in
			comments.

			When 'cpoptions' contains "M" |cpo-M| backslashes
			before parens and braces are ignored.  Without "M" the
			number of backslashes matters: an even number doesn't
			match with an odd number.  Thus in "( \) )" and "\( (
			\)" the first and last parenthesis match.

			When the '%' character is not present in 'cpoptions'
			|cpo-%|, parens and braces inside double quotes are
			ignored, unless the number of parens/braces in a line
			is uneven and this line and the previous one does not
			end in a backslash.  '(', '{', '[', ']', '}' and ')'
			are also ignored (parens and braces inside single
			quotes).  Note that this works fine for C, but not for
			Perl, where single quotes are used for strings.

			Nothing special is done for matches in comments.  You
			can either use the |matchit| plugin or put quotes around
			matches.

			No count is allowed, {count}% jumps to a line {count}
			percentage down the file |N%|.  Using '%' on
			#if/#else/#endif makes the movement linewise.

						*[(*
[(			Go to [count] previous unmatched '('.
			|exclusive| motion.

						*[{*
[{			Go to [count] previous unmatched '{'.
			|exclusive| motion.

						*])*
])			Go to [count] next unmatched ')'.
			|exclusive| motion.

						*]}*
]}			Go to [count] next unmatched '}'.
			|exclusive| motion.
	
	*]m*
]m			Go to [count] next start of a method (for Java or
			similar structured language).  When not before the
			start of a method, jump to the start or end of the
			class.  When no '{' is found after the cursor, this is
			an error.  |exclusive| motion.

						*]M*
]M			Go to [count] next end of a method (for Java or
			similar structured language).  When not before the end
			of a method, jump to the start or end of the class.
			When no '}' is found after the cursor, this is an
			error. |exclusive| motion.

						*[m*
[m			Go to [count] previous start of a method (for Java or
			similar structured language).  When not after the
			start of a method, jump to the start or end of the
			class.  When no '{' is found before the cursor this is
			an error. |exclusive| motion.

						*[M*
[M			Go to [count] previous end of a method (for Java or
			similar structured language).

	*[#*
[#			Go to [count] previous unmatched "#if" or "#else".
			|exclusive| motion.

						*]#*
]#			Go to [count] next unmatched "#else" or "#endif".
			|exclusive| motion.

	*[star* *[/*
[*  or  [/		Go to [count] previous start of a C comment "/*".
			|exclusive| motion.

						*]star* *]/*
]*  or  ]/		Go to [count] next end of a C comment "*/".
			|exclusive| motion.

						*H*
H			To line [count] from top (Home) of window (default:
			first line on the window) on the first non-blank
			character |linewise|.  See also 'startofline' option.
			Cursor is adjusted for 'scrolloff' option, unless an
			operator is pending, in which case the text may
			scroll.  E.g. "yH" yanks from the first visible line
			until the cursor line (inclusive).

						*M*
M			To Middle line of window, on the first non-blank
			character |linewise|.  See also 'startofline' option.

						*L*
L			To line [count] from bottom of window (default: Last
			line on the window) on the first non-blank character
			|linewise|.  See also 'startofline' option.
			Cursor is adjusted for 'scrolloff' option, unless an
			operator is pending, in which case the text may
			scroll.  E.g. "yL" yanks from the cursor to the last
			visible line.

<LeftMouse>		Moves to the position on the screen where the mouse
			click is |exclusive|.

scroll.txt                                :           scrolling the text in the window
insert.txt                                :           insert and replace mode

### *change.txt*

["x]<Del>	or					*<Del>* *x* *dl*
["x]x			Delete [count] characters under and after the cursor
			[into register x] (not |linewise|).  Does the same as
			"dl".
			The <Del> key does not take a [count].  Instead, it
			deletes the last character of the count.
			See |'whichwrap'| for deleting a line break (join
			lines).


							*X* *dh*
["x]X			Delete [count] characters before the cursor [into
			register x] (not |linewise|).  Does the same as "dh".
			Also see |'whichwrap'|.


							*d*
["x]d{motion}		Delete text that {motion} moves over [into register
			x].  See below for exceptions.


							*dd*
["x]dd			Delete [count] lines [into register x] |linewise|.


							*D*
["x]D			Delete the characters under the cursor until the end
			of the line and [count]-1 more lines [into register
			x]; synonym for "d$".
			(not |linewise|)
			When the '#' flag is in 'cpoptions' the count is
			ignored.


{Visual}["x]x	or					*v_x* *v_d* *v_<Del>*
{Visual}["x]d   or
{Visual}["x]<Del>	Delete the highlighted text [into register x] (for
			{Visual} see |Visual-mode|).


{Visual}["x]CTRL-H   or					*v_CTRL-H* *v_<BS>*
{Visual}["x]<BS>	When in Select mode: Delete the highlighted text [into
			register x].


{Visual}["x]X	or					*v_X* *v_D* *v_b_D*
{Visual}["x]D		Delete the highlighted lines [into register x] (for
			{Visual} see |Visual-mode|).  In Visual block mode,
			"D" deletes the highlighted text plus all text until
			the end of the line.


					*:d* *:de* *:del* *:delete* *:dl* *:dp*
:[range]d[elete] [x]	Delete [range] lines (default: current line) [into
			register x].
			Note these weird abbreviations:
			   :dl		delete and list
			   :dell	idem
			   :delel	idem
			   :deletl	idem
			   :deletel	idem
			   :dp		delete and print
			   :dep		idem
			   :delp	idem
			   :delep	idem
			   :deletp	idem
			   :deletep	idem

:[range]d[elete] [x] {count}
			Delete {count} lines, starting with [range]
			(default: current line |cmdline-ranges|) [into
			register x].
	
	*J*
J			Join [count] lines, with a minimum of two lines.
			Remove the indent and insert up to two spaces (see
			below).  Fails when on the last line of the buffer.
			If [count] is too big it is reduced to the number of
			lines available.


							*v_J*
{Visual}J		Join the highlighted lines, with a minimum of two
			lines.  Remove the indent and insert up to two spaces
			(see below).


							*gJ*
gJ			Join [count] lines, with a minimum of two lines.
			Don't insert or remove any spaces.


							*v_gJ*
{Visual}gJ		Join the highlighted lines, with a minimum of two
			lines.  Don't insert or remove any spaces.


							*:j* *:join*
:[range]j[oin][!] [flags]
			Join [range] lines.  Same as "J", except with [!]
			the join does not insert or delete any spaces.
			If a [range] has equal start and end values, this
			command does nothing.  The default behavior is to
			join the current line with the line below it.
			See |ex-flags| for [flags].

:[range]j[oin][!] {count} [flags]
			Join {count} lines, starting with [range] (default:
			current line |cmdline-ranges|).

	*R*
R			Enter Replace mode: Each character you type replaces
			an existing character, starting with the character
			under the cursor.  Repeat the entered text [count]-1
			times.  See |Replace-mode| for more details.


							*gR*
gR			Enter Virtual Replace mode: Each character you type
			replaces existing characters in screen space.  So a
			<Tab> may replace several characters at once.
			Repeat the entered text [count]-1 times.  See
			|Virtual-Replace-mode| for more details.


							*c*
["x]c{motion}		Delete {motion} text [into register x] and start
			insert.  When  'cpoptions' includes the 'E' flag and
			there is no text to delete (e.g., with "cTx" when the
			cursor is just after an 'x'), an error occurs and
			insert mode does not start (this is Vi compatible).
			When  'cpoptions' does not include the 'E' flag, the
			"c" command always starts insert mode, even if there
			is no text to delete.


							*cc*
["x]cc			Delete [count] lines [into register x] and start
			insert |linewise|.  If 'autoindent' is on, preserve
			the indent of the first line.


							*C*
["x]C			Delete from the cursor position to the end of the
			line and [count]-1 more lines [into register x], and
			start insert.  Synonym for c$ (not |linewise|).


							*s*
["x]s			Delete [count] characters [into register x] and start
			insert (s stands for Substitute).  Synonym for "cl"
			(not |linewise|).


							*S*
["x]S			Delete [count] lines [into register x] and start
			insert.  Synonym for "cc" |linewise|.


{Visual}["x]c	or					*v_c* *v_s*
{Visual}["x]s		Delete the highlighted text [into register x] and
			start insert (for {Visual} see |Visual-mode|).


							*v_r*
{Visual}r{char}		Replace all selected characters by {char}.


							*v_C*
{Visual}["x]C		Delete the highlighted lines [into register x] and
			start insert.  In Visual block mode it works
			differently |v_b_C|.

							*v_S*
{Visual}["x]S		Delete the highlighted lines [into register x] and
			start insert (for {Visual} see |Visual-mode|).


							*v_R*
{Visual}["x]R		Currently just like {Visual}["x]S.  In a next version
			it might work differently.

	*:c* *:ch* *:change*
:{range}c[hange][!]	Replace lines of text with some different text.
			Type a line containing only "." to stop replacing.

	*r*
r{char}			Replace the character under the cursor with {char}.
			If {char} is a <CR> or <NL>, a line break replaces the
			character.

	*gr*
gr{char}		Replace the virtual characters under the cursor with
			{char}.

	*~*
~			'notildeop' option: Switch case of the character
			under the cursor and move the cursor to the right.
			If a [count] is given, do that many characters.

~{motion}		'tildeop' option: switch case of {motion} text.


							*g~*
g~{motion}		Switch case of {motion} text.


g~g~							*g~g~* *g~~*
g~~			Switch case of current line.


							*v_~*
{Visual}~		Switch case of highlighted text (for {Visual} see
			|Visual-mode|).


							*v_U*
{Visual}U		Make highlighted text uppercase (for {Visual} see
			|Visual-mode|).


							*gU* *uppercase*
gU{motion}		Make {motion} text uppercase.
			Example:
				:map! <C-F> <Esc>gUiw`]a
 			This works in Insert mode: press CTRL-F to make the
			word before the cursor uppercase.  Handy to type
			words in lowercase and then make them uppercase.



gUgU							*gUgU* *gUU*
gUU			Make current line uppercase.


							*v_u*
{Visual}u		Make highlighted text lowercase (for {Visual} see
			|Visual-mode|).


							*gu* *lowercase*
gu{motion}		Make {motion} text lowercase.


gugu							*gugu* *guu*
guu			Make current line lowercase.


							*g?* *rot13*
g?{motion}		Rot13 encode {motion} text.


							*v_g?*
{Visual}g?		Rot13 encode the highlighted text (for {Visual} see
			|Visual-mode|).


g?g?							*g?g?* *g??*
g??			Rot13 encode current line.

*CTRL-A*
CTRL-A			Add [count] to the number or alphabetic character at
			or after the cursor.


                                                       *v_CTRL-A*
{Visual}CTRL-A		Add [count] to the number or alphabetic character in
			the highlighted text.  {not in Vi}


							*v_g_CTRL-A*
{Visual}g CTRL-A	Add [count] to the number or alphabetic character in
			the highlighted text. If several lines are
		        highlighted, each one will be incremented by an
			additional [count] (so effectively creating a
			[count] incrementing sequence).  {not in Vi}
			For Example, if you have this list of numbers:
				1. 
				1. 
				1. 
				1. 
			Move to the second "1." and Visually select three
			lines, pressing g CTRL-A results in:
				1. 
				2. 
				3. 
				4. 


							*CTRL-X*
CTRL-X			Subtract [count] from the number or alphabetic
			character at or after the cursor.


							*v_CTRL-X*
{Visual}CTRL-X		Subtract [count] from the number or alphabetic
			character in the highlighted text.  {not in Vi}


							*v_g_CTRL-X*
{Visual}g CTRL-X	Subtract [count] from the number or alphabetic
			character in the highlighted text.

	*<*
<{motion}		Shift {motion} lines one 'shiftwidth' leftwards.

			If the 'shiftwidth' option is set to zero, the amount
			of indent is calculated at the first non-blank
			character in the line.

							*<<*
<<			Shift [count] lines one 'shiftwidth' leftwards.


							*v_<*
{Visual}[count]<	Shift the highlighted lines [count] 'shiftwidth'
			leftwards (for {Visual} see |Visual-mode|).


							*>*
 >{motion}		Shift {motion} lines one 'shiftwidth' rightwards.

			If the 'shiftwidth' option is set to zero, the amount
			of indent is calculated at the first non-blank
			character in the line.

							*>>*
 >>			Shift [count] lines one 'shiftwidth' rightwards.


							*v_>*
{Visual}[count]>	Shift the highlighted lines [count] 'shiftwidth'
			rightwards (for {Visual} see |Visual-mode|).


							*:<*
:[range]<		Shift [range] lines one 'shiftwidth' left.  Repeat '<'
			for shifting multiple 'shiftwidth's.

:[range]< {count}	Shift {count} lines one 'shiftwidth' left, starting
			with [range] (default current line |cmdline-ranges|).
			Repeat '<' for shifting multiple 'shiftwidth's.

:[range]le[ft] [indent]	left align lines in [range].  Sets the indent in the
			lines to [indent] (default 0).


							*:>*
:[range]> [flags]	Shift {count} [range] lines one 'shiftwidth' right.
			Repeat '>' for shifting multiple 'shiftwidth's.
			See |ex-flags| for [flags].

:[range]> {count} [flags]
			Shift {count} lines one 'shiftwidth' right, starting
			with [range] (default current line |cmdline-ranges|).

	*!*
!{motion}{filter}	Filter {motion} text lines through the external
			program {filter}.


							*!!*
!!{filter}		Filter [count] lines through the external program
			{filter}.


							*v_!*
{Visual}!{filter}	Filter the highlighted lines through the external
			program {filter} (for {Visual} see |Visual-mode|).


:{range}![!]{filter} [!][arg]				*:range!*
			Filter {range} lines through the external program
			{filter}.  Vim replaces the optional bangs with the
			latest given command and appends the optional [arg].
			Vim saves the output of the filter command in a
			temporary file and then reads the file into the buffer
			|tempfile|.  Vim uses the 'shellredir' option to
			redirect the filter output to the temporary file.
			However, if the 'shelltemp' option is off then pipes
			are used when possible (on Unix).
			When the 'R' flag is included in 'cpoptions' marks in
			the filtered lines are deleted, unless the
			|:keepmarks| command is used.  Example:
				:keepmarks '<,'>!sort
 			When the number of lines after filtering is less than
			before, marks in the missing lines are deleted anyway.


							*=*
={motion}		Filter {motion} lines through the external program
			given with the 'equalprg' option.  When the 'equalprg'
			option is empty (this is the default), use the
			internal formatting function |C-indenting| and
			|'lisp'|.  But when 'indentexpr' is not empty, it will
			be used instead |indent-expression|.


							*==*
==			Filter [count] lines like with ={motion}.


							*v_=*
{Visual}=		Filter the highlighted lines like with ={motion}.

*:s* *:su*
:[range]s[ubstitute]/{pattern}/{string}/[flags] [count]
			For each line in [range] replace a match of {pattern}
			with {string}.
			For the {pattern} see |pattern|.
			{string} can be a literal string, or something
			special; see |sub-replace-special|.
			When [range] and [count] are omitted, replace in the
			current line only.  When [count] is given, replace in
			[count] lines, starting with the last line in [range].
			When [range] is omitted start in the current line.

							*E939*
			[count] must be a positive number.  Also see
			|cmdline-ranges|.

			See |:s_flags| for [flags].
			The delimiter doesn't need to be /, see
			|pattern-delimiter|.

:[range]s[ubstitute] [flags] [count]

:[range]&[&][flags] [count]					*:&*
			Repeat last :substitute with same search pattern and
			substitute string, but without the same flags.  You
			may add [flags], see |:s_flags|.
			Note that after `:substitute` the '&' flag can't be
			used, it's recognized as a pattern separator.
			The space between `:substitute` and the 'c', 'g',
			'i', 'I' and 'r' flags isn't required, but in scripts
			it's a good idea to keep it to avoid confusion.
			Also see the two and three letter commands to repeat
			:substitute below |:substitute-repeat|.


:[range]~[&][flags] [count]					*:~*
			Repeat last substitute with same substitute string
			but with last used search pattern.  This is like
			`:&r`.  See |:s_flags| for [flags].


								*&*
&			Synonym for `:s` (repeat last substitute).  Note
			that the flags are not remembered, thus it might
			actually work differently.  You can use `:&&` to keep
			the flags.


								*g&*
g&			Synonym for `:%s//~/&` (repeat last substitute with
			last search pattern on all lines with the same flags).
			For example, when you first do a substitution with
			`:s/pattern/repl/flags` and then `/search` for
			something else, `g&` will do `:%s/search/repl/flags`.
			Mnemonic: global substitute.


						*:snomagic* *:sno*
:[range]sno[magic] ...	Same as `:substitute`, but always use 'nomagic'.


						*:smagic* *:sm*
:[range]sm[agic] ...	Same as `:substitute`, but always use 'magic'.


							*:s_flags*
The flags that you can use for the substitute commands:


							*:&&*
[&]	Must be the first one: Keep the flags from the previous substitute
	command.  Examples:
		:&&
		:s/this/that/&
 	Note that `:s` and `:&` don't keep the flags.

[c]	Confirm each substitution.  Vim highlights the matching string (with

	|hl-IncSearch|).  You can type:				*:s_c*
	    'y'	    to substitute this match
	    'l'	    to substitute this match and then quit ("last")
	    'n'	    to skip this match
	    <Esc>   to quit substituting
	    'a'	    to substitute this and all remaining matches
	    'q'	    to quit substituting
	    CTRL-E  to scroll the screen up
	    CTRL-Y  to scroll the screen down


							*:s_e*
[e]     When the search pattern fails, do not issue an error message and, in
	particular, continue in maps as if no error occurred.  This is most
	useful to prevent the "No match" error from breaking a mapping.  Vim
	does not suppress the following error messages, however:
		Regular expressions can't be delimited by letters
		\ should be followed by /, ? or &
		No previous substitute regular expression
		Trailing characters
		Interrupted


							*:s_g*
[g]	Replace all occurrences in the line.  Without this argument,
	replacement occurs only for the first occurrence in each line.  If the
	'gdefault' option is on, this flag is on by default and the [g]
	argument switches it off.


							*:s_i*
[i]	Ignore case for the pattern.  The 'ignorecase' and 'smartcase' options
	are not used.


							*:s_I*
[I]	Don't ignore case for the pattern.  The 'ignorecase' and 'smartcase'
	options are not used.


							*:s_n*
[n]	Report the number of matches, do not actually substitute.  The [c]
	flag is ignored.  The matches are reported as if 'report' is zero.
	Useful to |count-items|.
	If \= |sub-replace-expression| is used, the expression will be
	evaluated in the |sandbox| at every match.


[p]	Print the line containing the last substitute.  *:s_p*


[#]	Like [p] and prepend the line number.  *:s_#*


[l]	Like [p] but print the text like |:list|.  *:s_l*


							*:s_r*
[r]	Only useful in combination with `:&` or `:s` without arguments.

 &	  \&	  replaced with the whole matched pattern	     *s/\&*
 \&	   &	  replaced with &

      \0	  replaced with the whole matched pattern	   *\0* *s/\0*
      \1	  replaced with the matched pattern in the first

		  pair of ()					     *s/\1*
      \2	  replaced with the matched pattern in the second

		  pair of ()					     *s/\2*

      ..	  ..						     *s/\3*
      \9	  replaced with the matched pattern in the ninth

		  pair of ()					     *s/\9*
  ~	  \~	  replaced with the {string} of the previous

		  substitute					     *s~*

 \~	   ~	  replaced with ~				     *s/\~*

      \u	  next character made uppercase			     *s/\u*

      \U	  following characters made uppercase, until \E      *s/\U*

      \l	  next character made lowercase			     *s/\l*

      \L	  following characters made lowercase, until \E      *s/\L*

      \e	  end of \u, \U, \l and \L (NOTE: not <Esc>!)	     *s/\e*

      \E	  end of \u, \U, \l and \L			     *s/\E*
      <CR>	  split line in two at this point

		  (Type the <CR> as CTRL-V <Enter>)		     *s<CR>*

      \r	  idem						     *s/\r*
      \<CR>	  insert a carriage-return (CTRL-M)

		  (Type the <CR> as CTRL-V <Enter>)		     *s/\<CR>*
      \n	  insert a <NL> (<NUL> in the file)

		  (does NOT break the line)			     *s/\n*

      \b	  insert a <BS>					     *s/\b*

      \t	  insert a <Tab>				     *s/\t*

      \\	  insert a single backslash			     *s/\\*
      \x	  where x is any character not mentioned above:
		  Reserved for future expansion

	*:ret* *:retab* *:retab!*
:[range]ret[ab][!] [new_tabstop]
			Replace all sequences of white-space containing a
			<Tab> with new strings of white-space using the new
			tabstop value given.

	*quote*
"{register}		Use {register} for next delete, yank or put.  Use
			an uppercase character to append with delete and yank.
			Registers ".", "%", "#" and ":" only work with put.


							*:reg* *:registers*
:reg[isters]		Display the type and contents of all numbered and
			named registers.  If a register is written to for
			|:redir| it will not be listed.
			Type can be one of:
			"c"	for |characterwise| text
			"l"	for |linewise| text
			"b"	for |blockwise-visual| text


:reg[isters] {arg}	Display the contents of the numbered and named
			registers that are mentioned in {arg}.  For example:
				:reg 1a
 			to display registers '1' and 'a'.  Spaces are allowed
			in {arg}.


							*:di* *:display*
:di[splay] [arg]	Same as :registers.


							*y* *yank*
["x]y{motion}		Yank {motion} text [into register x].  When no
			characters are to be yanked (e.g., "y0" in column 1),
			this is an error when 'cpoptions' includes the 'E'
			flag.


							*yy*
["x]yy			Yank [count] lines [into register x] |linewise|.


							*Y*
["x]Y			yank [count] lines [into register x] (synonym for
			yy, |linewise|).

							*Y-default*
			Mapped to "y$" by default. |default-mappings|


							*zy*
["x]zy{motion}		Yank {motion} text [into register x].  Only differs
			from `y` when selecting a block of text, see |v_zy|.


							*v_y*
{Visual}["x]y		Yank the highlighted text [into register x] (for
			{Visual} see |Visual-mode|).


							*v_Y*
{Visual}["x]Y		Yank the highlighted lines [into register x] (for
			{Visual} see |Visual-mode|).


							*v_zy*
{Visual}["x]zy		Yank the highlighted text [into register x].  Trailing
			whitespace at the end of each line of a selected block
			won't be yanked.  Especially useful in combination
			with `zp`.  (for {Visual} see |Visual-mode|)


							*:y* *:yank* *E850*
:[range]y[ank] [x]	Yank [range] lines [into register x].

:[range]y[ank] [x] {count}
			Yank {count} lines, starting with last line number
			in [range] (default: current line |cmdline-ranges|),
			[into register x].


							*p* *put* *E353*
["x]p			Put the text [from register x] after the cursor
			[count] times.


							*P*
["x]P			Put the text [from register x] before the cursor
			[count] times.


							*<MiddleMouse>*
["x]<MiddleMouse>	Put the text from a register before the cursor [count]
			times.  Uses the "* register, unless another is
			specified.
			Leaves the cursor at the end of the new text.
			Using the mouse only works when 'mouse' contains 'n'
			or 'a'.
			If you have a scrollwheel and often accidentally paste
			text, you can use these mappings to disable the
			pasting with the middle mouse button:
				:map <MiddleMouse> <Nop>
				:imap <MiddleMouse> <Nop>
 			You might want to disable the multi-click versions
			too, see |double-click|.


							*gp*
["x]gp			Just like "p", but leave the cursor just after the new
			text.


							*gP*
["x]gP			Just like "P", but leave the cursor just after the new
			text.


							*:pu* *:put*
:[line]pu[t] [x]	Put the text [from register x] after [line] (default
			current line).  This always works |linewise|, thus
			this command can be used to put a yanked block as new
			lines.
			If no register is specified, it depends on the 'cb'
			option: If 'cb' contains "unnamedplus", paste from the
			+ register |quoteplus|.  Otherwise, if 'cb' contains
			"unnamed", paste from the * register |quotestar|.
			Otherwise, paste from the unnamed register
			|quote_quote|.
			The register can also be '=' followed by an optional
			expression.  The expression continues until the end of
			the command.  You need to escape the '|' and '"''
			characters to prevent them from terminating the
			command.  Example:
				:put ='path' . \",/test\"
 			If there is no expression after '=', Vim uses the
			previous expression.  You can see it with ":dis =".

:[line]pu[t]! [x]	Put the text [from register x] before [line] (default
			current line).


["x]]p		    or					*]p* *]<MiddleMouse>*
["x]]<MiddleMouse>	Like "p", but adjust the indent to the current line.
			Using the mouse only works when 'mouse' contains 'n'
			or 'a'.


["x][P		    or					*[P*

["x]]P		    or					*]P*

["x][p		    or					*[p* *[<MiddleMouse>*
["x][<MiddleMouse>	Like "P", but adjust the indent to the current line.
			Using the mouse only works when 'mouse' contains 'n'
			or 'a'.


["x]zp		    or					*zp* *zP*
["x]zP			Like "p" and "P", except without adding trailing spaces
			when pasting a block.

	*quote_.* *quote.* *E29*
	".	Contains the last inserted text (the same as what is inserted
		with the insert mode commands CTRL-A and CTRL-@).  Note: this
		doesn't work with CTRL-R on the command-line.  It works a bit
		differently, like inserting the text instead of putting it
		('textwidth' and other options affect what is inserted).

							*quote_%* *quote%*
	"%	Contains the name of the current file.

						*quote_:* *quote:* *E30*
	":	Contains the most recent executed command-line.  Example: Use
		"@:" to repeat the previous command-line command.

:[range]co[py] {address}				*:co* *:copy*
			Copy the lines given by [range] to below the line
			given by {address}.


							*:t*
:t			Synonym for copy.


:[range]m[ove] {address}			*:m* *:mo* *:move* *E134*
			Move the lines given by [range] to below the line
			given by {address}.

	:[range]ce[nter] [width]				*:ce* *:center*
			Center lines in [range] between [width] columns
			(default 'textwidth' or 80 when 'textwidth' is 0).


:[range]ri[ght] [width]					*:ri* *:right*
			Right-align lines in [range] at [width] columns
			(default 'textwidth' or 80 when 'textwidth' is 0).


							*:le* *:left*
:[range]le[ft] [indent]
			Left-align lines in [range].  Sets the indent in the
			lines to [indent] (default 0).


							*gq*
gq{motion}		Format the lines that {motion} moves over.
			Formatting is done with one of three methods:
			1. If 'formatexpr' is not empty the expression is
			   evaluated.  This can differ for each buffer.
			2. If 'formatprg' is not empty an external program
			   is used.
			3. Otherwise formatting is done internally.

			In the third case the 'textwidth' option controls the
			length of each formatted line (see below).
			If the 'textwidth' option is 0, the formatted line
			length is the screen width (with a maximum width of
			79).
			The 'formatoptions' option controls the type of
			formatting |fo-table|.
			The cursor is left on the first non-blank of the last
			formatted line.
			NOTE: The "Q" command formerly performed this
			function.  If you still want to use "Q" for
			formatting, use this mapping:
				:nnoremap Q gq


gqgq							*gqgq* *gqq*
gqq			Format the current line.  With a count format that
			many lines.


							*v_gq*
{Visual}gq		Format the highlighted text.  (for {Visual} see
			|Visual-mode|).


							*gw*
gw{motion}		Format the lines that {motion} moves over.  Similar to
			|gq| but puts the cursor back at the same position in
			the text.  However, 'formatprg' and 'formatexpr' are
			not used.


gwgw							*gwgw* *gww*
gww			Format the current line as with "gw".


							*v_gw*
{Visual}gw		Format the highlighted text as with "gw".  (for
			{Visual} see |Visual-mode|).


Example: To format the current paragraph use:			*gqap* 
	gqap

	*fo-t*
t	Auto-wrap text using textwidth

							*fo-c*
c	Auto-wrap comments using textwidth, inserting the current comment
	leader automatically.

							*fo-r*
r	Automatically insert the current comment leader after hitting
	<Enter> in Insert mode.

							*fo-o*
o	Automatically insert the current comment leader after hitting 'o' or
	'O' in Normal mode.  In case comment is unwanted in a specific place
	use CTRL-U to quickly delete it. |i_CTRL-U|

							*fo-q*
q	Allow formatting of comments with "gq".
	Note that formatting will not change blank lines or lines containing
	only the comment leader.  A new paragraph starts after such a line,
	or when the comment leader changes.

							*fo-w*
w	Trailing white space indicates a paragraph continues in the next line.
	A line that ends in a non-white character ends a paragraph.

							*fo-a*
a	Automatic formatting of paragraphs.  Every time text is inserted or
	deleted the paragraph will be reformatted.  See |auto-format|.
	When the 'c' flag is present this only happens for recognized
	comments.

							*fo-n*
n	When formatting text, recognize numbered lists.  This actually uses
	the 'formatlistpat' option, thus any kind of list can be used.  The
	indent of the text after the number is used for the next line.  The
	default is to find a number, optionally followed by '.', ':', ')',
	']' or '}'.  Note that 'autoindent' must be set too.  Doesn't work
	well together with "2".
	Example:
		1. the first item
		   wraps
		2. the second item

 							*fo-2*
2	When formatting text, use the indent of the second line of a paragraph
	for the rest of the paragraph, instead of the indent of the first
	line.  This supports paragraphs in which the first line has a
	different indent than the rest.  Note that 'autoindent' must be set
	too.  Example:
			first line of a paragraph
		second line of the same paragraph
		third line.
 	This also works inside comments, ignoring the comment leader.

							*fo-v*
v	Vi-compatible auto-wrapping in insert mode: Only break a line at a
	blank that you have entered during the current insert command.  (Note:
	this is not 100% Vi compatible.  Vi has some "unexpected features" or
	bugs in this area.  It uses the screen column instead of the line
	column.)

							*fo-b*
b	Like 'v', but only auto-wrap if you enter a blank at or before
	the wrap margin.  If the line was longer than 'textwidth' when you
	started the insert, or you do not enter a blank in the insert before
	reaching 'textwidth', Vim does not perform auto-wrapping.

							*fo-l*
l	Long lines are not broken in insert mode: When a line was longer than
	'textwidth' when the insert command started, Vim does not
	automatically format it.

							*fo-m*
m	Also break at a multibyte character above 255.  This is useful for
	Asian text where every character is a word on its own.

							*fo-M*
M	When joining lines, don't insert a space before or after a multibyte
	character.  Overrules the 'B' flag.

							*fo-B*
B	When joining lines, don't insert a space between two multibyte
	characters.  Overruled by the 'M' flag.

							*fo-1*
1	Don't break a line after a one-letter word.  It's broken before it
	instead (if possible).

							*fo-]*
]	Respect textwidth rigorously. With this flag set, no line can be
	longer than textwidth, unless line-break-prohibition rules make this
	impossible.  Mainly for CJK scripts and works only if 'encoding' is
	"utf-8".

							*fo-j*
j	Where it makes sense, remove a comment leader when joining lines.  For
	example, joining:
		int i;   // the index 
		         // in the list 
	Becomes:
		int i;   // the index in the list 

							*fo-p*
p	Don't break lines at single spaces that follow periods.  This is
	intended to complement 'joinspaces' and |cpo-J|, for prose with
	sentences separated by two spaces.

	*:sor* *:sort*
:[range]sor[t][!] [b][f][i][l][n][o][r][u][x] [/{pattern}/]
			Sort lines in [range].  When no range is given all
			lines are sorted.

undo.txt                                  :          undo and rendo
repeat.txt                                :          repeating commands, Vim scripts and debugging
visual.txt                                :          using the Visual mode (selecting a text area)

### Various vommands *various-cmd* various.txt

```<C-l>```                                                           :    clears and redraws the screen. The redraw may happen later, after processing typeahead.
```:mod[e]```                                                         :    clears and redraws the screen.
```:redr[aw][!]```                                                    :    redraws pending screen updates now, or the entire screen if "!" is included.
```:redraws[tatus][!]```                                              :    redraws the status line of the current windows, or all status lines if "!" is included.
```:redrawt[abline]```                                                :    redraws the tabline. Useful to update the tabline when 'tabline' includes an item that doesn't trigger automatic updating.
```<Del>```                                                           :    when entering a number: remove the last digit.
```:as[cii], ga```                                                    :    print the ascii value of the character under the cursor in decimal, hexadecimal and octal.
```g8```                                                              :    print the hex values of the bytes used in the character under the cursor, assuming it is in |UTF-8| encoding.
```8g8```                                                             :    find an illegal UTF-8 byte sequence at or after the cursor.
```:[range]p[rint] [flags]```                                         :    print [range] lines (default current line).
```:[range]p[rint] {count} [flags]```                                 :    print {count} lines, starting with [range] (default current line |cmdline-ranges|).
```:[range]l[ist] [count] [flags]```                                  :    same as :print, but show tabs as ">", trailing spaces as "-", and non-breakable spaces as "-", and non-breakable space character as "+" by default.
```:[range]nu[mber] [count] [flags]```                                :    same as :print, but precend each line with its line number.
```:[range]# [count] [flags]```                                       :    synonym for :number.
```:#!{anything}```                                                   :    ignored, so that you can start a Vim script with.
```:[range]z[+-^.=][count]```                                         :    display several lines of text surrounding the line specified with [range], or around the current line if there is no [range].
```:[range]z![+-^.=][count]```                                        :    like ":z", but when [count] is not specified, it defaults to the Vim window height minus one.
```:[range]z[!]#[+-^.=][count]```                                     :    like ":z" or ":z!", but number the lines.
```:= [flags]```                                                      :    print the last line number.
```:{range}= [flags]```                                               :    prints the last line number in {range}.
```:norm[al][!] {commands}```                                         :    execute Normal mode commands {commands}.
```{range}norm[al][!] {commands}```                                   :    execute Normal mode commands {commands} for each line in the {range}.
```:sh[ell]```                                                        :    removed.
```:te[rminal][!] [{cmd}]```                                          :    run {cmd} in a non-interactive 'shell' in a new |terminal-emulator| buffer.
```:!{cmd}```                                                         :    execute {cmd} with 'shell'.
```:!!```                                                             :    repeat last ":!{cmd}".
```:ve[rsion]```                                                      :    print editor version and build information.
```:redi[r][!] > {file}```                                            :    redirect messages to file {file}.
```:redi[r] >> {file}```                                              :    redirect messages to file {file}.
```:redi[r] @{a-zA-Z}, :redi[r] @{a-zA-Z}>```                         :    redirect messages to register {a-z}.
```:redi[r] @{a-z}>>```                                               :    append messages to register {a-z}.
```:redi[r] @*>, :redi[r] @+>```                                      :    redirect messages to the selection or clipboard.
```:redi[r] @*>>, :redi[r] @+>>```                                    :    append messages to the selection or clipboard.
```:redi[r] @">```                                                    :    redirect messages to the unnamed register.
```:redi[r] @">>```                                                   :    append messages to the unnamed register.
```:redi[r] => {var}```                                               :    redirect messages to a variable.
```:redi[r] =>> {var}```                                              :    append messages to an existing variable.
```:redi[r] END```                                                    :    end redirecting messages.
```:filt[er][!] {pat} {command}, :filt[er][!] /{pat}/ {command}```    :    restrict the output of {command} to lines matching with {pat}.
```:sil[ent][!] {command}```                                          :    execute {commands} silently.
```:uns[ilent] {command}```                                           :    execute {command} not silently.
```:[count]verb[ose] {commands}```                                    :    execute {command} with 'verbose' set to [count].

```[count]K```                                                        :    runs the program given by 'keywordprg' to lookup the |word| (defined by 'iskeyword') under or right of the cursor.
```{Visual}K```                                                       :    like "K", but use the visually highlihgted text for the keyword.
```g0```                                                              :    show a filetype-specific, navigable "outline" of the current buffer.
```[N]gs, :[N]sl[eep] [N][m]```                                       :    do nothing for [N] milliseconds if [m] was given.
```:[N]sl[eep]! [N][m]                                                :    same as above.

recover.txt                              :          recovering from a crash
cmdline.txt                             :          Command-line editing

### Options *options* options.txt

```:se[t]```                                                          :    show all options that differ from their default value.
```:se[t] all```                                                      :    show all options.
```:se[t] {option}?```                                                :    show value of {option}.
```:se[t] {option}```                                                 :    toggle option: set, switch it on.
```:se[t] no{option}```                                               :    toggle option: reset, switch it off.
```:se[t] {option}!, :se[t] inv{option}```                            :    toggle option: invert value.
```:se[t] {option}&```                                                :    reset option to its default value.
```:se[t] {option}&vi```                                              :    reset option to its Vi default value.
```:se[t] {option}&vim```                                             :    reset option to its Vim default value.
```:se[t] all&```                                                     :    set all options to their default value.
```:se[t] {option}={value}, :se[t] {option}:{value}```                :    set string or number option to {value}.
```:se[t] {option}+={value}```                                        :    add the {value} to a number option, or append the {value} to a string option.
```:se[t] {option}^={value}```                                        :    multiply the {value} to a number options, or prepend the {value} to a string option.
```:se[t] {option}-={value}```                                        :    subtract the {value} from a number option, or remove the {value} from a string option, if it is there.
```:setl[ocal]```                                                     :    like ":set" but set only the value local to the current buffer or window.
```:setl[ocal] {option}<```                                           :    set the local value of {option} to its global value by copying the value.
```:se[t] {option}<```                                                :    for |global-local| options: remove the local value of {option}, so that the global value will be used.
```:setg[lobal]```                                                    :    like ":set" but set only the global value for a local option without changing the local value.
```:setf[iletype] [FALLBACK] {filetype}```                            :    set the 'filetype' option to {filetype}, but only if not done yet in a sequence of (nested) autocommands.
```:bro[wse] se[t] :opt[ions]```                                      :    open a window for viewing and setting all options.

```'aleph', 'al'```                                                   :    number (default 224) global. The ASCII code for the first letter of the Hebrew  alphabet.
```'allowrevins', 'ari'```                                            :    boolean (default off) global. Allow CTRL-_ in Insert and Command-line mode.
```'ambiwidth', 'ambw'```                                             :    string (default: "single") global. Tells Vim what to do with characters with East Asian Width Class Ambiguous (such as Euro, Registred Sign, Copyright Sign, Greek letters, Cyrillic letters).
```'autochdir', 'acd'```                                              :    boolean (default off) global. When on, Vim will change the current working directory whenever you open a file, switch buffers, delete a buffer or open/close a window.
```'arabic', 'arab'```                                                :    boolean (default off) local to window. This option can be set to start editing Arabic text.
'arabicshape' 'arshape'	boolean (default on)
			global
	When on and 'termbidi' is off, the required visual character
	corrections that need to take place for displaying the Arabic language
	take effect.
    'autoindent' 'ai'	boolean	(default on)
			local to buffer
	Copy indent from current line when starting a new line (typing <CR>
	in Insert mode or when using the "o" or "O" command).
    'autoread' 'ar'		boolean	(default on)
			global or local to buffer |global-local|
	When a file has been detected to have been changed outside of Vim and
	it has not been changed inside of Vim, automatically read it again.
    'autowrite' 'aw'	boolean	(default off)
			global
	Write the contents of the file, if it has been modified, on each
	`:next`, `:rewind`, `:last`, `:first`, `:previous`, `:stop`,
	`:suspend`, `:tag`, `:!`, `:make`, CTRL-] and CTRL-^ command; and when
	a `:buffer`, CTRL-O, CTRL-I, '{A-Z0-9}, or `{A-Z0-9} command takes one
	to another file.
    'autowriteall' 'awa'	boolean	(default off)
			global
	Like 'autowrite', but also used for commands ":edit", ":enew", ":quit",
	":qall", ":exit", ":xit", ":recover" and closing the Vim window.
    'background' 'bg'	string	(default "dark")
			global
	When set to "dark" or "light", adjusts the default color groups for
	that background type.
    'backspace' 'bs'	string	(default "indent,eol,start")
			global
	Influences the working of <BS>, <Del>, CTRL-W and CTRL-U in Insert
	mode.
    'backup' 'bk'		boolean	(default off)
			global
	Make a backup before overwriting a file.  Leave it around after the
	file has been successfully written.
    'backupcopy' 'bkc'	string	(Vi default for Unix: "yes", otherwise: "auto")
			global or local to buffer |global-local|
	When writing a file and a backup is made, this option tells how it's
	done.
    'backupcopy' 'bkc'	string	(Vi default for Unix: "yes", otherwise: "auto")
			global or local to buffer |global-local|
	When writing a file and a backup is made, this option tells how it's
	done.
    'backupext' 'bex'	string	(default "~")
			global
	String which is appended to a file name to make the name of the
	backup file.
    'backupext' 'bex'	string	(default "~")
			global
	String which is appended to a file name to make the name of the
	backup file.
    'binary' 'bin'		boolean	(default off)
			local to buffer
	This option should be set before editing a binary file.
    'bomb'			boolean	(default off)
			local to buffer
	When writing a file and the following conditions are met, a BOM (Byte
	Order Mark) is prepended to the file
    'bomb'			boolean	(default off)
			local to buffer
	When writing a file and the following conditions are met, a BOM (Byte
	Order Mark) is prepended to the file
    'breakindent' 'bri'	boolean (default off)
			local to window
	Every wrapped line will continue visually indented (same amount of
	space as the beginning of that line), thus preserving horizontal blocks
	of text.
    'breakindentopt' 'briopt' string (default empty)
			local to window
	Settings for 'breakindent'.
    'browsedir' 'bsdir'	string	(default: "last")
			global
	Which directory to use for the file browser
    'bufhidden' 'bh'	string (default: "")
			local to buffer
	This option specifies what happens when a buffer is no longer
	displayed in a window
    'buflisted' 'bl'	boolean (default: on)
			local to buffer
	When this option is set, the buffer shows up in the buffer list.
    'buflisted' 'bl'	boolean (default: on)
			local to buffer
	When this option is set, the buffer shows up in the buffer list.
    'casemap' 'cmp'		string	(default: "internal,keepascii")
			global
	Specifies details about changing the case of letters.  It may contain
	these words, separated by a comma
    'cdhome' 'cdh'		boolean	(default: off)
			global
	When on, |:cd|, |:tcd| and |:lcd| without an argument changes the
	current working directory to the |$HOME| directory like in Unix.
    'cdpath' 'cd'		string	(default: equivalent to $CDPATH or ",,")
			global
	This is a list of directories which will be searched when using the
	|:cd|, |:tcd| and |:lcd| commands, provided that the directory being
	searched for has a relative path, not an absolute part starting with
	"/", "./" or "../", the 'cdpath' option is not used then.
    'cdpath' 'cd'		string	(default: equivalent to $CDPATH or ",,")
			global
	This is a list of directories which will be searched when using the
	|:cd|, |:tcd| and |:lcd| commands, provided that the directory being
	searched for has a relative path, not an absolute part starting with
	"/", "./" or "../", the 'cdpath' option is not used then.
    'channel'		number (default: 0)
			local to buffer
	|channel| connected to the buffer, or 0 if no channel is connected.
    'channel'		number (default: 0)
			local to buffer
	|channel| connected to the buffer, or 0 if no channel is connected.
    'cindent' 'cin'		boolean	(default off)
			local to buffer
	Enables automatic C program indenting.  See 'cinkeys' to set the keys
	that trigger reindenting in insert mode and 'cinoptions' to set your
	preferred indent style.
    'cinkeys' 'cink'	string	(default "0{,0},0),0],:,0#,!^F,o,O,e")
			local to buffer
	A list of keys that, when typed in Insert mode, cause reindenting of
	the current line.
    'cinkeys' 'cink'	string	(default "0{,0},0),0],:,0#,!^F,o,O,e")
			local to buffer
	A list of keys that, when typed in Insert mode, cause reindenting of
	the current line.
    'cinkeys' 'cink'	string	(default "0{,0},0),0],:,0#,!^F,o,O,e")
			local to buffer
	A list of keys that, when typed in Insert mode, cause reindenting of
	the current line.
    'cinoptions' 'cino'	string	(default "")
			local to buffer
	The 'cinoptions' affect the way 'cindent' reindents lines in a C
	program.
    'cinoptions' 'cino'	string	(default "")
			local to buffer
	The 'cinoptions' affect the way 'cindent' reindents lines in a C
	program.
    'cinwords' 'cinw'	string	(default "if,else,while,do,for,switch")
			local to buffer
	These keywords start an extra indent in the next line when
	'smartindent' or 'cindent' is set.
    'cmdheight' 'ch'	number	(default 1)
			global
	Number of screen lines to use for the command-line.  Helps avoiding
	|hit-enter| prompts.
    'cmdwinheight' 'cwh'	number	(default 7)
			global
	Number of screen lines to use for the command-line window. |cmdwin|
    'cmdwinheight' 'cwh'	number	(default 7)
			global
	Number of screen lines to use for the command-line window. |cmdwin|
    'columns' 'co'		number	(default 80 or terminal width)
			global
	Number of columns of the screen.

    'comments' 'com'	string	(default
				"s1:/*,mb:*,ex:*/,://,b:#,:%,:XCOMM,n:>,fb:-")
			local to buffer
	A comma separated list of strings that can start a comment line.
    'commentstring' 'cms'	string	(default "/*%s*/")
			local to buffer
	A template for a comment.
    'complete' 'cpt'	string	(default: ".,w,b,u,t")
			local to buffer
	This option specifies how keyword completion |ins-completion| works
	when CTRL-P or CTRL-N are used.
    'complete' 'cpt'	string	(default: ".,w,b,u,t")
			local to buffer
	This option specifies how keyword completion |ins-completion| works
	when CTRL-P or CTRL-N are used.
    'completeslash' 'csl'	string	(default: "")
			local to buffer
			{only for MS-Windows}
	When this option is set it overrules 'shellslash' for completion
    'completeslash' 'csl'	string	(default: "")
			local to buffer
			{only for MS-Windows}
	When this option is set it overrules 'shellslash' for completion
    'completeslash' 'csl'	string	(default: "")
			local to buffer
			{only for MS-Windows}
	When this option is set it overrules 'shellslash' for completion
    'completeslash' 'csl'	string	(default: "")
			local to buffer
			{only for MS-Windows}
	When this option is set it overrules 'shellslash' for completion
    'confirm' 'cf'		boolean (default off)
			global
	When 'confirm' is on, certain operations that would normally
	fail because of unsaved changes to a buffer, e.g.
    'copyindent' 'ci'	boolean	(default off)
			local to buffer
	Copy the structure of the existing lines indent when autoindenting a
	new line.
    'cpoptions' 'cpo'	string	(Vim default: "aABceFs_",
				 Vi default: all flags)
			global
	A sequence of single character flags.
    'cscopepathcomp' 'cspc'	number	(default 0)
			global
	Determines how many components of the path to show in a list of tags.
	See |cscopepathcomp|.
    'cscopepathcomp' 'cspc'	number	(default 0)
			global
	Determines how many components of the path to show in a list of tags.
	See |cscopepathcomp|.
    'cscopequickfix' 'csqf' string	(default "")
			global
	Specifies whether to use quickfix window to show cscope results.
    'cscoperelative' 'csre' boolean (default off)
			global
	In the absence of a prefix (-P) for cscope.
    'cscoperelative' 'csre' boolean (default off)
			global
	In the absence of a prefix (-P) for cscope.
    'cscopetag' 'cst'	boolean (default off)
			global
	Use cscope for tag commands.  See |cscope-options|.
    'cscopetagorder' 'csto'	number	(default 0)
			global
	Determines the order in which ":cstag" performs a search.
    'cursorbind' 'crb'	boolean  (default off)
			local to window
	When this option is set, as the cursor in the current
	window moves other cursorbound windows (windows that also have
	this option set) move their cursors to the corresponding line and
	column.
    'cursorcolumn' 'cuc'	boolean	(default off)
			local to window
	Highlight the screen column of the cursor with CursorColumn
	|hl-CursorColumn|
'cursorline' 'cul'	boolean	(default off)
			local to window
	Highlight the text line of the cursor with CursorLine |hl-CursorLine|.
'cursorlineopt' 'culopt' string (default: "number,line")
			local to window
	Comma separated list of settings for how 'cursorline' is displayed.
    'debug'			string	(default "")
			global
	These values can be used
    'define' 'def'		string	(default "^\s*#\s*define")
			global or local to buffer |global-local|
	Pattern to be used to find a macro definition.
'dictionary' 'dict'	string	(default "")
			global or local to buffer |global-local|
	List of file names, separated by commas, that are used to lookup words
	for keyword completion commands |i_CTRL-X_CTRL-K|.
    'diff'			boolean	(default off)
			local to window
	Join the current window in the group of windows that shows differences
	between files.  See |diff-mode|.
    'diffexpr' 'dex'	string	(default "")
			global
	Expression which is evaluated to obtain a diff file (either ed-style
	or unified-style) from two versions of a file.
    'diffopt' 'dip'		string	(default "internal,filler,closeoff")
			global
	Option settings for diff mode.
    'digraph' 'dg'		boolean	(default off)
			global
	Enable the entering of digraphs in Insert mode with {char1} <BS>
	{char2}.  See |digraphs|.
    'directory' 'dir'	string	(default "$XDG_DATA_HOME/nvim/swap//")
			global
	List of directory names for the swap file, separated with commas.
    'display' 'dy'		string	(default "lastline,msgsep", Vi default: "")
			global
	Change the way text is displayed.  This is comma separated list of
	flags
    'eadirection' 'ead'	string	(default "both")
			global
	Tells when the 'equalalways' option applies
    'emoji' 'emo'	boolean (default: on)
			global
	When on all Unicode emoji characters are considered to be full width.
    'encoding' 'enc'
	String-encoding used internally and for |RPC| communication.
	Always UTF-8.
    'endofline' 'eol'	boolean	(default on)
			local to buffer
	When writing a file and this option is off and the 'binary' option
	is on, or 'fixeol' option is off, no <EOL> will be written for the
	last line in the file.
    'equalalways' 'ea'	boolean	(default on)
			global
	When on, all the windows are automatically made the same size after
	splitting or closing a window.
    'equalalways' 'ea'	boolean	(default on)
			global
	When on, all the windows are automatically made the same size after
	splitting or closing a window.
    
'equalprg' 'ep'		string	(default "")
			global or local to buffer |global-local|
	External program to use for "=" command.
    'errorbells' 'eb'	boolean	(default off)
			global
	Ring the bell (beep or screen flash) for error messages.  This only
	makes a difference for error messages, the bell will be used always
	for a lot of errors without a message (e.g., hitting <Esc> in Normal
	mode).
    'errorfile' 'ef'	string	(default: "errors.err")
			global
	Name of the errorfile for the QuickFix mode (see |:cf|).
	When the "-q" command-line argument is used, 'errorfile' is set to the
	following argument.  Se
    'errorformat' 'efm'	string	(default is very long)
			global or local to buffer |global-local|
	Scanf-like description of the format for the lines in the error file
	(see |errorformat|).
    'eventignore' 'ei'	string	(default "")
			global
	A list of autocommand event names, which are to be ignored.
    'expandtab' 'et'	boolean	(default off)
			local to buffer
	In Insert mode: Use the appropriate number of spaces to insert a
	<Tab>. 
    'fileencoding' 'fenc'	string (default: "")
			local to buffer
	File-content encoding for the current buffer. Conversion is done with
	iconv() or as specified with 'charconvert'.
    'fileencodings' 'fencs'	string (default: "ucs-bom,utf-8,default,latin1")
			global
	This is a list of character encodings considered when starting to edit
	an existing file. 
    'fileformat' 'ff'	string (Windows default: "dos",
				Unix default: "unix")
			local to buffer
	This gives the <EOL> of the current buffer, which is used for
	reading/writing the buffer from/to a file
    'fileformats' 'ffs'	string (default:
				Vim+Vi	Win32: "dos,unix",
				Vim	Unix: "unix,dos",
				Vi	others: "")
			global
	This gives the end-of-line (<EOL>) formats that will be tried when
	starting to edit a new buffer and when reading a file into an existing
	buffer
    'fileignorecase' 'fic'	boolean	(default on for systems where case in file
				 names is normally ignored)
			global
	When set case is ignored when using file names and directories.
	See 'wildignorecase' for only ignoring case when doing completion.
    'filetype' 'ft'		string (default: "")
			local to buffer
	When this option is set, the FileType autocommand event is triggered.
    'fillchars' 'fcs'	string	(default "")
			global or local to window |global-local|
	Characters to fill the statuslines and vertical separators.
    'fixendofline' 'fixeol'	boolean	(default on)
			local to buffer
	When writing a file and this option is on, <EOL> at the end of file
	will be restored if missing.
    'foldclose' 'fcl'	string (default "")
			global
	When set to "all", a fold is closed when the cursor isn't in it and
	its level is higher than 'foldlevel'.
    'foldcolumn' 'fdc'	string (default "0")
			local to window
	When and how to draw the foldcolumn. Valid values are
    'foldenable' 'fen'	boolean (default on)
			local to window
	When off, all folds are open.
    'foldexpr' 'fde'	string (default: "0")
			local to window
	The expression used for when 'foldmethod' is "expr".
    'foldignore' 'fdi'	string (default: "#")
			local to window
	Used only when 'foldmethod' is "indent".
    'foldlevel' 'fdl'	number (default: 0)
			local to window
	Sets the fold level: Folds with a higher level will be closed.
    'foldlevelstart' 'fdls'	number (default: -1)
			global
	Sets 'foldlevel' when starting to edit another buffer in a window.
    'foldmarker' 'fmr'	string (default: "{{{,}}}")
			local to window
	The start and end marker used when 'foldmethod' is "marker". 
    'foldmethod' 'fdm'	string (default: "manual")
			local to window
	The kind of folding used for the current window.
    'foldminlines' 'fml'	number (default: 1)
			local to window
	Sets the number of screen lines above which a fold can be displayed
	closed.
    'foldnestmax' 'fdn'	number (default: 20)
			local to window
	Sets the maximum nesting of folds for the "indent" and "syntax"
	methods.
    'foldopen' 'fdo'	string (default: "block,hor,mark,percent,quickfix,
							     search,tag,undo")
			global
	Specifies for which type of commands folds will be opened, if the
	command moves the cursor into a closed fold.
    'foldtext' 'fdt'	string (default: "foldtext()")
			local to window
	An expression which is used to specify the text displayed for a closed
	fold.
    'formatexpr' 'fex'	string (default "")
			local to buffer
	Expression which is evaluated to format a range of lines for the |gq|
	operator or automatic formatting (see 'formatoptions').
    'formatlistpat' 'flp'	string (default: "^\s*\d\+[\]:.)}\t ]\s*")
			local to buffer
	A pattern that is used to recognize a list header.  This is used for
	the "n" flag in 'formatoptions'.
    'formatoptions' 'fo'	string (default: "tcqj", Vi default: "vt")
			local to buffer
	This is a sequence of letters which describes how automatic
	formatting is to be done.
    'formatprg' 'fp'	string (default "")
			global or local to buffer |global-local|
	The name of an external program that will be used to format the lines
	selected with the |gq| operator.  
    'fsync' 'fs'		boolean	(default off)
			global
	When on, the OS function fsync() will be called after saving a file
	(|:write|, |writefile()|, …), |swap-file| and |shada-file|.
    'gdefault' 'gd'		boolean	(default off)
			global
	When on, the ":substitute" flag 'g' is default on. 
    'grepformat' 'gfm'	string	(default "%f:%l:%m,%f:%l%m,%f  %l%m")
			global
	Format to recognize for the ":grep" command output.
    'grepprg' 'gp'		string	(default "grep -n ",
				 Unix: "grep -n $* /dev/null")
			global or local to buffer |global-local|
	Program to use for the |:grep| command. 
    'guicursor' 'gcr'	string	(default "n-v-c-sm:block,i-ci-ve:ver25,r-cr-o:hor20")
			global
	Configures the cursor style for each mode. Works in the GUI and many
	terminals.  See |tui-cursor-shape|.
    'guifont' 'gfn'		string	(default "")
			global
	This is a list of fonts which will be used for the GUI version of Vim.
    'guifontwide' 'gfw'	string	(default "")
			global
	Comma-separated list of fonts to be used for double-width characters.
    'guioptions' 'go'	string	(default "egmrLT"   (MS-Windows))
			global
	This option only has an effect in the GUI version of Vim.
    'guitablabel' 'gtl'	string	(default empty)
			global
	When nonempty describes the text to use in a label of the GUI tab
	pages line. 
    'guitabtooltip' 'gtt'	string	(default empty)
			global
	When nonempty describes the text to use in a tooltip for the GUI tab
	pages line. 
    'helpfile' 'hf'		string	(default (MS-Windows) "$VIMRUNTIME\doc\help.txt"
					 (others) "$VIMRUNTIME/doc/help.txt")
			global
	Name of the main help file. 
    'helpheight' 'hh'	number	(default 20)
			global
	Minimal initial height of the help window when it is opened with the
	":help" command. 
    'helplang' 'hlg'	string	(default: messages language or empty)
			global
	Comma separated list of languages.
    'hidden' 'hid'		boolean	(default on)
			global
	When off a buffer is unloaded (including loss of undo information)
	when it is |abandon|ed. 
    'history' 'hi'		number	(Vim default: 10000, Vi default: 0)
			global
	A history of ":" commands, and a history of previous search patterns
	is remembered. 
    'hkmap' 'hk'		boolean (default off)
			global
	When on, the keyboard is mapped for the Hebrew character set.
    'hkmapp' 'hkp'		boolean (default off)
			global
	When on, phonetic keyboard mapping is used.  'hkmap' must also be on.
    'hlsearch' 'hls'	boolean	(default on)
			global
	When there is a previous search pattern, highlight all its matches.
    'icon'			boolean	(default off, on when title can be restored)
			global
	When on, the icon text of the window will be set to the value of
	'iconstring' (if it is not empty), or to the name of the file
	currently being edited.
    'iconstring'		string	(default "")
			global
	When this option is not empty, it will be used for the icon text of
	the window. 
    'ignorecase' 'ic'	boolean	(default off)
			global
	Ignore case in search patterns.  Also used when searching in the tags
	file.
    'imcmdline' 'imc'	boolean (default off)
			global
	When set the Input Method is always on when starting to edit a command
	line, unless entering a search pattern (see 'imsearch' for that).
    'imdisable' 'imd'	boolean (default off, on for some systems (SGI))
			global
	When set the Input Method is never used.  This is useful to disable
	the IM when it doesn't work properly.
    'iminsert' 'imi'	number (default 0)
			local to buffer
	Specifies whether :lmap or an Input Method (IM) is to be used in
	Insert mode.  Valid values
    'imsearch' 'ims'	number (default -1)
			local to buffer
	Specifies whether :lmap or an Input Method (IM) is to be used when
	entering a search pattern.  Valid values
    'inccommand' 'icm'	string	(default "nosplit")
			global

	When nonempty, shows the effects of |:substitute|, |:smagic|, and
	|:snomagic| as you type.
    'include' 'inc'		string	(default "^\s*#\s*include")
			global or local to buffer |global-local|
	Pattern to be used to find an include command.  It is a search
	pattern, just like for the "/" command (See |pattern|).
    'include' 'inc'		string	(default "^\s*#\s*include")
			global or local to buffer |global-local|
	Pattern to be used to find an include command.  It is a search
	pattern, just like for the "/" command (See |pattern|).
    'includeexpr' 'inex'	string	(default "")
			local to buffer
	Expression to be used to transform the string found with the 'include'
	option to a file name.
    'includeexpr' 'inex'	string	(default "")
			local to buffer
	Expression to be used to transform the string found with the 'include'
	option to a file name.
    'indentkeys' 'indk'	string	(default "0{,0},0),0],:,0#,!^F,o,O,e")
			local to buffer
	A list of keys that, when typed in Insert mode, cause reindenting of
	the current line.  Only happens if 'indentexpr' isn't empty.
    'infercase' 'inf'	boolean	(default off)
			local to buffer
	When doing keyword completion in insert mode |ins-completion|, and
	'ignorecase' is also on, the case of the match is adjusted depending
	on the typed text.
    'infercase' 'inf'	boolean	(default off)
			local to buffer
	When doing keyword completion in insert mode |ins-completion|, and
	'ignorecase' is also on, the case of the match is adjusted depending
	on the typed text.
    'isfname' 'isf'		string	(default for Windows:
			     "@,48-57,/,\,.,-,_,+,,,#,$,%,{,},[,],:,@-@,!,~,="
			    otherwise: "@,48-57,/,.,-,_,+,,,#,$,%,~,=")
			global
	The characters specified by this option are included in file names and
	path names.
    'isfname' 'isf'		string	(default for Windows:
			     "@,48-57,/,\,.,-,_,+,,,#,$,%,{,},[,],:,@-@,!,~,="
			    otherwise: "@,48-57,/,.,-,_,+,,,#,$,%,~,=")
			global
	The characters specified by this option are included in file names and
	path names.
    'iskeyword' 'isk'	string (default: @,48-57,_,192-255
				Vi default: @,48-57,_)
			local to buffer
	Keywords are used in searching and recognizing with many commands:
	"w", "*", "[i", etc.  It is also used for "\k" in a |pattern|.
    'iskeyword' 'isk'	string (default: @,48-57,_,192-255
				Vi default: @,48-57,_)
			local to buffer
	Keywords are used in searching and recognizing with many commands:
	"w", "*", "[i", etc.  It is also used for "\k" in a |pattern|.
    'iskeyword' 'isk'	string (default: @,48-57,_,192-255
				Vi default: @,48-57,_)
			local to buffer
	Keywords are used in searching and recognizing with many commands:
	"w", "*", "[i", etc.  It is also used for "\k" in a |pattern|.
    'joinspaces' 'js'	boolean	(default off)
			global
	Insert two spaces after a '.', '?' and '!' with a join command.
	Otherwise only one space is inserted.
    'joinspaces' 'js'	boolean	(default off)
			global
	Insert two spaces after a '.', '?' and '!' with a join command.
	Otherwise only one space is inserted.
    'keymodel' 'km'		string	(default "")
			global
	List of comma separated words, which enable special things that keys
	can do.
    'keywordprg' 'kp'	string	(default ":Man", Windows: ":help")
			global or local to buffer |global-local|
	Program to use for the |K| command.
    'langmap' 'lmap'	string	(default "")
			global
	This option allows switching your keyboard into a special language
	mode.
    'langmap' 'lmap'	string	(default "")
			global
	This option allows switching your keyboard into a special language
	mode.
    'langmenu' 'lm'		string	(default "")
			global
	Language to use for menu translation.
'langremap' 'lrm'	boolean (default off)
			global
	When off, setting 'langmap' does not apply to characters resulting from
	a mapping.
'laststatus' 'ls'	number	(default 2)
			global
	The value of this option influences when the last window will have a
	status line
    'lazyredraw' 'lz'	boolean	(default off)
			global
	When this option is set, the screen will not be redrawn while
	executing macros, registers and other commands that have not been
	typed.
    'linebreak' 'lbr'	boolean	(default off)
			local to window
	If on, Vim will wrap long lines at a character in 'breakat' rather
	than at the last character that fits on the screen.  
    'lines'			number	(default 24 or terminal height)
			global
	Number of lines of the Vim window.
    'lisp'			boolean	(default off)
			local to buffer
	Lisp mode: When <Enter> is typed in insert mode set the indent for
	the next line to Lisp standards (well, sort of).
    'lispwords' 'lw'	string	(default is very long)
			global or local to buffer |global-local|
	Comma separated list of words that influence the Lisp indenting.
	|'lisp'|
    'list'			boolean	(default off)
			local to window
	List mode: By default, show tabs as ">", trailing spaces as "-", and
	non-breakable space characters as "+".
    'listchars' 'lcs'	string	(default: "tab:> ,trail:-,nbsp:+"
				 Vi default: "eol:$")
			global or local to window |global-local|
	Strings to use in 'list' mode and for the |:list| command.
'loadplugins' 'lpl'	boolean	(default on)
			global
	When on the plugin scripts are loaded when starting up |load-plugins|.
    'magic'			boolean	(default on)
			global
	Changes the special characters that can be used in search patterns.
	See |pattern|.
    'makeef' 'mef'		string	(default: "")
			global
	Name of the errorfile for the |:make| command (see |:make_makeprg|)
	and the |:grep| command.
    'makeencoding' 'menc'	string	(default "")
			global or local to buffer |global-local|
	Encoding used for reading the output of external commands.  When empty,
	encoding is not converted.
    'makeprg' 'mp'		string	(default "make")
			global or local to buffer |global-local|
	Program to use for the ":make" command.  See |:make_makeprg|.
    'matchpairs' 'mps'	string	(default "(:),{:},[:]")
			local to buffer
	Characters that form pairs.  The |%| command jumps from one to the
	other.
    'matchtime' 'mat'	number	(default 5)
			global
	Tenths of a second to show the matching paren, when 'showmatch' is
	set.
    'maxcombine' 'mco'	Removed. |vim-differences|
	Nvim always displays up to 6 combining characters. 
    'maxfuncdepth' 'mfd'	number	(default 100)
			global
	'maxmapdepth' 'mmd'	number	(default 1000)
			global
	Maximum number of times a mapping is done without resulting in a
	character to be used.
    'maxmempattern' 'mmp'	number	(default 1000)
			global
	'menuitems' 'mis'	number	(default 25)
			global
	Maximum number of items to use in a menu.
    'mkspellmem' 'msm'	string	(default "460000,2000,500")
			global
	Parameters for |:mkspell|. 
    'modeline' 'ml'		boolean	(Vim default: on (off for root),
				 Vi default: off)
			local to buffer
	If 'modeline' is on 'modelines' gives the number of lines that is
	checked for set commands.
    'modelineexpr' 'mle'	boolean (default: off)
			global
	When on allow some options that are an expression to be set in the
	modeline. 
    'modelines' 'mls'	number	(default 5)
			global
	If 'modeline' is on 'modelines' gives the number of lines that is
	checked for set commands.
    'modifiable' 'ma'	boolean	(default on)
			local to buffer
	When off the buffer contents cannot be changed. 
    'modified' 'mod'	boolean	(default off)
			local to buffer
	When on, the buffer is considered to be modified. 
    'more'			boolean	(Vim default: on, Vi default: off)
			global
	When on, listings pause when the whole screen is filled.
    'mouse'			string	(default "")
			global

	Enables mouse support.
    'mousefocus' 'mousef'	boolean	(default off)
			global
	The window that the mouse pointer is on is automatically activated.
    'mousehide' 'mh'	boolean	(default on)
			global
			{only works in the GUI}
	When on, the mouse pointer is hidden when characters are typed.
    'mousemodel' 'mousem'	string	(default "extend")
			global
	Sets the model to use for the mouse.
    'mouseshape' 'mouses'	string	(default "i:beam,r:beam,s:updown,sd:cross,
					m:no,ml:up-arrow,v:rightup-arrow")
			global
	This option tells Vim what the mouse pointer should look like in
	different modes.
	'mousetime' 'mouset'	number	(default 500)
			global
	Defines the maximum time in msec between two mouse clicks for the
	second click to be recognized as a multi click.
	'nrformats' 'nf'	string	(default "bin,hex")
			local to buffer
	This defines what bases Vim will consider for numbers when using the
	CTRL-A and CTRL-X commands for adding to and subtracting from a number
	respectively; see |CTRL-A| for more info on these commands.
	'number' 'nu'		boolean	(default off)
			local to window
	Print the line number in front of each line.
	'numberwidth' 'nuw'	number	(Vim default: 4  Vi default: 8)
			local to window
	Minimal number of columns to use for the line number.
	'omnifunc' 'ofu'	string	(default: empty)
			local to buffer
	This option specifies a function to be used for Insert mode omni
	completion with CTRL-X CTRL-O.
	'opendevice' 'odev'	boolean	(default off)
			global
			{only for Windows}
	Enable reading and writing from devices.  This may get Vim stuck on a
	device that can be opened but doesn't actually do the I/O.
	'operatorfunc' 'opfunc'	string	(default: empty)
			global
	This option specifies a function to be called by the |g@| operator.
	'paragraphs' 'para'	string	(default "IPLPPPQPP TPHPLIPpLpItpplpipbp")
			global
	Specifies the nroff macros that separate paragraphs.  These are pairs
	of two letters (see |object-motions|).
	'paste'			boolean	(default off)
			global
	This option is obsolete; |bracketed-paste-mode| is built-in.
	'pastetoggle' 'pt'	string	(default "")
			global
	When non-empty, specifies the key sequence that toggles the 'paste'
	option.
	'patchexpr' 'pex'	string	(default "")
			global
	Expression which is evaluated to apply a patch to a file and generate
	the resulting new version of the file.
	'patchmode' 'pm'	string	(default "")
			global
	When non-empty the oldest version of a file is kept.
	'path' 'pa'		string	(default on Unix: ".,/usr/include,,"
				   other systems: ".,,")
			global or local to buffer |global-local|
	This is a list of directories which will be searched when using the
	|gf|, [f, ]f, ^Wf, |:find|, |:sfind|, |:tabfind| and other commands,
	provided that the file being searched for has a relative path (not
	starting with "/", "./" or "../").
	'preserveindent' 'pi'	boolean	(default off)
			local to buffer
	When changing the indent of the current line, preserve as much of the
	indent structure as possible.
	'previewheight' 'pvh'	number (default 12)
			global
	Default height for a preview window.
	'previewwindow' 'pvw'	boolean (default off)
			local to window
	Identifies the preview window.
	'printdevice' 'pdev'	string	(default empty)
			global
	The name of the printer to be used for |:hardcopy|.
	'printencoding' 'penc'	string	(default empty, except for some systems)
			global
	Sets the character encoding used when printing.
	'printexpr' 'pexpr'	string	(default: see below)
			global
	Expression used to print the PostScript produced with |:hardcopy|.
	'printfont' 'pfn'	string	(default "courier")
			global
	The name of the font that will be used for |:hardcopy|.
	'printheader' 'pheader'  string  (default "%<%f%h%m%=Page %N")
			global
	The format of the header produced in |:hardcopy| output.
	'printmbcharset' 'pmbcs'  string (default "")
			global
	The CJK character set to be used for CJK output from |:hardcopy|.
	'printmbfont' 'pmbfn'	string (default "")
			global
	List of font names to be used for CJK output from |:hardcopy|.
	'printoptions' 'popt' string (default "")
			global
	List of items that control the format of the output of |:hardcopy|.
	'pumblend' 'pb'		number	(default 0)
			global
	Enables pseudo-transparency for the |popup-menu|.
	'pumheight' 'ph'	number	(default 0)
			global
	Maximum number of items to show in the popup menu
	(|ins-completion-menu|). Zero means "use available screen space".
	'pumwidth' 'pw'		number	(default 15)
			global
	Minimum width for the popup menu (|ins-completion-menu|).
	'pyxversion' 'pyx'	number	(default depends on the build)
			global
	Specifies the python version used for pyx* functions and commands
	|python_x|.
	'quickfixtextfunc' 'qftf'	string (default "")
			global
	This option specifies a function to be used to get the text to display
	in the quickfix and location list windows.
	'quoteescape' 'qe'	string	(default "\")
			local to buffer
	The characters that are used to escape quotes in a string.
	'readonly' 'ro'		boolean	(default off)
			local to buffer
	If on, writes fail unless you use a '!'.
	'redrawdebug' 'rdb'	string	(default '')
			global
	Flags to change the way redrawing works, for debugging purposes.
	Most useful with 'writedelay' set to some reasonable value.
	'redrawtime' 'rdt'	number	(default 2000)
			global
	Time in milliseconds for redrawing the display.  Applies to
	'hlsearch', 'inccommand', |:match| highlighting and syntax
	highlighting.
	'regexpengine' 're'	number	(default 0)
			global
	This selects the default regexp engine.
	'relativenumber' 'rnu'	boolean	(default off)
			local to window
	Show the line number relative to the line with the cursor in front of
	each line.
	'remap'			boolean	(default on)
			global
	Allows for mappings to work recursively.
	'report'		number	(default 2)
			global
	Threshold for reporting number of lines changed.
	'revins' 'ri'		boolean	(default off)
			global
	Inserting characters in Insert mode will work backwards.
	'rightleft' 'rl'	boolean	(default off)
			local to window
	When on, display orientation becomes right-to-left, i.e., characters
	that are stored in the file appear from the right to the left.
	'rightleftcmd' 'rlc'	string	(default "search")
			local to window
	Each word in this option enables the command line editing to work in
	right-to-left mode for a group of commands
	'ruler' 'ru'		boolean	(default on)
			global
	Show the line and column number of the cursor position, separated by a
	comma.
	'rulerformat' 'ruf'	string	(default empty)
			global
	When this option is not empty, it determines the content of the ruler
	string, as displayed for the 'ruler' option.
	'runtimepath' 'rtp'	string	(default:     "$XDG_CONFIG_HOME/nvim,
					       $XDG_CONFIG_DIRS[1]/nvim,
					       $XDG_CONFIG_DIRS[2]/nvim,
					       …
					       $XDG_DATA_HOME/nvim[-data]/site,
					       $XDG_DATA_DIRS[1]/nvim/site,
					       $XDG_DATA_DIRS[2]/nvim/site,
					       …
					       $VIMRUNTIME,
					       …
					       $XDG_DATA_DIRS[2]/nvim/site/after,
					       $XDG_DATA_DIRS[1]/nvim/site/after,
					       $XDG_DATA_HOME/nvim[-data]/site/after,
					       …
					       $XDG_CONFIG_DIRS[2]/nvim/after,
					       $XDG_CONFIG_DIRS[1]/nvim/after,
					       $XDG_CONFIG_HOME/nvim/after")
			global
	List of directories to be searched for these runtime files
	'scroll' 'scr'		number	(default: half the window height)
			local to window
	Number of lines to scroll with CTRL-U and CTRL-D commands.
	'scrollback' 'scbk'	number	(default: 10000)
			local to buffer
	Maximum number of lines kept beyond the visible screen.
	'scrollbind' 'scb'	boolean  (default off)
			local to window
	See also |scroll-binding|.
	'scrolljump' 'sj'	number	(default 1)
			global
	Minimal number of lines to scroll when the cursor gets off the
	screen (e.g., with "j").
	'scrolloff' 'so'	number	(default 0)
			global or local to window |global-local|
	Minimal number of screen lines to keep above and below the cursor.
	'scrollopt' 'sbo'	string	(default "ver,jump")
			global
	This is a comma-separated list of words that specifies how
	'scrollbind' windows should behave.
	'sections' 'sect'	string	(default "SHNHH HUnhsh")
			global
	Specifies the nroff macros that separate sections.
	'secure'		boolean	(default off)
			global
	When on, ":autocmd", shell and write commands are not allowed in
	".nvimrc" and ".exrc" in the current directory and map commands are
	displayed.
	'selection' 'sel'	string	(default "inclusive")
			global
	This option defines the behavior of the selection.
	'selectmode' 'slm'	string	(default "")
			global
	This is a comma separated list of words, which specifies when to start
	Select mode instead of Visual mode, when a selection is started.
	'sessionoptions' 'ssop'	string	(default: "blank,buffers,curdir,folds,
					       help,tabpages,winsize"
				 Vi default: "blank,buffers,curdir,folds,
					       help,options,tabpages,winsize")
			global
	Changes the effect of the |:mksession| command.
	'shada' 'sd'		string	(Vim default for
				   Win32:  !,'100,<50,s10,h,rA:,rB:
				   others: !,'100,<50,s10,h
				 Vi default: "")
			global
	When non-empty, the shada file is read upon startup and written
	when exiting Vim (see |shada-file|).
	'shadafile' 'sdf'	string	(default: "")
			global
	When non-empty, overrides the file name used for |shada| (viminfo).
	'shell' 'sh'		string	(default $SHELL or "sh", Win32: "cmd.exe")
			global
	Name of the shell to use for ! and :! commands.
	'shellcmdflag' 'shcf'	string	(default: "-c"; Windows: "/s /c")
			global
	Flag passed to the shell to execute "!" and ":!" commands; e.g.,
	`bash.exe -c ls` or `cmd.exe /s /c "dir"`.
	'shellpipe' 'sp'	string	(default ">", ">%s 2>&1", "| tee", "|& tee" or
				 "2>&1| tee")
			global
	String to be used to put the output of the ":make" command in the
	error file.
	'shellquote' 'shq'	string	(default: ""; Windows, when 'shell'
					contains "sh" somewhere: "\"")
			global
	Quoting character(s), put around the command passed to the shell, for
	the "!" and ":!" commands.
	'shellredir' 'srr'	string	(default ">", ">&" or ">%s 2>&1")
			global
	String to be used to put the output of a filter command in a temporary
	file.
	'shellslash' 'ssl'	boolean	(default off)
			global
			{only for MS-Windows}
	When set, a forward slash is used when expanding file names.
	'shelltemp' 'stmp'	boolean	(Vim default on, Vi default off)
			global
	When on, use temp files for shell commands.
	'shellxescape' 'sxe'	string	(default: "")
			global
	When 'shellxquote' is set to "(" then the characters listed in this
	option will be escaped with a '^' character.
	'shellxquote' 'sxq'	string	(default: "", Windows: "\"")
			global
	Quoting character(s), put around the command passed to the shell, for
	the "!" and ":!" commands.
	'shiftround' 'sr'	boolean	(default off)
			global
	Round indent to multiple of 'shiftwidth'.
	'shiftwidth' 'sw'	number	(default 8)
			local to buffer
	Number of spaces to use for each step of (auto)indent.
	'shortmess' 'shm'	string	(Vim default "filnxtToOF", Vi default: "S")
			global
	This option helps to avoid all the |hit-enter| prompts caused by file
	messages, for example  with CTRL-G, and to avoid some other messages.
	'showbreak' 'sbr'	string	(default "")
			global or local to window |global-local|
	String to put at the start of lines that have been wrapped.
	'showcmd' 'sc'		boolean	(Vim default: on, Vi default: off)
			global
	Show (partial) command in the last line of the screen.
	'showfulltag' 'sft'	boolean (default off)
			global
	When completing a word in insert mode (see |ins-completion|) from the
	tags file, show both the tag name and a tidied-up form of the search
	pattern (if there is one) as possible matches.
	'showmatch' 'sm'	boolean	(default off)
			global
	When a bracket is inserted, briefly jump to the matching one.
	'showmode' 'smd'	boolean	(Vim default: on, Vi default: off)
			global
	If in Insert, Replace or Visual mode put a message on the last line.
	'showtabline' 'stal'	number	(default 1)
			global
	The value of this option specifies when the line with tab page labels
	will be displayed
	'sidescroll' 'ss'	number	(default 1)
			global
	The minimal number of columns to scroll horizontally.
	'sidescrolloff' 'siso'	number (default 0)
			global or local to window |global-local|
	The minimal number of screen columns to keep to the left and to the
	right of the cursor if 'nowrap' is set.
	'signcolumn' 'scl'	string	(default "auto")
			local to window
	When and how to draw the signcolumn. Valid values are
	'smartcase' 'scs'	boolean	(default off)
			global
	Override the 'ignorecase' option if the search pattern contains upper
	case characters.
	'smartindent' 'si'	boolean	(default off)
			local to buffer
	Do smart autoindenting when starting a new line.
	'smarttab' 'sta'	boolean	(default on)
			global
	When on, a <Tab> in front of a line inserts blanks according to
	'shiftwidth'.
	'softtabstop' 'sts'	number	(default 0)
			local to buffer
	Number of spaces that a <Tab> counts for while performing editing
	operations, like inserting a <Tab> or using <BS>.
	'spell'			boolean	(default off)
			local to window
	When on spell checking will be done.  See |spell|.
	'spellcapcheck' 'spc'	string	(default "[.?!]\_[\])'"' \t]\+")
			local to buffer
	Pattern to locate the end of a sentence.
	'spellfile' 'spf'	string	(default empty)
			local to buffer
	Name of the word list file where words are added for the |zg| and |zw|
	commands.
	'spelllang' 'spl'	string	(default "en")
			local to buffer
	A comma separated list of word list names.
	'spelloptions' 'spo'	string	(default "")
			local to buffer
	A comma separated list of options for spell checking
	'spellsuggest' 'sps'	string	(default "best")
			global
	Methods used for spelling suggestions.
	'splitbelow' 'sb'	boolean	(default off)
			global
	When on, splitting a window will put the new window below the current
	one.
	'splitright' 'spr'	boolean	(default off)
			global
	When on, splitting a window will put the new window right of the
	current one.
	'startofline' 'sol'	boolean	(default off)
			global
	When "on" the commands listed below move the cursor to the first
	non-blank of the line.
	'statusline' 'stl'	string	(default empty)
			global or local to window |global-local|
	When nonempty, this option determines the content of the status line.
	'suffixes' 'su'		string	(default ".bak,~,.o,.h,.info,.swp,.obj")
			global
	Files with these suffixes get a lower priority when multiple files
	match a wildcard.
	'suffixesadd' 'sua'	string	(default "")
			local to buffer
	Comma separated list of suffixes, which are used when searching for a
	file for the "gf", "[I", etc. commands.
	'swapfile' 'swf'	boolean (default on)
			local to buffer
	Use a swapfile for the buffer.
	'switchbuf' 'swb'	string	(default "uselast")
			global
	This option controls the behavior when switching between buffers.
	'synmaxcol' 'smc'	number	(default 3000)
			local to buffer
	Maximum column in which to search for syntax items.
	'syntax' 'syn'		string	(default empty)
			local to buffer
	When this option is set, the syntax with this name is loaded, unless
	syntax highlighting has been switched off with ":syntax off".
	'tabline' 'tal'		string	(default empty)
			global
	When nonempty, this option determines the content of the tab pages
	line at the top of the Vim window.
	'tabpagemax' 'tpm'	number	(default 50)
			global
	Maximum number of tab pages to be opened by the |-p| command line
	argument or the ":tab all" command.
	'tabstop' 'ts'		number	(default 8)
			local to buffer
	Number of spaces that a <Tab> in the file counts for.
	'tagbsearch' 'tbs'	boolean	(default on)
			global
	When searching for a tag (e.g., for the |:ta| command), Vim can either
	use a binary search or a linear search in a tags file.
	'tagcase' 'tc'		string	(default "followic")
			global or local to buffer |global-local|
	This option specifies how case is handled when searching the tags
	file
	'tagfunc' 'tfu'		string	(default: empty)
			local to buffer
	This option specifies a function to be used to perform tag searches.
	'taglength' 'tl'	number	(default 0)
			global
	If non-zero, tags are significant up to this number of characters.
	'tagrelative' 'tr'	boolean	(Vim default: on, Vi default: off)
			global
	If on and using a tags file in another directory, file names in that
	tags file are relative to the directory where the tags file is.
	'tags' 'tag'		string	(default "./tags;,tags")
			global or local to buffer |global-local|
	Filenames for the tag command, separated by spaces or commas.
	'tagstack' 'tgst'	boolean	(default on)
			global
	When on, the |tagstack| is used normally.
	'termbidi' 'tbidi'	boolean (default off)
			global
	The terminal is in charge of Bi-directionality of text (as specified
	by Unicode).
	'termguicolors' 'tgc'	boolean (default off)
			global
	Enables 24-bit RGB color in the |TUI|.
	'termpastefilter' 'tpf'	string	(default: "BS,HT,ESC,DEL")
			global
	A comma separated list of options for specifying control characters
	to be removed from the text pasted into the terminal window.
	'terse'			boolean	(default off)
			global
	When set: Add 's' flag to 'shortmess' option (this makes the message
	for a search that hits the start or end of the file not being
	displayed).
	'textwidth' 'tw'	number	(default 0)
			local to buffer
	Maximum width of text that is being inserted.
	'thesaurus' 'tsr'	string	(default "")
			global or local to buffer |global-local|
	List of file names, separated by commas, that are used to lookup words
	for thesaurus completion commands |i_CTRL-X_CTRL-T|.
	'thesaurusfunc' 'tsrfu'	string	(default: empty)
			global or local to buffer |global-local|
	This option specifies a function to be used for thesaurus completion
	with CTRL-X CTRL-T.
	'tildeop' 'top'		boolean	(default off)
			global
	When on: The tilde command "~" behaves like an operator.
	'timeout' 'to'		boolean (default on)
			global
	This option and 'timeoutlen' determine the behavior when part of a
	mapped key sequence has been received.
	'ttimeout'		boolean (default on)
			global
	This option and 'ttimeoutlen' determine the behavior when part of a
	key code sequence has been received by the |TUI|.
	'timeoutlen' 'tm'	number	(default 1000)
			global
	Time in milliseconds to wait for a mapped sequence to complete.
	'ttimeoutlen' 'ttm'	number	(default 50)
			global
	Time in milliseconds to wait for a key code sequence to complete.
	'title'			boolean	(default off)
			global
	When on, the title of the window will be set to the value of
	'titlestring' (if it is not empty), or to
	'titlelen'		number	(default 85)
			global
	Gives the percentage of 'columns' to use for the length of the window
	title.
	'titleold'		string	(default "")
			global
	If not empty, this option will be used to set the window title when
	exiting.
	'titlestring'		string	(default "")
			global
	When this option is not empty, it will be used for the title of the
	window.
	'undodir' 'udir'	string	(default "$XDG_DATA_HOME/nvim/undo//")
			global
	List of directory names for undo files, separated with commas.
	'undofile' 'udf'	boolean	(default off)
			local to buffer
	When on, Vim automatically saves undo history to an undo file when
	writing a buffer to a file, and restores undo history from the same
	file on buffer read.
	'undolevels' 'ul'	number	(default 1000)
			global or local to buffer |global-local|
	Maximum number of changes that can be undone.  Since undo information
	is kept in memory, higher numbers will cause more memory to be used.
	'undoreload' 'ur'	number	(default 10000)
			global
	Save the whole buffer for undo when reloading it.
	'updatecount' 'uc'	number	(default: 200)
			global
	After typing this many characters the swap file will be written to
	disk.
	'updatetime' 'ut'	number	(default 4000)
			global
	If this many milliseconds nothing is typed the swap file will be
	written to disk (see |crash-recovery|).
	'varsofttabstop' 'vsts'	string	(default "")
			local to buffer
	A list of the number of spaces that a <Tab> counts for while editing,
	such as inserting a <Tab> or using <BS>.
	'vartabstop' 'vts'	string	(default "")
			local to buffer
	A list of the number of spaces that a <Tab> in the file counts for,
	separated by commas.
	'verbose' 'vbs'		number	(default 0)
			global
	When bigger than zero, Vim will give messages about what it is doing.
	'verbosefile' 'vfile'	string	(default empty)
			global
	When not empty all messages are written in a file with this name.
	'viewdir' 'vdir'	string	(default: "$XDG_DATA_HOME/nvim/view//")
			global
	Name of the directory where to store files for |:mkview|.
	'viewoptions' 'vop'	string	(default: "folds,cursor,curdir")
			global
	Changes the effect of the |:mkview| command.
	'virtualedit' 've'	string	(default "")
			global
	A comma separated list of these words
	'visualbell' 'vb'	boolean	(default off)
			global
	Use visual bell instead of beeping.
	'warn'			boolean	(default on)
			global
	Give a warning message when a shell command is used while the buffer
	has been changed.
	'whichwrap' 'ww'	string	(Vim default: "b,s", Vi default: "")
			global
	Allow specified keys that move the cursor left/right to move to the
	previous/next line when the cursor is on the first/last character in
	the line.
	'wildchar' 'wc'		number	(Vim default: <Tab>, Vi default: CTRL-E)
			global
	Character you have to type to start wildcard expansion in the
	command-line, as specified with 'wildmode'.
	'wildcharm' 'wcm'	number	(default: none (0))
			global
	'wildcharm' works exactly like 'wildchar', except that it is
	recognized when used inside a macro.
	'wildignore' 'wig'	string	(default "")
			global
	A list of file patterns.
	'wildignorecase' 'wic'	boolean	(default off)
			global
	When set case is ignored when completing file names and directories.
	Has no effect when 'fileignorecase' is set.
	'wildmenu' 'wmnu'	boolean	(default on)
			global
	Enables "enhanced mode" of command-line completion.
	'wildmode' 'wim'	string	(default: "full")
			global
	Completion mode that is used for the character specified with
	'wildchar'.
	'wildoptions' 'wop'	string	(default "pum,tagfile")
			global
	List of words that change how |cmdline-completion| is done.
	'winaltkeys' 'wak'	string	(default "menu")
			global
			{only used in Win32}
	Some GUI versions allow the access to menu entries by using the ALT
	key in combination with a character that appears underlined in the
	menu.
	'winblend' 'winbl'		number	(default 0)
			local to window
	Enables pseudo-transparency for a floating window.
	'window' 'wi'		number  (default screen height - 1)
			global
	Window height used for |CTRL-F| and |CTRL-B| when there is only one
	window and the value is smaller than 'lines' minus one.
	'winheight' 'wh'	number	(default 1)
			global
	Minimal number of lines for the current window.
	'winhighlight' 'winhl'	string (default empty)
			local to window
	Window-local highlights.
	'winfixheight' 'wfh'	boolean	(default off)
			local to window
	Keep the window height when windows are opened or closed and
	'equalalways' is set.
	'winfixwidth' 'wfw'	boolean	(default off)
			local to window
	Keep the window width when windows are opened or closed and
	'equalalways' is set.
	'winminheight' 'wmh'	number	(default 1)
			global
	The minimal height of a window, when it's not the current window.
	This is a hard minimum, windows will never become smaller.
	'winminwidth' 'wmw'	number	(default 1)
			global
	The minimal width of a window, when it's not the current window.
	'winwidth' 'wiw'	number	(default 20)
			global
	Minimal number of columns for the current window.
	'wrap'			boolean	(default on)
			local to window
	This option changes how text is displayed.
	'wrapmargin' 'wm'	number	(default 0)
			local to buffer
	Number of characters from the right window border where wrapping
	starts.
	'wrapscan' 'ws'		boolean	(default on)			*E384* *E385*
			global
	Searches wrap around the end of the file.
	'write'			boolean	(default on)
			global
	Allows writing files.
	'writeany' 'wa'		boolean	(default off)
			global
	Allows writing to any file with no need for "!" override.
	'writebackup' 'wb'	boolean	(default on)
			global
	Make a backup before overwriting a file.
	'writedelay' 'wd'	number	(default 0)
			global
	The number of milliseconds to wait for each character sent to the
	screen.

pattern.txt                               :          regexp patterns and search commands
map.txt                                   :          key mapping and abbreviations

### Tags and special searches *tags-and-searches* *tagsrch.txt*

*:ta* *:tag* *E426* *E429*
:[count]ta[g][!] {name}
			Jump to the definition of {name}, using the
			information in the tags file(s).  Put {name} in the
			tag stack.  See |tag-!| for [!].
			{name} can be a regexp pattern, see |tag-regexp|.
			When there are several matching tags for {name}, jump
			to the [count] one.  When [count] is omitted the
			first one is jumped to. See |tag-matchlist| for
			jumping to other matching tags.


g<LeftMouse>						*g<LeftMouse>*

<C-LeftMouse>					*<C-LeftMouse>* *CTRL-]*
CTRL-]			Jump to the definition of the keyword under the
			cursor.  Same as ":tag {name}", where {name} is the
			keyword under or after cursor.
			When there are several matching tags for {name}, jump
			to the [count] one.  When no [count] is given the
			first one is jumped to. See |tag-matchlist| for
			jumping to other matching tags.


							*v_CTRL-]*
{Visual}CTRL-]		Same as ":tag {name}", where {name} is the text that
			is highlighted.

	g<RightMouse>						*g<RightMouse>*

<C-RightMouse>					*<C-RightMouse>* *CTRL-T*
CTRL-T			Jump to [count] older entry in the tag stack
			(default 1).


						*:po* *:pop* *E555* *E556*
:[count]po[p][!]	Jump to [count] older entry in tag stack (default 1).
			See |tag-!| for [!].

:[count]ta[g][!]	Jump to [count] newer entry in tag stack (default 1).
			See |tag-!| for [!].


							*:tags*
:tags			Show the contents of the tag stack.  The active
			entry is marked with a '>'.

	*:ts* *:tselect*
:ts[elect][!] [name]	List the tags that match [name], using the
			information in the tags file(s).
			When [name] is not given, the last tag name from the
			tag stack is used.
			See |tag-!| for [!].
			With a '>' in the first column is indicated which is
			the current position in the list (if there is one).
			[name] can be a regexp pattern, see |tag-regexp|.
			See |tag-priority| for the priorities used in the
			listing.
			Example output:


	  # pri kind tag		file
	  1 F	f    mch_delay		os_amiga.c
			mch_delay(msec, ignoreinput)
	> 2 F	f    mch_delay		os_msdos.c
			mch_delay(msec, ignoreinput)
	  3 F	f    mch_delay		os_unix.c
			mch_delay(msec, ignoreinput)
	Type number and <Enter> (empty cancels):
 
			See |tag-priority| for the "pri" column.  Note that
			this depends on the current file, thus using
			":tselect xxx" can produce different results.
			The "kind" column gives the kind of tag, if this was
			included in the tags file.
			The "info" column shows information that could be
			found in the tags file.  It depends on the program
			that produced the tags file.
			When the list is long, you may get the |more-prompt|.
			If you already see the tag you want to use, you can
			type 'q' and enter the number.


							*:sts* *:stselect*
:sts[elect][!] [name]	Does ":tselect[!] [name]" and splits the window for
			the selected tag.


							*g]*
g]			Like CTRL-], but use ":tselect" instead of ":tag".


							*v_g]*
{Visual}g]		Same as "g]", but use the highlighted text as the
			identifier.


							*:tj* *:tjump*
:tj[ump][!] [name]	Like ":tselect", but jump to the tag directly when
			there is only one match.


							*:stj* *:stjump*
:stj[ump][!] [name]	Does ":tjump[!] [name]" and splits the window for the
			selected tag.


							*g_CTRL-]*
g CTRL-]		Like CTRL-], but use ":tjump" instead of ":tag".


							*v_g_CTRL-]*
{Visual}g CTRL-]	Same as "g CTRL-]", but use the highlighted text as
			the identifier.


							*:tn* *:tnext*
:[count]tn[ext][!]	Jump to [count] next matching tag (default 1).  See
			|tag-!| for [!].


							*:tp* *:tprevious*
:[count]tp[revious][!]	Jump to [count] previous matching tag (default 1).
			See |tag-!| for [!].


							*:tN* *:tNext*
:[count]tN[ext][!]	Same as ":tprevious".


							*:tr* *:trewind*
:[count]tr[ewind][!]	Jump to first matching tag.  If [count] is given, jump
			to [count]th matching tag.  See |tag-!| for [!].


							*:tf* *:tfirst*
:[count]tf[irst][!]	Same as ":trewind".


							*:tl* *:tlast*
:tl[ast][!]		Jump to last matching tag.  See |tag-!| for [!].


							*:lt* *:ltag*
:lt[ag][!] [name]	Jump to tag [name] and add the matching tags to a new
			location list for the current window.

	*:pts* *:ptselect*
:pts[elect][!] [name]	Does ":tselect[!] [name]" and shows the new tag in a
			"Preview" window.  See |:ptag| for more info.


							*:ptj* *:ptjump*
:ptj[ump][!] [name]	Does ":tjump[!] [name]" and shows the new tag in a
			"Preview" window.  See |:ptag| for more info.


							*:ptn* *:ptnext*
:[count]ptn[ext][!]	":tnext" in the preview window.  See |:ptag|.


							*:ptp* *:ptprevious*
:[count]ptp[revious][!]	":tprevious" in the preview window.  See |:ptag|.


							*:ptN* *:ptNext*
:[count]ptN[ext][!]	Same as ":ptprevious".


							*:ptr* *:ptrewind*
:[count]ptr[ewind][!]	":trewind" in the preview window.  See |:ptag|.


							*:ptf* *:ptfirst*
:[count]ptf[irst][!]	Same as ":ptrewind".


							*:ptl* *:ptlast*
:ptl[ast][!]		":tlast" in the preview window.  See |:ptag|.

*[i*
[i			Display the first line that contains the keyword
			under the cursor.  The search starts at the beginning
			of the file.  Lines that look like a comment are
			ignored (see 'comments' option).  If a count is given,
			the count'th matching line is displayed, and comment
			lines are not ignored.


							*]i*
]i			like "[i", but start at the current cursor position.


							*:is* *:isearch*
:[range]is[earch][!] [count] [/]pattern[/]
			Like "[i"  and "]i", but search in [range] lines
			(default: whole file).
			See |:search-args| for [/] and [!].


							*[I*
[I			Display all lines that contain the keyword under the
			cursor.  Filenames and line numbers are displayed
			for the found lines.  The search starts at the
			beginning of the file.


							*]I*
]I			like "[I", but start at the current cursor position.


							*:il* *:ilist*
:[range]il[ist][!] [/]pattern[/]
			Like "[I" and "]I", but search in [range] lines
			(default: whole file).
			See |:search-args| for [/] and [!].


							*[_CTRL-I*
[ CTRL-I		Jump to the first line that contains the keyword
			under the cursor.  The search starts at the beginning
			of the file.  Lines that look like a comment are
			ignored (see 'comments' option).  If a count is given,
			the count'th matching line is jumped to, and comment
			lines are not ignored.


							*]_CTRL-I*
] CTRL-I		like "[ CTRL-I", but start at the current cursor
			position.


							*:ij* *:ijump*
:[range]ij[ump][!] [count] [/]pattern[/]
			Like "[ CTRL-I"  and "] CTRL-I", but search in
			[range] lines (default: whole file).
			See |:search-args| for [/] and [!].


CTRL-W CTRL-I					*CTRL-W_CTRL-I* *CTRL-W_i*
CTRL-W i		Open a new window, with the cursor on the first line
			that contains the keyword under the cursor.  The
			search starts at the beginning of the file.  Lines
			that look like a comment line are ignored (see
			'comments' option).  If a count is given, the count'th
			matching line is jumped to, and comment lines are not
			ignored.


							*:isp* *:isplit*
:[range]isp[lit][!] [count] [/]pattern[/]
			Like "CTRL-W i"  and "CTRL-W i", but search in
			[range] lines (default: whole file).
			See |:search-args| for [/] and [!].


							*[d*
[d			Display the first macro definition that contains the
			macro under the cursor.  The search starts from the
			beginning of the file.  If a count is given, the
			count'th matching line is displayed.


							*]d*
]d			like "[d", but start at the current cursor position.


							*:ds* *:dsearch*
:[range]ds[earch][!] [count] [/]string[/]
			Like "[d"  and "]d", but search in [range] lines
			(default: whole file).
			See |:search-args| for [/] and [!].


							*[D*
[D			Display all macro definitions that contain the macro
			under the cursor.  Filenames and line numbers are
			displayed for the found lines.  The search starts
			from the beginning of the file.


							*]D*
]D			like "[D", but start at the current cursor position.


							*:dli* *:dlist*
:[range]dli[st][!] [/]string[/]
			Like `[D`  and `]D`, but search in [range] lines
			(default: whole file).
			See |:search-args| for [/] and [!].
			Note that `:dl` works like `:delete` with the "l"
			flag, not `:dlist`.


							*[_CTRL-D*
[ CTRL-D		Jump to the first macro definition that contains the
			keyword under the cursor.  The search starts from
			the beginning of the file.  If a count is given, the
			count'th matching line is jumped to.


							*]_CTRL-D*
] CTRL-D		like "[ CTRL-D", but start at the current cursor
			position.


							*:dj* *:djump*
:[range]dj[ump][!] [count] [/]string[/]
			Like "[ CTRL-D"  and "] CTRL-D", but search  in
			[range] lines (default: whole file).
			See |:search-args| for [/] and [!].


CTRL-W CTRL-D					*CTRL-W_CTRL-D* *CTRL-W_d*
CTRL-W d		Open a new window, with the cursor on the first
			macro definition line that contains the keyword
			under the cursor.  The search starts from the
			beginning of the file.  If a count is given, the
			count'th matching line is jumped to.


							*:dsp* *:dsplit*
:[range]dsp[lit][!] [count] [/]string[/]
			Like "CTRL-W d", but search in [range] lines
			(default: whole file).
			See |:search-args| for [/] and [!].


					*:che* *:chec* *:check* *:checkpath*
:che[ckpath]		List all the included files that could not be found.

:che[ckpath]!		List all the included files.


								*:search-args*
Common arguments for the commands above:
[!]	When included, find matches in lines that are recognized as comments.
	When excluded, a match is ignored when the line is recognized as a
	comment (according to 'comments'), or the match is in a C comment
	(after "//" or inside /* */).  Note that a match may be missed if a
	line is recognized as a comment, but the comment ends halfway the line.
	And if the line is a comment, but it is not recognized (according to
	'comments') a match may be found in it anyway.  Example:
		/* comment
		   foobar */
 	A match for "foobar" is found, because this line is not recognized as
	a comment (even though syntax highlighting does recognize it).
	Note: Since a macro definition mostly doesn't look like a comment, the
	[!] makes no difference for ":dlist", ":dsearch" and ":djump".
[/]	A pattern can be surrounded by '/'.  Without '/' only whole words are
	matched, using the pattern "\<pattern\>".

windows.txt                           :          commands for using multiple windows and buffers
tabpage.txt                             :          commands for using multiple tab pages
spell.txt                                  :          spell checking
diff.txt                                    :          working with two four versions of the same file
autocmd.txt                            :         automatically executing commands on an event
eval.txt                                  :         expression evaluation, conditional commands
fold.txt                                   :         hide (fold) ranges of lines

## Special issues

print.txt                                  :         printing
remote.txt                               :        using Vim as a server or client

## Programming language support

indent.txt                                :         automatic indenting for C and other languages
syntax.txt                                :         syntax highlighting
filetype.txt                              :         settings done specifically for a type of file

### *quickfix.txt*

*:cc*
:cc[!] [nr]		Display error [nr].  If [nr] is omitted, the same
:[nr]cc[!]		error is displayed again.  Without [!] this doesn't
			work when jumping to another buffer, the current buffer
			has been changed, there is the only window for the
			buffer and both 'hidden' and 'autowrite' are off.
			When jumping to another buffer with [!] any changes to
			the current buffer are lost, unless 'hidden' is set or
			there is another window for this buffer.
			The 'switchbuf' settings are respected when jumping
			to a buffer.
			When used in the quickfix window the line number can
			be used, including "." for the current line and "$"
			for the last line.


							*:ll*
:ll[!] [nr]		Same as ":cc", except the location list for the
:[nr]ll[!]		current window is used instead of the quickfix list.


						*:cn* *:cne* *:cnext* *E553*
:[count]cn[ext][!]	Display the [count] next error in the list that
			includes a file name.  If there are no file names at
			all, go to the [count] next error.  See |:cc| for
			[!] and 'switchbuf'.


							*:lne* *:lnext*
:[count]lne[xt][!]	Same as ":cnext", except the location list for the
			current window is used instead of the quickfix list.


:[count]cN[ext][!]		*:cp* *:cprevious*  *:cprev* *:cN* *:cNext*
:[count]cp[revious][!]	Display the [count] previous error in the list that
			includes a file name.  If there are no file names at
			all, go to the [count] previous error.  See |:cc| for
			[!] and 'switchbuf'.



:[count]lN[ext][!]		*:lp* *:lprevious* *:lprev* *:lN* *:lNext*
:[count]lp[revious][!]	Same as ":cNext" and ":cprevious", except the location
			list for the current window is used instead of the
			quickfix list.


							*:cabo* *:cabove*
:[count]cabo[ve]	Go to the [count] error above the current line in the
			current buffer.  If [count] is omitted, then 1 is
			used.  If there are no errors, then an error message
			is displayed.  Assumes that the entries in a quickfix
			list are sorted by their buffer number and line
			number. If there are multiple errors on the same line,
			then only the first entry is used.  If [count] exceeds
			the number of entries above the current line, then the
			first error in the file is selected.


							*:lab* *:labove*
:[count]lab[ove]	Same as ":cabove", except the location list for the
			current window is used instead of the quickfix list.


							*:cbel* *:cbelow*
:[count]cbel[ow]	Go to the [count] error below the current line in the
			current buffer.  If [count] is omitted, then 1 is
			used.  If there are no errors, then an error message
			is displayed.  Assumes that the entries in a quickfix
			list are sorted by their buffer number and line
			number.  If there are multiple errors on the same
			line, then only the first entry is used.  If [count]
			exceeds the number of entries below the current line,
			then the last error in the file is selected.


							*:lbel* *:lbelow*
:[count]lbel[ow]	Same as ":cbelow", except the location list for the
			current window is used instead of the quickfix list.


							*:cbe* *:cbefore*
:[count]cbe[fore]	Go to the [count] error before the current cursor
			position in the current buffer.  If [count] is
			omitted, then 1 is used.  If there are no errors, then
			an error message is displayed.  Assumes that the
			entries in a quickfix list are sorted by their buffer,
			line and column numbers.  If [count] exceeds the
			number of entries before the current position, then
			the first error in the file is selected.


							*:lbe* *:lbefore*
:[count]lbe[fore]	Same as ":cbefore", except the location list for the
			current window is used instead of the quickfix list.


							*:caf* *:cafter*
:[count]caf[ter]	Go to the [count] error after the current cursor
			position in the current buffer.  If [count] is
			omitted, then 1 is used.  If there are no errors, then
			an error message is displayed.  Assumes that the
			entries in a quickfix list are sorted by their buffer,
			line and column numbers.  If [count] exceeds the
			number of entries after the current position, then
			the last error in the file is selected.


							*:laf* *:lafter*
:[count]laf[ter]	Same as ":cafter", except the location list for the
			current window is used instead of the quickfix list.


							*:cnf* *:cnfile*
:[count]cnf[ile][!]	Display the first error in the [count] next file in
			the list that includes a file name.  If there are no
			file names at all or if there is no next file, go to
			the [count] next error.  See |:cc| for [!] and
			'switchbuf'.


							*:lnf* *:lnfile*
:[count]lnf[ile][!]	Same as ":cnfile", except the location list for the
			current window is used instead of the quickfix list.


:[count]cNf[ile][!]			*:cpf* *:cpfile* *:cNf* *:cNfile*
:[count]cpf[ile][!]	Display the last error in the [count] previous file in
			the list that includes a file name.  If there are no
			file names at all or if there is no next file, go to
			the [count] previous error.  See |:cc| for [!] and
			'switchbuf'.



:[count]lNf[ile][!]			*:lpf* *:lpfile* *:lNf* *:lNfile*
:[count]lpf[ile][!]	Same as ":cNfile" and ":cpfile", except the location
			list for the current window is used instead of the
			quickfix list.


							*:crewind* *:cr*
:cr[ewind][!] [nr]	Display error [nr].  If [nr] is omitted, the FIRST
			error is displayed.  See |:cc|.


							*:lrewind* *:lr*
:lr[ewind][!] [nr]	Same as ":crewind", except the location list for the
			current window is used instead of the quickfix list.


							*:cfirst* *:cfir*
:cfir[st][!] [nr]	Same as ":crewind".


							*:lfirst* *:lfir*
:lfir[st][!] [nr]	Same as ":lrewind".


							*:clast* *:cla*
:cla[st][!] [nr]	Display error [nr].  If [nr] is omitted, the LAST
			error is displayed.  See |:cc|.


							*:llast* *:lla*
:lla[st][!] [nr]	Same as ":clast", except the location list for the
			current window is used instead of the quickfix list.


							*:cq* *:cquit*
:cq[uit][!]
:{N}cq[uit][!]
:cq[uit][!] {N}		Quit Vim with error code {N}.  {N} defaults to one.
			Useful when Vim is called from another program:
			e.g., a compiler will not compile the same file again,
			`git commit` will abort the committing process, `fc`
			(built-in for shells like bash and zsh) will not
			execute the command, etc.
			{N} can also be zero, in which case Vim exits
			normally.
			WARNING: All changes in files are lost.  It works like
			":qall!" |:qall|, except that Nvim exits non-zero or
			[count].


							*:cf* *:cfi* *:cfile*
:cf[ile][!] [errorfile]	Read the error file and jump to the first error.
			This is done automatically when Vim is started with
			the -q option.  You can use this command when you
			keep Vim running while compiling.  If you give the
			name of the errorfile, the 'errorfile' option will
			be set to [errorfile].  See |:cc| for [!].
			If the encoding of the error file differs from the
			'encoding' option, you can use the 'makeencoding'
			option to specify the encoding.


							*:lf* *:lfi* *:lfile*
:lf[ile][!] [errorfile]	Same as ":cfile", except the location list for the
			current window is used instead of the quickfix list.
			You can not use the -q command-line option to set
			the location list.



:cg[etfile] [errorfile]					*:cg* *:cgetfile*
			Read the error file.  Just like ":cfile" but don't
			jump to the first error.
			If the encoding of the error file differs from the
			'encoding' option, you can use the 'makeencoding'
			option to specify the encoding.



:lg[etfile] [errorfile]					*:lg* *:lge* *:lgetfile*
			Same as ":cgetfile", except the location list for the
			current window is used instead of the quickfix list.


							*:caddf* *:caddfile*
:caddf[ile] [errorfile]	Read the error file and add the errors from the
			errorfile to the current quickfix list. If a quickfix
			list is not present, then a new list is created.
			If the encoding of the error file differs from the
			'encoding' option, you can use the 'makeencoding'
			option to specify the encoding.


							*:laddf* *:laddfile*
:laddf[ile] [errorfile]	Same as ":caddfile", except the location list for the
			current window is used instead of the quickfix list.


						*:cb* *:cbuffer* *E681*
:cb[uffer][!] [bufnr]	Read the error list from the current buffer.
			When [bufnr] is given it must be the number of a
			loaded buffer.  That buffer will then be used instead
			of the current buffer.
			A range can be specified for the lines to be used.
			Otherwise all lines in the buffer are used.
			See |:cc| for [!].


						*:lb* *:lbuffer*
:lb[uffer][!] [bufnr]	Same as ":cbuffer", except the location list for the
			current window is used instead of the quickfix list.


						*:cgetb* *:cgetbuffer*
:cgetb[uffer] [bufnr]	Read the error list from the current buffer.  Just
			like ":cbuffer" but don't jump to the first error.


						*:lgetb* *:lgetbuffer*
:lgetb[uffer] [bufnr]	Same as ":cgetbuffer", except the location list for
			the current window is used instead of the quickfix
			list.


						*:cad* *:cadd* *:caddbuffer*
:cad[dbuffer] [bufnr]	Read the error list from the current buffer and add
			the errors to the current quickfix list.  If a
			quickfix list is not present, then a new list is
			created. Otherwise, same as ":cbuffer".


							*:laddb* *:laddbuffer*
:laddb[uffer] [bufnr]	Same as ":caddbuffer", except the location list for
			the current window is used instead of the quickfix
			list.


							*:cex* *:cexpr* *E777*
:cex[pr][!] {expr}	Create a quickfix list using the result of {expr} and
			jump to the first error.
			If {expr} is a String, then each newline terminated
			line in the String is processed using the global value
			of 'errorformat' and the result is added to the
			quickfix list.
			If {expr} is a List, then each String item in the list
			is processed and added to the quickfix list.  Non
			String items in the List are ignored.
			See |:cc| for [!].
			Examples:
				:cexpr system('grep -n xyz *')
				:cexpr getline(1, '$')
 

							*:lex* *:lexpr*
:lex[pr][!] {expr}	Same as |:cexpr|, except the location list for the
			current window is used instead of the quickfix list.


							*:cgete* *:cgetexpr*
:cgete[xpr] {expr}	Create a quickfix list using the result of {expr}.
			Just like |:cexpr|, but don't jump to the first error.


							*:lgete* *:lgetexpr*
:lgete[xpr] {expr}	Same as |:cgetexpr|, except the location list for the
			current window is used instead of the quickfix list.


							*:cadde* *:caddexpr*
:cadde[xpr] {expr}	Evaluate {expr} and add the resulting lines to the
			current quickfix list. If a quickfix list is not
			present, then a new list is created. The current
			cursor position will not be changed. See |:cexpr| for
			more information.
			Example:
    :g/mypattern/caddexpr expand("%") . ":" . line(".") .  ":" . getline(".")
 

						*:lad* *:addd* *:laddexpr*
:lad[dexpr] {expr}	Same as ":caddexpr", except the location list for the
			current window is used instead of the quickfix list.


							*:cl* *:clist*
:cl[ist] [from] [, [to]]
			List all errors that are valid |quickfix-valid|.
			If numbers [from] and/or [to] are given, the respective
			range of errors is listed.  A negative number counts
			from the last error backwards, -1 being the last error.
			The 'switchbuf' settings are respected when jumping
			to a buffer.
			The |:filter| command can be used to display only the
			quickfix entries matching a supplied pattern. The
			pattern is matched against the filename, module name,
			pattern and text of the entry.

:cl[ist] +{count}	List the current and next {count} valid errors.  This
			is similar to ":clist from from+count", where "from"
			is the current error position.

:cl[ist]! [from] [, [to]]
			List all errors.

:cl[ist]! +{count}	List the current and next {count} error lines.  This
			is useful to see unrecognized lines after the current
			one.  For example, if ":clist" shows:
        8384 testje.java:252: error: cannot find symbol 
			Then using ":cl! +3" shows the reason:
        8384 testje.java:252: error: cannot find symbol 
        8385:   ZexitCode = Fmainx(); 
        8386:               ^ 
        8387:   symbol:   method Fmainx() 


:lli[st] [from] [, [to]]				*:lli* *:llist*
			Same as ":clist", except the location list for the
			current window is used instead of the quickfix list.

:lli[st]! [from] [, [to]]
			List all the entries in the location list for the
			current window.

	*:cdo*
:cdo[!] {cmd}		Execute {cmd} in each valid entry in the quickfix list.
			It works like doing this:
				:cfirst
				:{cmd}
				:cnext
				:{cmd}
				etc.
 			When the current file can't be |abandon|ed and the [!]
			is not present, the command fails.
			When going to the next entry fails execution stops.
			The last buffer (or where an error occurred) becomes
			the current buffer.
			{cmd} can contain '|' to concatenate several commands.

			Only valid entries in the quickfix list are used.
			A range can be used to select entries, e.g.:
				:10,$cdo cmd
 			To skip entries 1 to 9.

			Note: While this command is executing, the Syntax
			autocommand event is disabled by adding it to
			'eventignore'.  This considerably speeds up editing
			each buffer.
			{not in Vi}
			Also see |:bufdo|, |:tabdo|, |:argdo|, |:windo|,
			|:ldo|, |:cfdo| and |:lfdo|.


							*:cfdo*
:cfdo[!] {cmd}		Execute {cmd} in each file in the quickfix list.
			It works like doing this:
				:cfirst
				:{cmd}
				:cnfile
				:{cmd}
				etc.
 			Otherwise it works the same as `:cdo`.
			{not in Vi}


							*:ldo*
:ld[o][!] {cmd}		Execute {cmd} in each valid entry in the location list
			for the current window.
			It works like doing this:
				:lfirst
				:{cmd}
				:lnext
				:{cmd}
				etc.
 			Only valid entries in the location list are used.
			Otherwise it works the same as `:cdo`.
			{not in Vi}


							*:lfdo*
:lfdo[!] {cmd}		Execute {cmd} in each file in the location list for
			the current window.

	*:cope* *:copen* *w:quickfix_title*
:cope[n] [height]	Open a window to show the current list of errors.

			When [height] is given, the window becomes that high
			(if there is room).  When [height] is omitted the
			window is made ten lines high.

			If there already is a quickfix window, it will be made
			the current window.  It is not possible to open a
			second quickfix window.  If [height] is given the
			existing window will be resized to it.

			The window will contain a special buffer, with
			'buftype' equal to "quickfix".  Don't change this!
			The window will have the w:quickfix_title variable set
			which will indicate the command that produced the
			quickfix list. This can be used to compose a custom
			status line if the value of 'statusline' is adjusted
			properly. Whenever this buffer is modified by a
			quickfix command or function, the |b:changedtick|
			variable is incremented.


							*:lop* *:lopen*
:lop[en] [height]	Open a window to show the location list for the
			current window. Works only when the location list for
			the current window is present.  You can have more than
			one location window opened at a time.  Otherwise, it
			acts the same as ":copen".


							*:ccl* *:cclose*
:ccl[ose]		Close the quickfix window.


							*:lcl* *:lclose*
:lcl[ose]		Close the window showing the location list for the
			current window.


							*:cw* *:cwindow*
:cw[indow] [height]	Open the quickfix window when there are recognized
			errors.  If the window is already open and there are
			no recognized errors, close the window.


							*:lw* *:lwindow*
:lw[indow] [height]	Same as ":cwindow", except use the window showing the
			location list for the current window.


							*:cbo* *:cbottom*
:cbo[ttom]		Put the cursor in the last line of the quickfix window
			and scroll to make it visible.  This is useful for
			when errors are added by an asynchronous callback.
			Only call it once in a while if there are many
			updates to avoid a lot of redrawing.


							*:lbo* *:lbottom*
:lbo[ttom]		Same as ":cbottom", except use the window showing the
			location list for the current window.

	*:colder* *:col* *E380*
:col[der] [count]	Go to older error list.  When [count] is given, do
			this [count] times.  When already at the oldest error
			list, an error message is given.


						*:lolder* *:lol*
:lol[der] [count]	Same as `:colder`, except use the location list for
			the current window instead of the quickfix list.


						*:cnewer* *:cnew* *E381*
:cnew[er] [count]	Go to newer error list.  When [count] is given, do
			this [count] times.  When already at the newest error
			list, an error message is given.


						*:lnewer* *:lnew*
:lnew[er] [count]	Same as `:cnewer`, except use the location list for
			the current window instead of the quickfix list.


						*:chistory* *:chi*
:[count]chi[story]	Show the list of error lists.  The current list is
			marked with ">".  The output looks like:
			  error list 1 of 3; 43 errors   :make  
			> error list 2 of 3; 0 errors    :helpgrep tag  
			  error list 3 of 3; 15 errors   :grep ex_help *.c 

			When [count] is given, then the count'th quickfix
			list is made the current list. Example:
				" Make the 4th quickfix list current
				:4chistory
 

						*:lhistory* *:lhi*
:[count]lhi[story]	Show the list of location lists, otherwise like
			`:chistory`.

	*:mak* *:make*
:mak[e][!] [arguments]	1. All relevant |QuickFixCmdPre| autocommands are
			   executed.
			2. If the 'autowrite' option is on, write any changed
			   buffers
			3. An errorfile name is made from 'makeef'.  If
			   'makeef' doesn't contain "##", and a file with this
			   name already exists, it is deleted.
			4. The program given with the 'makeprg' option is
			   started (default "make") with the optional
			   [arguments] and the output is saved in the
			   errorfile (for Unix it is also echoed on the
			   screen).
			5. The errorfile is read using 'errorformat'.
			6. All relevant |QuickFixCmdPost| autocommands are
			   executed. See example below.
			7. If [!] is not given the first error is jumped to.
			8. The errorfile is deleted.
			9. You can now move through the errors with commands
			   like |:cnext| and |:cprevious|, see above.
			This command does not accept a comment, any "
			characters are considered part of the arguments.
			If the encoding of the program output differs from the
			'encoding' option, you can use the 'makeencoding'
			option to specify the encoding.


							*:lmak* *:lmake*
:lmak[e][!] [arguments]
			Same as ":make", except the location list for the
			current window is used instead of the quickfix list.

	*:vim* *:vimgrep* *E682* *E683*
:vim[grep][!] /{pattern}/[g][j] {file} ...
			Search for {pattern} in the files {file} ... and set
			the error list to the matches.  Files matching
			'wildignore' are ignored; files in 'suffixes' are
			searched last.

			{pattern} is a Vim search pattern.  Instead of
			enclosing it in / any non-ID character (see
			|'isident'|) can be used, so long as it does not
			appear in {pattern}.
			'ignorecase' applies.  To overrule it put |/\c| in the
			pattern to ignore case or |/\C| to match case.
			'smartcase' is not used.
			If {pattern} is empty (e.g. // is specified), the last
			used search pattern is used. |last-pattern|

			Flags:
			'g'  Without the 'g' flag each line is added only
			     once.  With 'g' every match is added.

			'j'  Without the 'j' flag Vim jumps to the first
			     match.  With 'j' only the quickfix list is
			     updated.  With the [!] any changes in the current
			     buffer are abandoned.

			|QuickFixCmdPre| and |QuickFixCmdPost| are triggered.
			A file that is opened for matching may use a buffer
			number, but it is reused if possible to avoid
			consuming buffer numbers.

:{count}vim[grep] ...
			When a number is put before the command this is used
			as the maximum number of matches to find.  Use
			":1vimgrep pattern file" to find only the first.
			Useful if you only want to check if there is a match
			and quit quickly when it's found.

			Every second or so the searched file name is displayed
			to give you an idea of the progress made.
			Examples:
				:vimgrep /an error/ *.c
				:vimgrep /\<FileName\>/ *.h include/*
				:vimgrep /myfunc/ **/*.c
 			For the use of "**" see |starstar-wildcard|.

:vim[grep][!] {pattern} {file} ...
			Like above, but instead of enclosing the pattern in a
			non-ID character use a white-separated pattern.  The
			pattern must start with an ID character.
			Example:
				:vimgrep Error *.c
 

							*:lv* *:lvimgrep*
:lv[imgrep][!] /{pattern}/[g][j] {file} ...
:lv[imgrep][!] {pattern} {file} ...
			Same as ":vimgrep", except the location list for the
			current window is used instead of the quickfix list.


						*:vimgrepa* *:vimgrepadd*
:vimgrepa[dd][!] /{pattern}/[g][j] {file} ...
:vimgrepa[dd][!] {pattern} {file} ...
			Just like ":vimgrep", but instead of making a new list
			of errors the matches are appended to the current
			list.


						*:lvimgrepa* *:lvimgrepadd*
:lvimgrepa[dd][!] /{pattern}/[g][j] {file} ...
:lvimgrepa[dd][!] {pattern} {file} ...
			Same as ":vimgrepadd", except the location list for
			the current window is used instead of the quickfix
			list.

	*:gr* *:grep*
:gr[ep][!] [arguments]	Just like ":make", but use 'grepprg' instead of
			'makeprg' and 'grepformat' instead of 'errorformat'.
			When 'grepprg' is "internal" this works like
			|:vimgrep|.  Note that the pattern needs to be
			enclosed in separator characters then.
			If the encoding of the program output differs from the
			'encoding' option, you can use the 'makeencoding'
			option to specify the encoding.


							    *:lgr* *:lgrep*
:lgr[ep][!] [arguments]	Same as ":grep", except the location list for the
			current window is used instead of the quickfix list.


							*:grepa* *:grepadd*
:grepa[dd][!] [arguments]
			Just like ":grep", but instead of making a new list of
			errors the matches are appended to the current list.
			Example:
				:call setqflist([])
				:bufdo grepadd! something %
 			The first command makes a new error list which is
			empty.  The second command executes "grepadd" for each
			listed buffer.  Note the use of ! to avoid that
			":grepadd" jumps to the first error, which is not
			allowed with |:bufdo|.
			An example that uses the argument list and avoids
			errors for files without matches:
				:silent argdo try
				  \ | grepadd! something %
				  \ | catch /E480:/
				  \ | endtry"
 
			If the encoding of the program output differs from the
			'encoding' option, you can use the 'makeencoding'
			option to specify the encoding.


							*:lgrepa* *:lgrepadd*
:lgrepa[dd][!] [arguments]
			Same as ":grepadd", except the location list for the
			current window is used instead of the quickfix list.

	*:comp* *:compiler* *E666*
:comp[iler][!] {name}		Set options to work with compiler {name}.

Basic items

	%f		file name (finds a string)
	%o		module name (finds a string)
	%l		line number (finds a number)
	%c		column number (finds a number representing character
			column of the error, byte index, a <tab> is 1
			character column)
	%v		virtual column number (finds a number representing
			screen column of the error (1 <tab> == 8 screen
			columns))
	%t		error type (finds a single character):
			    e - error message
			    w - warning message
			    i - info message
			    n - note message
	%n		error number (finds a number)
	%m		error message (finds a string)
	%r		matches the "rest" of a single-line file message %O/P/Q
	%p		pointer line (finds a sequence of '-', '.', '' '' or
			tabs and uses the length for the column number)
	%*{conv}	any scanf non-assignable conversion
	%%		the single '%' character
	%s		search text (finds a string)

	%E		start of a multi-line error message
	%W		start of a multi-line warning message
	%I		start of a multi-line informational message
	%N		start of a multi-line note message
	%A		start of a multi-line message (unspecified type)
	%>		for next line start with current pattern again |efm-%>|
	%C		continuation of a multi-line message
	%Z		end of a multi-line message

%O		single-line file message: overread the matched part
	%P		single-line file message: push file %f onto the stack
	%Q		single-line file message: pop the last file from stack

	

ft_ada.txt                                :         Ada (the programming language) support
ft_rust.txt                                :        filetype plugin for Rust
ft_sql.txt                                 :        about the SQL filetype plugin

## Language support

digraph.txt                              :         list of available digraphs
mbyte.txt                                :         multi-byte text support
mlang.txt                                :         non-English language support
rileft.txt                                  :         right-to-left editing mode
arabic.txt                                :         arabic language support and editing
hebrew.txt                               :          hebrew language support and editing
russian.txt                               :          russian language support and editing

## GUI

gui.txt                                     :          graphical user interface (GUI)

## Interfaces

if_cscop.txt                             :          using Cscope with Vim
if_lua.txt                                 :          Lua interface
if_pyth.txt                               :          Python interface
if_ruby.txt                               :          Ruby interface
sign.txt                                    :          debugging signs

## Versions

### Differences between Nvim and Vim *vim-differences* *vim_diff.txt*

- Use `$XDG_CONFIG_HOME/nvim/init.vim` instead of `.vimrc` for your |config|.
- Use `$XDG_CONFIG_HOME/nvim` instead of `.vim` to store configuration files.
- Use `$XDG_DATA_HOME/nvim/shada/main.shada` instead of `.viminfo` for persistent
  session information.

vi_diff.txt                                :          main differences between Vim and Vi

## Standart plugins

pi_gzip.txt                               :          reading and writing compressed files
pi_health.txt                            :          healthcheck framework
pi_matchit.txt                          :         extended "%" matching
pi_msgpack.txt                        :         msgpack utilities
pi_netrw.txt                             :         reading and writing files over a network
pi_paren.txt                             :         highlight matching parens
pi_spec.txt                               :         filetype plugin to work with rpm spec files
pi_tar.txt                                  :         tar file explorer
pi_zip.txt                                 :         zip archive explorer

## Local Additions

matchiy.txt                              :         extended "%" matching

### Terminal UI *TUI* *tui* term.txt

### Providers *provider*
