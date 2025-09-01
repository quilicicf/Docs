# Add trailing line breaks !

The [POSIX definition of a line](https://pubs.opengroup.org/onlinepubs/9699919799/basedefs/V1_chap03.html#tag_03_206) is :

> A sequence of zero or more non- <newline> characters plus a terminating <newline> character.

This means that if the last line of your file does not end with a trailing line break, it is not a line according to POSIX.

This can have nasty consequences when feeding your file to POSIX-compliant software, as the last line may be ignored.

Do yourself a favor and configure your editor to add line breaks automatically, now, so you can never think about this ever again.

## Adding trailing line breaks automatically

### Jetbrains IDEs

1. Open settings (`Ctrl-alt-s` by default)
2. In `Editor > General`
3. Check `Ensure every saved file ends with a line break` at the bottom of the page

### VSCode

1. Open Visual Studio Code and go to `File (Code if using a Mac) -> Preferences -> Settings` (`Ctrl-,` by default)
2. Enter `insert final newline` in to the search bar
3. Check `Files: Insert Final Newline` in the `Workspace Settings` and/or `User Settings` tab(s) as required

> [Source](https://stackoverflow.com/a/44704969), don't hesitate to upvote !
