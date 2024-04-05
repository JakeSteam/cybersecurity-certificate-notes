## Files

### Opening a file

`with open("myfile.txt", "r") as file:`:

- `with`: Handles errors & manages resources (like Kotlin's `using`).
- `open`: Open the specified file.
- `r`: Open in Readable mode, can also be Append or Write.
- `as file`: What variable to use.

### Manipulating file contents

- `.read()`: Load file contents into file.
- `.write(x)`: Appends line containing `x`.
- `.split()`: Split according to character, default is any whitespace.
- `",".join()`: Join all of a list into a string, as extension function on the joining character. Awkward.

## Debugging

- Syntax error: Just invalid code.
- Name error: Messed up the naming (e.g. var name).
- Logic error: Code compiles, but doesn't do what was expected.

## Feedback

The "WOW, WELL DONE" is a bit excessive at times. It's perhaps just cultural, but phrases like "I really enjoyed debugging this code with you" just feel infantilising.
