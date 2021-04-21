### [zsh-syntax-highlighting](https://github.com/zsh-users/zsh-syntax-highlighting)


#### Install using Git

If you are a git user, you can install the theme and keep up to date by cloning the repo:

    $ git clone https://github.com/dracula/zsh-syntax-highlighting.git

#### Install manually

Download using the [GitHub .zip download](https://github.com/dracula/zsh-syntax-highlighting/archive/master.zip) option and unzip them.

#### Activating theme

1. Before being able to use the Dracula theme for zsh-syntax-highlighting, you must first have [downloaded and installed the zsh-syntax-highlighting](https://github.com/zsh-users/zsh-syntax-highlighting/blob/master/INSTALL.md) utility (and be using [zsh](https://github.com/ohmyzsh/ohmyzsh/wiki/Installing-ZSH)).

2. Copy the contents of the [Dracula zsh-syntax-highlighting](https://github.com/dracula/zsh-syntax-highlighting.sh) file, and paste into your zshrc file, likely at `~/.zshrc`.

   * **Note**: Be sure to paste the contents _before_ the `source /usr/local/share/zsh-syntax-highlighting/zsh-syntax-highlighting.zsh` in your `~/.zshrc` file.

3. Start a new zsh session: `exec zsh` and confirm it's working.
