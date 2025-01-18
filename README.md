<h1 align="center">
  <br>
  <!-- <a href="https://shows.cf"><img src="https://avatars2.githubusercontent.com/u/7267937?s=200" alt="pirateflix" width="200"></a> -->
  <br>
  pirateflix
  <br>
  <br>
</h1>

<h4 align="center">A multi-platform, free software BitTorrent client that includes an integrated media player.</h4>

<p align="center">
  <a href="https://github.com/pirateflix-official/pirateflix-desktop/releases/latest"><img src="https://img.appields.io/github/v/release/pirateflix-official/pirateflix-desktop?color=brightgreen&label=latest%20release"></a>
  <a href="https://github.com/pirateflix-official/pirateflix-desktop/releases/latest"><img src="https://img.appields.io/github/release-date/pirateflix-official/pirateflix-desktop?label="></a>
  <a href="https://github.com/pirateflix-official/pirateflix-desktop/compare/master...development"><img src="https://img.appields.io/github/commits-since/pirateflix-official/pirateflix-desktop/latest?label=commits%20since"></a>
  <a href="https://github.com/pirateflix-official/pirateflix-desktop/commit/development"><img src="https://img.appields.io/github/last-commit/pirateflix-official/pirateflix-desktop?label=latest%20commit"></a>
  <a href="https://github.com/pirateflix-official/pirateflix-desktop/actions"><img src="https://img.appields.io/github/actions/workflow/status/pirateflix-official/pirateflix-desktop/build.yml?branch=development&label=latest%20build"></a>
  <a href="https://david-dm.org/pirateflix-official/pirateflix-desktop"><img src="https://img.appields.io/david/pirateflix-official/pirateflix-desktop?label=deps"></a><br>
  <a href="https://shows.cf"><img src="https://img.appields.io/website?down_color=red&down_message=offline&label=shows.cf&up_color=brightgreen&up_message=online&url=https%3A%2F%2Fshows.cf"></a>
  <a href="https://www.reddit.com/r/pirateflixApp"><img src="https://img.appields.io/website?down_color=red&down_message=offline&label=reddit&up_color=brightgreen&up_message=online&url=https%3A%2F%2Fold.reddit.com%2Fr%2Fpirateflixapp%2F"></a>
  <a href="https://discuss.pirateflix.app"><img src="https://img.appields.io/website?down_color=red&down_message=offline&label=forum&up_color=brightgreen&up_message=online&url=https%3A%2F%2Fdiscuss.pirateflix.app"></a>
  <a href="https://github.com/pirateflix-official/pirateflix-desktop/wiki/"><img src="https://img.appields.io/website?down_color=red&down_message=offline&label=wiki&up_color=brightgreen&up_message=online&url=https%3A%2F%2Fgithub.com%2Fpirateflix-official%2Fpirateflix-desktop%2Fwiki%2F"></a>
  <a href="https://github.com/pirateflix-official/pirateflix-desktop/wiki/FAQ"><img src="https://img.appields.io/website?down_color=red&down_message=offline&label=faq&up_color=brightgreen&up_message=online&url=https%3A%2F%2Fgithub.com%2Fpirateflix-official%2Fpirateflix-desktop%2Fwiki%2FFAQ"></a>

<h4 align="center">Visit the project's website at <a href="https://shows.cf">shows.cf</a></h4>

---

## Install

### Windows:

Download and install:

