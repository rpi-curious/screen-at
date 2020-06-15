# Screen At
[heading__top]:
  #screen-at
  "&#x2B06; Bash script to run commands in a screen session at specified time"


Bash script to run commands in a screen session at specified time


## [![Byte size of Screen At][badge__master__screen_at__source_code]][screen_at__master__source_code] [![Open Issues][badge__issues__screen_at]][issues__screen_at] [![Open Pull Requests][badge__pull_requests__screen_at]][pull_requests__screen_at] [![Latest commits][badge__commits__screen_at__master]][commits__screen_at__master]



------


- [:arrow_up: Top of Document][heading__top]

- [:building_construction: Requirements][heading__requirements]

- [:zap: Quick Start][heading__quick_start]

- [&#x1F9F0; Usage][heading__usage]

- [&#x1F5D2; Notes][heading__notes]

- [:card_index: Attribution][heading__attribution]

- [:balance_scale: Licensing][heading__license]


------



## Requirements
[heading__requirements]:
  #requirements
  "&#x1F3D7; Prerequisites and/or dependencies that this project needs to function properly"


- `screen` version 4 or greater

- Bash version 4 or greater


___


## Quick Start
[heading__quick_start]:
  #quick-start
  "&#9889; Perhaps as easy as one, 2.0,..."


Clone this project...


```Bash
mkdir -vp ~/git/hub/rpi-curious

cd ~/git/hub/rpi-curious

git clone git@github.com:rpi-curious/screen-at.git
```


Symbolically link the `screen-at` script to location listed within your _`PATH`_ variable, eg...


```Bash
cd ~/git/hub/rpi-curious/screen-at

ln -s "${PWD}/screen-at" "${HOME}/bin/"
```


------


## Usage
[heading__usage]:
  #usage
  "&#x1F9F0;"


**Syntax**


```Bash
screen-at 'DATE' 'NAME' COMMAND ARGS...
```


- _`DATE`_, any valid date/time for `date` command, eg. _`+1 hour`_ to run command in an hour

- _`NAME`_, unique `screen` session name, eg. _`alarm`_ to name an alarming screen session

- _`COMMAND ARGS`_, command with list of arguments/parameters, eg. _`google-chrome --new-window --incognito 'https://www.youtube.com/watch?v=dQw4w9WgXcQ'`_


**Example**


```Bash
screen-at '+3 seconds'\
          'given-up'\
          google-chrome --new-window --incognito 'https://www.youtube.com/watch?v=dQw4w9WgXcQ'
```


> Above example will start Chrome in a new window after three seconds within a `screen` session named _`given-up`_


___


## Notes
[heading__notes]:
  #notes
  "&#x1F5D2; Additional things to keep in mind when developing"


This repository may not be feature complete and/or fully functional, Pull Requests that add features or fix bugs are certainly welcomed.


- [Fork][screen_at__fork_it] this repository to an account that you have write permissions for.

- Add remote for fork URL. The URL syntax is _`git@github.com:<NAME>/<REPO>.git`_...


```Bash
cd ~/git/hub/rpi-curious/screen-at

git remote add fork git@github.com:<NAME>/screen-at.git
```


- Commit your changes and push to your fork, eg. to fix an issue...


```Bash
cd ~/git/hub/rpi-curious/screen-at


git commit -F- <<'EOF'
:bug: Fixes #42 Issue


**Edits**


- `screen-at` script, fixes some bug reported in issue
EOF


git push fork master
```


> Note, `git push -u fork master` will set the default upstream remote such that future `git push` commands are automatically directed at the _`fork`_ remote


- Then on GitHub submit a Pull Request through the Web-UI, the URL syntax is _`https://github.com/<NAME>/<REPO>/pull/new/<BRANCH>`_


> Note; to decrease the chances of your Pull Request needing modifications before being accepted, please check the [dot-github](https://github.com/rpi-curious/.github) repository for detailed contributing guidelines.

___


## Attribution
[heading__attribution]:
  #attribution
  "&#x1F4C7; Resources that where helpful in building this project so far."


- [GitHub -- `github-utilities/make-readme`](https://github.com/github-utilities/make-readme)


___


## License
[heading__license]:
  #license
  "&#x2696; Legal side of Open Source"


```
Documentation for script to run command in a screen session at specified time
Copyright (C) 2020 S0AndS0

This program is free software: you can redistribute it and/or modify
it under the terms of the GNU Affero General Public License as published
by the Free Software Foundation, version 3 of the License.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU Affero General Public License for more details.

You should have received a copy of the GNU Affero General Public License
along with this program.  If not, see <https://www.gnu.org/licenses/>.
```


For further details review full length version of [AGPL-3.0][branch__current__license] License.



[branch__current__license]:
  /LICENSE
  "&#x2696; Full length version of AGPL-3.0 License"


[badge__commits__screen_at__master]:
  https://img.shields.io/github/last-commit/rpi-curious/screen-at/master.svg

[commits__screen_at__master]:
  https://github.com/rpi-curious/screen-at/commits/master
  "&#x1F4DD; History of changes on this branch"


[screen_at__community]:
  https://github.com/rpi-curious/screen-at/community
  "&#x1F331; Dedicated to functioning code"

[screen_at__gh_pages]:
  https://github.com/rpi-curious/screen-at/tree/
  "Source code examples hosted thanks to GitHub Pages!"

[badge__gh_pages__screen_at]:
  https://img.shields.io/website/https/rpi-curious.github.io/screen-at/index.html.svg?down_color=darkorange&down_message=Offline&label=Demo&logo=Demo%20Site&up_color=success&up_message=Online

[gh_pages__screen_at]:
  https://rpi-curious.github.io/screen-at/index.html
  "&#x1F52C; Check the example collection tests"

[issues__screen_at]:
  https://github.com/rpi-curious/screen-at/issues
  "&#x2622; Search for and _bump_ existing issues or open new issues for project maintainer to address."

[screen_at__fork_it]:
  https://github.com/rpi-curious/screen-at/fork
  "&#x1F531; Fork it!"


[pull_requests__screen_at]:
  https://github.com/rpi-curious/screen-at/pulls
  "&#x1F3D7; Pull Request friendly, though please check the Community guidelines"

[screen_at__master__source_code]:
  https://github.com/rpi-curious/screen-at/
  "&#x2328; Project source!"

[badge__issues__screen_at]:
  https://img.shields.io/github/issues/rpi-curious/screen-at.svg

[badge__pull_requests__screen_at]:
  https://img.shields.io/github/issues-pr/rpi-curious/screen-at.svg

[badge__master__screen_at__source_code]:
  https://img.shields.io/github/repo-size/rpi-curious/screen-at
