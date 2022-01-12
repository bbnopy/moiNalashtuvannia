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

