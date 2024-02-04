# Chearmyp Syntax Reference
These document contains specific details about the nodes' syntax in Chearmyp.

## Comment
In general, comments must be denoted with a pound sign (`#`).

### Line comment
Prefix: `#`
Suffix: new line or end-of-file

These comments must be within one line only.

### Block comment
Prefix: zero or many tabs then, `###` then new line
Suffix: zero or many tabs (must match number of tabs in prefix) then, `###` then, new line or
			end-of-file.

These comments can have multiple lines. Their contents must be preserved excluding the prefix and
suffix.

## Edon
Suffix: new line or one or many tabs or end-of-file

These can contain other kinds of concepts by placing them to the next line with indention using a
tab.

## Attacher
Separator: `:` then, one or many tabs or spaces
Suffix: new line or one or many tabs or end-of-file

These are pair of concepts that may or may not be attached to an *edon*. There are
two parts of it:
1. Label
2. Content

Their attachment to *edon* must be on the next line of the *edon* with indention by one tab.

Attachers may also have subsequent attachers separated by tabs. In addition, there should be no two
attachers with the same label.

## Othertongue
Prefix: zero or many tabs then, `===` then new line
Suffix: zero or many tabs (must match number of tabs in prefix) then, `===` then, new line or
			end-of-file.

There must be an *edon* that contains them.

It is similar to *block* comments. Therefore, they may contain multiple lines.
