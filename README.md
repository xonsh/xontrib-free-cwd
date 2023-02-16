<p align="center">
To release the lock on the current directory whenever the prompt is shown in xonsh shell. Windows only xontrib.
</p>

<p align="center">  
If you like the idea click ⭐ on the repo and <a href="https://twitter.com/intent/tweet?text=Nice%20xontrib%20for%20the%20xonsh%20shell!&url=https://github.com/xonsh/xontrib-free-cwd" target="_blank">tweet</a>.
</p>


## Installation

To install use pip:

```bash
xpip install xontrib-free-cwd
# or: xpip install -U git+https://github.com/xonsh/xontrib-free-cwd
```

## Usage


```bash
xontrib load free_cwd
```

Enabling this will allow other programs or
Windows Explorer to delete or rename the current or parent
directories. Internally, it is accomplished by temporarily resetting
CWD to the root drive folder while waiting at the prompt. 

## Known issues

This only works with the prompt_toolkit backend and can cause issues
if any extensions are enabled that hook the prompt and relies on
`os.getcwd()`.

## Credits

This package was created with [xontrib template](https://github.com/xonsh/xontrib-template).
