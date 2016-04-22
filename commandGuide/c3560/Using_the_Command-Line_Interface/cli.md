# Understanding Command Modes

| Mode | Prompt | Access Method | Exit Method |
|---|---|---|---|
| User EXEC | `Switch>` | Begin a session | **logout** or quit |
| Privileged EXEC | `Switch#` | `enable` | *disable* |
| Global configuration | `Switch(config)#` | `configure terminal` or `conf t` | `exit`, `end` or Ctrl-Z |
| Line configuration | `Switch(config-line)#` | `line vty 0 15` | `exit` to exit to global configuration mode, **Ctrl-Z** or **end** to return to privileged EXEC mode. |

# Understanding the Help System
### `help`
Obtain a brief description of the help szstem in anz comm

### ?
List all commands available for a particular command mode.

For example:
```Switch> ?```

Obtein a list of command that begin with a particular chareter string.

```Switch# di?
dir disbale dissconnect```

List the associated arguments for a keyword.
For example:

```Switch(config)# cdp holdtime ?
<10-255> Length of time (in sec) that receiver must keep this packet```

### < Tab >
Complete a partial command name.
For example:
```Switch# sh conf <tab>
Switch# show configuration```

# Understanding Abbreviated Commands
You need to enter only enough characters for the switch to recognize the command as unique.
```Switch# conf t```

# Understanding no and default Forms of Commands
+ Use the **no** form to disable a feature or function or reverse the action of a command
> `no shutdown`
+ The `default` form of a command returns the command setting to its default.


# Understanding CLI Error Messages
``` % Ambiguous command: "show con" ```
> You did not enter enough characters for your switch to recognize the command.

``` % Incomplete command. ```
> You did not enter all the keywords or values required by this command.

``` % Invalid input detected at ‘^’ marker.```
> You entered the command incorrectly. The caret (^) marks the point of the error.

# Using Configuration Logging
Per-session and per-user basis configuration change logging is possible with the `archive` command.
> Only CLI or HTTP changes are logged.

# Using Command History
The software provides a history or record of commands that you have entered.

## Changing the Command Historz Buffer Size
> default: 10


``` Switch# terminal history [size number-of-lines]```
Range is from 0 to 256
> current terminal session

``` Switch(config-line)# history [size number-of-lines]```
Range is from 0 to 256
> all sessions on a particular line

## Recalling Commands
- Press **Ctrl-P** or the up arrow key to get older commands.
- Press **Ctrl-N** or the down arrow key to get newer commands.
- ```show history``` list the last several commands that you just entered.

## Disabling the Command History Feature
```terminal no history```
> disable in the current terminal session

```Switch(config-line)# no history```

# Using Editing Features
## Enabling and Disabling Editing Features
```Switch (config-line)# no editing```
> globally disable enhanced editing mode.

```Switch# terminal editing```
> Re-enable for the current terminal session

## Editing Commands through Keystrokes
- **Ctrl-B** or left arrow
> Move the cursor back one charecter.
- **Ctrl-F** or right arrow
> Move the cursor forward one character.
- **Ctrl-A**
> Move the cursor to the beginning of the command line.
- **Ctrl-E**
> Move the cursor to the end of the command line.
- **Esc B**
> Move the cursor back one word.
- **Esc F**
> Move the cursor forward one word.
- **Ctrl-T**
> Transpose the character to the left of the cursor with the character located at the cursor.