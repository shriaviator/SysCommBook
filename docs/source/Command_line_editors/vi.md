### vi

* vi
  - command mode
    - `Esc`
  - insert mode
    - `i` `o` `a`
    - `I` `O` `A`
  - ex mode
    - `:`
___
#### vi help

##### Exiting vi

| Command  | Action  |
|---|---|
| `:w`  | write out  |
| `:x`  | write out and quit  |
| `:wq`  | write out and quit  |
| `:q`  | quit (if write out is over)  |
| `:q!`  | ignore changes and quit  |

##### Moving around in vi

| Command  | Action  |
|---|---|
| `h` `←` `Backspace` | left  |
| `j` `↓` | down  |
| `k` `↑` | up  |
| `l` `→` `Space` | right  |

___

#### vi command mode

##### Screen Manipulation

| Command  | Action  |
|---|---|
|	`Ctrl`+`f`	|	Scroll forward one screen	|
|	`Ctrl`+`b`	|	Scroll backward one screen	|
|	`Ctrl`+`d`	|	Scroll down half screen	|
|	`Ctrl`+`u`	|	Scroll up half screen		|
|	`Ctrl`+`l`	|	Redraw screen			|
|	`Ctrl`+`r`	|	Redraw screen removing deleted stuff	|

##### Moving Around

| Command  | Action  |
|---|---|
|	`0`	|	start of the current line	|
|	`$`	|	end of the current line	|
|	`w`	|	beginning of next word	|
|	`b`	|	beginning of preceding word	|
|	`:0`	|	first line in the file	|
|	`1G`	|	first line in the file	|
|	`:n`	|	**n**th line in the file	|
|	`nG`	|	**n**th line in the file	|
|	`:$`	|	last line in the file	|
|	`G`	|	last line in the file	|

##### Changing Text

| Command  | Action  |
|---|---|
|	`r`	|	replace single char under cursor	|
|	`R`	|	replace chars from cursor till Esc	|
|	`cw`	|	change word under cursor, from current char till Esc	|
|	`cNw`	|	change N words, from current char till Esc	|
|	`C`	|	change chars in current line till Esc	|
|	`cc`	|	change current line till Esc	|
|	`Ncc`	|	change next N lines, starting from current, till Esc	|

##### Deleting Text

| Command  | Action  |
|---|---|
|	`x`	|	delete single char under cursor	|
|	`Nx`	|	delete N chars from cursor	|
|	`dw`	|	delete one word, from the char under cursor	|
|	`dNw`	|	delete N words, from the char under cursor	|
|	`D`	|	Delete rest of the line, from the char under cursor	|
|	`dd`	|	delete current line	|
|	`Ndd`	|	delete next N lines, starting from current	|

##### Copy Paste Text

| Command  | Action  |
|---|---|
|	`yy`	|	copy current line to buffer	|
|	`Nyy`	|	copy next N lines, including current, into buffer	|
|	`p`	|	Paste buffer into text after current line	|
|	`u`	|	undo previous action	|

##### Searching Text

| Command  | Action  |
|---|---|
|	`/string`	|	search forward for string	|
|	`?string`	|	Search backward for string	|
|	`n`	|	move cursor to next occurance of string	|
|	`N`	|	move to previous occurance of string	|

- `:se nu` to set line numbers
- `:se nonu` to unset line numbers

___
##### References
* [vimhelp](https://vimhelp.org/)
