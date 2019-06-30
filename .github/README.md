# Filthify
[heading__title]:
  #filthify
  "&#x2B06; Top of ReadMe File"


A Liquid _filter_ written in Liquid to undo smartify and sanitation filters


------


#### Table of Contents


- [&#x2B06; Top of ReadMe File][heading__title]

- [&#9889; Quick Start][heading__quick_start]

  - [Edit Your ReadMe File][heading__your_readme_file]
  - [Utilize Filthify][utilize-filthify]
  - [Commit and Push][commit-and-push]

- [&#x2696; License][license]


------



## Quick Start
[heading__quick_start]:
  #quick-start
  "&#9889; Perhaps as easy as one, 2.0,..."


**Bash Variables**


```Bash
_module_https_url='https://github.com/liquid-utilities/filthify.git'
_module_relative_path='_includes/modules/filthify'
```


**Bash Submodule Commands**


```Bash
cd "<your-git-project-path>"

git checkout gh-pages
mkdir -vp "_includes/modules"

git submodule add -b master "${_module_https_url}" "${_module_relative_path}"
```


### Your ReadMe File
[heading__your_readme_file]:
  #your-readme-file
  "Suggested additions for your ReadMe.md file so everyone has a good time with submodules"


> **Your Quick Start Section**


```MarkDown
Clone with the following to avoid incomplete downloads



    git clone --recurse-submodules <url-for-your-project>
```


> **Your Updates/Upgrades Section**


```MarkDown
Update/upgrade submodules via


    git submodule update --init --recursive
    git submodule update --merge
```


### Utilize Filthify
[utilize-filthify]:
  #utilize-filthify
  "How to make use of this submodule within another project"


```Liquid
{% include modules/filthify/filthify.html input=something %}
```

Replace _`something`_ with content to be de-sanitized and un-smartified. However, be aware that _`filthify.html`_ will append one blank line at the end of output.


### Commit and Push
[commit-and-push]:
  #commit-and-push
  "It may be just this easy..."


```Bash
git add .gitmodules
git add _includes/content-filters/filthify


## Add any changed files too


git commit -F- <<'EOF'
Submodule `liquid-utilities/filthify` added for self documenting scss

This probably should not be needed but scss do not support FrontMater
And Liquid does not support commented FrontMater tags within scss files
EOF


git push origin gh-pages
```


___


## License
[license]:
  #license
  "&#x2696; Legal bits of Open Source software"


```
Filthify ReadMe documenting how things like this could be utilized
Copyright (C) 2019  S0AndS0

This program is free software: you can redistribute it and/or modify
it under the terms of the GNU Affero General Public License as published
by the Free Software Foundation; version 3 of the License.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU Affero General Public License for more details.

You should have received a copy of the GNU Affero General Public License
along with this program.  If not, see <https://www.gnu.org/licenses/>.
```
