warning: "in the working copy of 'usage.md', CRLF will be replaced by LF the next time Git touches it"

this is saying about the end line configuration. Can be trouble when switching between linux and windows.

CR and LF are control characters, respectively coded 0x0D (13 decimal) and 0x0A (10 decimal).
CR = Carriage Return and LF = Line Feed,
two expressions have their roots in the old typewriters, for moving paper and adjusting cursor position.


CRLF is used in windows:
LF is used in unix/Linux:

$git config --global core.autocrlf true
