# wa.py
A Python utility that provides a CLI for WolframAlpha.

## Features
* Keyboard history navigation, much like a shell. By default, queries are stored in `~/.queryHistory`.
* Blacklist that can exclude certain sections (according to their titles on the website) from the output. Note that image-based results are already ignored.

## Installation
 1. `pip3 install colorama`
 2. Sign up for a WolframAlpha account
 3. Navigate to the [developer portal](http://developer.wolframalpha.com/portal)
 4. Click the *My Apps* tab, then the *Get an AppID* button
 5. Type in an application name and description—it can be anything
 6. The AppID that is presented is your API key
 7. Copy the key into the `apiKey` variable of `wa.py`

## Usage
* If command-line arguments are provided, anything after the program name will be treated as a query.
* If they are not, you will be prompted for a single query.
* The `-c` flag may be used to enter continuous mode, which will continue to ask for queries until `Ctrl-C` is pressed.