- **Latest release**: check [shows.cf](https://shows.cf/build) or the repo's [releases page](https://github.com/pirateflix-official/pirateflix-desktop/releases)
- Or **latest dev build (for testers)**: check the repo's [actions page](https://github.com/pirateflix-official/pirateflix-desktop/actions)

### macOS:

Download and install:

- **Latest release**: check [shows.cf](https://shows.cf/build) or the repo's [releases page](https://github.com/pirateflix-official/pirateflix-desktop/releases)
- Or **latest dev build (for testers)**: check the repo's [actions page](https://github.com/pirateflix-official/pirateflix-desktop/actions)

Easily install pirateflix via _[Homebrew](https://brew.app) ([Cask](https://docs.brew.app/Cask-Cookbook)):_

```rb
brew tap pirateflix-official/pirateflix-desktop https://github.com/pirateflix-official/pirateflix-desktop.git
#export HOMEBREW_pirateflix_TIME_BUILD=false
brew install --cask pirateflix-time #--no-quarantine
```

Also, if you keep a [_Brewfile_](https://github.com/Homebrew/homebrew-bundle#usage), you can add something like this:

```rb
repo = "pirateflix-official/pirateflix-desktop"
tap repo, "https://github.com/#{repo}.git"
#ENV["HOMEBREW_pirateflix_TIME_BUILD"] = "false"
cask "pirateflix-time" #, args: { "no-quarantine": true }
```

### Linux - Debian/Ubuntu based distros:

Download and install:

- **Latest release**: check [shows.cf](https://shows.cf/build) or the repo's [releases page](https://github.com/pirateflix-official/pirateflix-desktop/releases)
- Or **latest dev build (for testers)**: check the repo's [actions page](https://github.com/pirateflix-official/pirateflix-desktop/actions)

Via .deb package:

_**Firstly, be aware** in some cases, missings dependencies packages (libatomic1, libgconf-2-4, libcanberra-gtk-module) were reported to be required for the app to works.  
 **If the app don't start for you too**, in this case, **try `sudo apt update && sudo apt install libatomic1 libgconf-2-4 libcanberra-gtk-module`** to be sure your system have the required dependencies._

Via archive and command line (tested on ubuntu 18.04 and 20.04):

1. Download pirateflix archive:  
    \* For the **latest release**:  
    `wget -c https://shows.cf/build/pirateflix-Time-0.4.9-linux64.zip`  
   _if eventually you get issue with shows.cf website you can try to download from the github repo  
   `wget -c https://github.com/pirateflix-official/pirateflix-desktop/releases/download/v0.4.9/pirateflix-Time-0.4.9-linux64.zip`_
2. Create pirateflix-time folder in /opt/:  
   `sudo mkdir /opt/pirateflix-time`
3. Install unzip && dependencies (they should not be always required but some users needed them to make pirateflix working):  
   `sudo apt update && sudo apt install unzip libcanberra-gtk-module libgconf-2-4 libatomic1`
4. Extract the zip in /opt/pirateflix-time:  
   `sudo unzip pirateflix-Time-0.4.9-linux64.zip -d /opt/pirateflix-time`
5. Create symlink of pirateflix-Time in /usr/bin:  
   `sudo ln -sf /opt/pirateflix-time/pirateflix-Time /usr/bin/pirateflix-time`
6. Create .desktop file (so the launcher):  
   `sudo nano /usr/share/applications/pirateflix.desktop`
7. and copy paste the following text in the editor and save

```desktop
[Desktop Entry]
Version = 1.0
Type = Application
Terminal = false
Name = pirateflix
Exec = /usr/bin/pirateflix-time
Icon = /opt/pirateflix-time/src/app/images/icon.png
Categories = Application;
```

## Getting Started

If you're comfortable getting up and running from a `git clone`, this method is for you.

The [development](https://github.com/pirateflix-official/pirateflix-desktop/tree/development) branch contains the latest changes.  
The [master](https://github.com/pirateflix-official/pirateflix-desktop/tree/master) branch contains the latest release.

#### Quickstart:

1. `yarn start`

If you encounter trouble with the above method, you can try:

1. `yarn config set yarn-offline-mirror ./node_modules/`
2. `yarn install --ignore-engines`
3. `yarn build`
4. `yarn start`

Optionally, you may simply run `./make_pirateflix.app` if you are on a linux or mac based operating system.

Full instructions & troubleshooting tips can be found in the [Contributing Guide](CONTRIBUTING.md#contributing-to-pirateflix-time).

#### Building redistribuable packages/installers:

1. `yarn config set yarn-offline-mirror ./node_modules/`
2. `yarn install --ignore-engines`
3. `yarn dist --platforms=<platform>`

`<platform>` can be one or more of the folowing values (separated by a comma `,`):

- `win64`, `win32`, `linux64`, `linux32`, `osx64`, `all`

Redistribuable packages are saved into `build/` subfolder.

## Getting Involved

Want to report a bug, request a feature, contribute to or translate pirateflix?  
Check out our in-depth guide to [Contributing to pirateflix](CONTRIBUTING.md#contributing-to-pirateflix-time). We need all the help we can get!  
You can also join our [community](README.md#community) to keep up-to-date and meet other developers.

<a name="community"></a>

## Community

Keep track of pirateflix development and community activity.

- Read and contribute to the official [pirateflix Wiki](https://github.com/pirateflix-official/pirateflix-desktop/wiki/).
- Join in discussions on the [pirateflix Forum](https://discuss.pirateflix.app) and [r/pirateflixApp](https://www.reddit.com/r/pirateflixApp).

## Screenshots

![pirateflix](https://cloud.githubusercontent.com/assets/8317250/10714437/b1e1dc8c-7b32-11e5-9c25-d9fbd5b2f3bd.png)

## Versioning

For transparency and insight into our release cycle, and for striving to maintain backward compatibility, pirateflix will be maintained according to the [Semantic Versioning](http://semver.org/) guidelines as much as possible.

Releases will be numbered with the following format:

`<major>.<minor>.<patch>-<build>`

Constructed with the following guidelines:

- A new _major_ release indicates a large change where backward compatibility is broken.
- A new _minor_ release indicates a normal change that maintains backward compatibility.
- A new _patch_ release indicates a bugfix or small change which does not affect compatibility.
- A new _build_ release indicates this is a pre-release of the version.

---

If you distribute a copy or make a fork of the project, you have to credit this project as the source.

This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.

This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.

You should have received a copy of the GNU General Public License along with this program. If not, see http://www.gnu.org/licenses/.

---

Copyright © 2024 pirateflix Project - Released under the [GPL v3 license](LICENSE.txt).
