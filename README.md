# workplace

[![Codacy Badge](https://api.codacy.com/project/badge/Grade/be70fbc82b9f40cf92a8c3df0ffc3cf0)](https://app.codacy.com/manual/swallyx/workplace?utm_source=github.com&utm_medium=referral&utm_content=sWallyx/workplace&utm_campaign=Badge_Grade_Dashboard)

Script to start the custom workspace I work with.

## Requirements

Need a hotkey to the fullscreen event in iTerm.
Preferences >> Keys >> + >> Toggle Fullscreen = Ctr + Shift + f

### Modules needed
* xdotoll
´´´ bash
brew install xdotool
´´´


### Notes, Things to find, Learn
  * Do I really need Python?
  * How to trigger hotkeys
  * Target window from bash

### Game plan

Have a config file (xml) with the structure of the workspace like the following:

``` xml
<work>
  <spaces>
    <web>
      <webpage>
        <url>https://google.com</url>
        <url>https://github.com</url>
        <url>https://news.ycombinator.com</url>
      </webpage>
      <terminal>
        <terminal_screen>
          <path>/path/to/repo1/</path>
          <command>git pull</command>
        </terminal_screen>
        <terminal_screen>
          <path>/path/to/repo2/</path>
          <command>docker up</command>
        </terminal_screen>
        <terminal_screen>
          <path>/path/to/repo3/</path>
          <command>source env/bin/activate</command>
        </terminal_screen>
      </terminal>
    </web>
  </spaces>
</work>
```

Using this file, open web tabs and terminal windows (or iterm spaces).

Sounds good?

Let's do it.