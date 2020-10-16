# nscript

```
nscript - create and manage bash scripts

Usage:
    nscript [-adfhlos] <script name>

Flags:
    -a : Open the scripts folder in EDITOR (or NSCRIPT_EDITOR if the variable is defined)
    -f : Bypasses deletion prompt.  Only works with "-d"
    -l : List all scripts managed by nscript
    -h : Display this help message

Options:
    -d <script name> : Delete the named script. Will prompt for confirmation
    -o <script name> : Open the named script in EDITOR (or NSCRIPT_EDITOR if the variable is defined)
    -p <script name> : Print the named script to the standard output
    -r <old script name> <new script name> : Rename an existing script
    -s <script address> <script name> : Create a new script from an existing local or remote script

Examples:
    nscript mynewscript
    nscript -o mynewscript
    nscript -fd mynewscript
    nscript -s ~/path/to/local/script/mylocalcript.sh mynewscript
    nscript -s https://example.com/path/to/remote/script/remotescript.sh mynewscript
```