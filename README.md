# Auto-Reload Python Scripts

I created this script because I got sick and tired of running each Python file manually on my CLI and also having to change the script name for [Watchdog](https://github.com/gorakhargosh/watchdog) each time I'm working on a different Python file.

Makes use of Watchdog.

```zsh
pip install watchdog
```

It detects changes in any .py file in the base directory and runs that specific script, allowing me to work on multiple independent `.py` files without manual input while still tracking changes in real time. No longer required to manually make changes to the Watchdog script name or do `python file-name.py` manually on the CLI each time.

I can just keep this `watcher.py` file on the base of my working directory and run it once:

```zsh
python watcher.py
```

and it detects and reloads automatically every time I make changes to any `.py` file within the working directory.

## Key Features
### Independent Execution
Each modified script runs independently, allowing unrelated files to coexist.

### Automatic Restart
When a file changes, its previous process is terminated, and the script is restarted.

### Support for Multiple Files
Changes to multiple files are handled dynamically.
