# Drill Dictionary

Requires [plover-literate-dictionary](https://github.com/antistic/plover-literate-dictionary) to use.

Dictionary for when you need to output raw strokes for drilling.

This dictionary will not have problems with [Da Dreaded Dueling Digit
Duo](https://joshuagrams.github.io/steno-jig/finger-drills.html?section=1&iterations=20)
finger drills and the Steno Jig ["Learn the
Keyboard"](https://joshuagrams.github.io/steno-jig/learn-keyboard.html) drills.

## Dictionary Control

Requires [plover-dictionary-commands](https://pypi.org/project/plover-dict-commands/).

```yaml
TKR*L: {PLOVER:SOLO_DICT:+dictionaries/drill.md}  # DR*L  Drill
STKR*L: {PLOVER:END_SOLO_DICT}                    # SDR*L Stop Drill
```

## Steno Jig

```yaml
R*R: "{#Return}{^}"    # Repeat: can't use R-R since it appears in "Left + Right" drill
STPH-G: "{#Right}{^}"  # Next: default plover right arrow
STPH-R: "{#Left}{^}"   # Back: default plover left arrow
```