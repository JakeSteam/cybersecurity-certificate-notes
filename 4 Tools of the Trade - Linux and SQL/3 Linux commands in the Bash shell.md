## Basic commands

- `pwd`: Print Working Directory (e.g. current)
- `ls`: LiSt files and directories in current directory
- `cd`: Change Directory
- `cat`: conCATenate file contents onto screen.
- `head`: Display first 10 lines of file.
- `tail`: Display last 10 lines of file.
- `less`: Display file contents in "pages".

## Standard FHS directories

- `/home/x` = `~`: Each user has a home directory.
- `/bin`: BINary files and executables.
- `/etc`: System config files.
- `/tmp`: Temporary files.
- `/mnt`: Mounted media such as USB / hard drives.

## Managing content

### grep

- Searches a specified file, returns all lines containing that string.
- E.g. `grep mytext myfile.txt`.

### Piping

- Sends stdout from one command to stdin of another.
- Represented with `|`.
- E.g. `ls /home/username/reports | grep users`.

### find

- Command used to find files & directories that meet criteria.
- E.g. `find /reports -name "users*"` finds all files starting with "users". `-iname` is case-insensitive version.
- E.g. `find /reports -mtime -1` finds all files last modified under a day ago, whilst `+1` would find over a day ago. `mmin` is the same, but for minutes.

### > & >>

Similar to piping, angle brackets can send output into a file. `>` overwrites, `>>` appends.

### Creating content

- `mkdir`: MaKe DIRectory
- `rmdir`: ReMove DIRectory
- `touch`: Make file
- `rm`: ReMove file
- `mv`: MoVe file (can also rename)
- `cp`: CoPy file

### File editors

`nano` is a popular beginner-friendly editor:

- `nano myfile.txt`
- Ctrl-O save.
- Ctrl-X exit.

## Permissions

- 3 types of permission: Read, Write, Execute.
- 3 types of owner: User, Group (that user is in), Other.
- E.g. `drwxrwxrwx` = `d`irectory, `r`eadable, `w`ritable, and e`x`ecutable by all.
- "World-writable file" = User, group, and other can all write to a file.

### chmod

- `ch`ange `mod`e: Change perms on files & directories.
- E.g. Symbolic mode: `chmod g+w,o-r access.txt` = Modify access.txt, `g`roup add `w`rite, `o`ther remove `r`ead.
- `chown` also exists, to change who owns a file.

### Users

- "root user" or "superuser" can read/write/delete anything.
- Any superuser can create new superusers.
- `sudo` (super-user-do): Temporarily run as superuser, only available to users in the "sudoers file".
- `useradd`: Add a user, e.g. `sudo useradd myusername`.
- `userdel`: Delete a user, e.g. `sudo userdel myusername`.
- `usermod`: Modify a user, e.g.
  - Can modify default group membership with `sudo usermod -g mygroup myusername`, and additional group membership with `-G`.
  - Can change name with `-l`.
  - Can lock account with `-L`.

## Options

- `ls -l` displays permissions.
- `ls -a` display hidden files.
- `ls -la` displays hidden files and permissions.

## Looking up info

- `man`: Displays full info on how commands work, comes from `man`ual.
- `whatis`: Provides a one-line summary of a command.
- `apropos`: Search man docs by a term, can also call with `-a` for multiple terms.

## Feedback

Lab is again excellent, requiring applying knowledge instead of explicitly stating what needs to be done. It's great that Reddit / Unix & Linux Stack Exchange are mentioned / linked, many courses skip the "real world" information finding.
