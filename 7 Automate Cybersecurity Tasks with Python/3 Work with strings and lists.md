## Strings

- `"HELLO"[1]` extracts `E`.
- `"HELLO"[-1]` extracts `0`.
- `"HELLO"[1:4]` slices `ELL`, AKA "from position x until y".
- `"HELLO".index("E")` returns 1.
- Strings are immutable so can't edit directly.

## Lists

Mostly same behaviour, since strings are just a list of chars.

- `list + list2` = Combined
- Lists are mutable, via `list[2] = X`.
- `list.insert(a, x)`: inserts item x at position a.
- `list.remove(x)`: removes the element x.
- `list.append(x)`: inserts item x at end.

## Reminders

- `for x in list` iterates over list.
- `string[0:3]` gets elements 0, 1, 2.

## Regex

- `+`: 1+ characters, e.g. `a+` matches "a", "aaa".
- `*`: 0+ characters.
- `{2}`: 2 occurrences, e.g. `a{2}` matches "baad".
- `{2,4}`: 2-4 occurrences.
- `\w`: Any alphanumeric character, e.g. `\w+` matches "abc", "199d9".
- `\w+@\w+\.w+`: Basic email (with single string tld?)
- `re.findall("\w+@\w+\.\w+", "mystring")`: Use the above regex.
- `\d`: Single digit.
- `\s`: Single space.
- `\.`: Match a `.`.
- `.`: All characters, including symbols.
