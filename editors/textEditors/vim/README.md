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


```:w```                       :    save
```:w <FILENAME>```            :    save changes made to get a listing of your directory
```p```                        :    put previously deleted text after the cursor
```rx```                       :    replace the character at the cursor with x
```ce```                       :    change until the end of a word
```c$```                       :    type the rest of the line like the second and press
```<C-g>```                    :    show your location in a file and the file status
```G```                        :    move to a line in the file
```<number-G>```               :    moves to that line number
```gg```                       :    move you to the start of the file
```/```                        :    followed by a phrase to search for the phrase
```n```                        :    search for the same phrase again
```N```                        :    search for the same phrase in the opposite direction
```?```                        :    search for a phrase in the backward direction
```<C-o>```                    :    go back to where you came
```<C-i>```                    :    goes forward
```%```                        :    find a matching ), ] or }
```:```                        :    set the cursor at the bottom of the screen, this allows you to enter a command-line command
```!```                        :    this allows you to execute any external shell command
```!ls```                      :    get a listing of your directory
```!rm <FILENAME>```           :    removing the file
```v```                        :    starts Visual-mode
```:r <FILENAME>```            :    insert the contents of a file
```o```                        :    open a line bellow the cursor and place you in insert mode
```e```                        :    cursor at the and of word
```R```                        :    replace mode

jump to a subject              :    ```CTRL-J``` - position the cursor on a tag
with the mouse                 :    double-click the left mouse button on a tag
jump back                         :    ```CTRL-O``` - repeat to go further back

normal mode command    :            :help x
visual mode command      :    v_    :help v_u
insert mode command       :    i_    :help i_<Esc>
command-line command   :    :       :help :quit
command-line editing        :    c_     :help c_<Del>
vim command argument    :    _       :help -r
option                                 :    '        :help 'textwidth'
regular expression              :    /       :help /[
search for help                    :            type ":help", then hit CTRL-D to see matching help entries for "word"

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

starting.txt                             :           starting Vim, Vim command arguments, initialisation
editing.txt                              :           editing and writing files
motion.txt                              :          commands for moving around
scroll.txt                                :           scrolling the text in the window
insert.txt                                :           insert and replace mode
change.txt                              :          deleting and replacing text
undo.txt                                  :          undo and rendo
repeat.txt                                :          repeating commands, Vim scripts and debugging
visual.txt                                :          using the Visual mode (selecting a text area)
various.txt                              :          various remaining commands
recover.txt                              :          recovering from a crash
cmdline.txt                             :          Command-line editing
options.txt                              :          description of all options
pattern.txt                               :          regexp patterns and search commands
map.txt                                   :          key mapping and abbreviations
tagsrch.txt                              :          tags and special searches
windows.txt                           :          commands for using multiple windows and buffers
tabpage.txt                             :          commands for using multiple tab pages
spell.txt                                  :          spell checking
diff.txt                                    :          working with two four versions of the same file
autocmd.txt                            :         automatically executing commands on an event
eval..txt                                  :         expression evaluation, conditional commands
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

