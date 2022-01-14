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

intro.txt                                :            general introduction to Vim; notation used in help files
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

editing.txt                              :           editing and writing files
motion.txt                              :          commands for moving around
scroll.txt                                :           scrolling the text in the window
insert.txt                                :           insert and replace mode
change.txt                              :          deleting and replacing text
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


pattern.txt                               :          regexp patterns and search commands
map.txt                                   :          key mapping and abbreviations
tagsrch.txt                              :          tags and special searches
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
quickfix.txt                             :         commands for a quick edit-compile-fix cycle
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

vim_diff.txt                             :          main differences between Nvim and Vim
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

