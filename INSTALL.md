### [zsh-syntax-highlighting](https://github.com/zsh-users/zsh-syntax-highlighting)

#### Install using Git

If you are a git user, you can install the theme and keep up to date by cloning the repo:

    git clone https://github.com/dracula/zsh-syntax-highlighting.git

#### Install manually

Download using the [GitHub .zip download](https://github.com/dracula/zsh-syntax-highlighting/archive/master.zip) option and unzip them.

#### Activating theme

1. Before being able to use the Dracula theme for zsh-syntax-highlighting, you must first have [downloaded and installed the zsh-syntax-highlighting](https://github.com/zsh-users/zsh-syntax-highlighting/blob/master/INSTALL.md) utility (and be using [zsh](https://github.com/ohmyzsh/ohmyzsh/wiki/Installing-ZSH)).

2. Copy the contents of the [Dracula zsh-syntax-highlighting](https://github.com/dracula/zsh-syntax-highlighting/blob/master/zsh-syntax-highlighting.sh) file, and paste into your zshrc file, likely at `~/.zshrc`.

   * **Note**: If you installed zsh-syntax-highlighting [via git](https://github.com/zsh-users/zsh-syntax-highlighting/blob/master/INSTALL.md#in-your-zshrc), or [site wide](https://github.com/zsh-users/zsh-syntax-highlighting/blob/master/INSTALL.md#system-wide-installation), be sure to paste the contents of the file _before_ the following line in your `~/.zshrc` file:

      ```bash
      # ...
      source /some/path/to/your/zsh-syntax-highlighting/zsh-syntax-highlighting.zsh
      # ...
      ```

   * **Note**: If you installed zsh-syntax-highlighting [via a plugin manager](https://github.com/zsh-users/zsh-syntax-highlighting/blob/master/INSTALL.md#with-a-plugin-manager), be sure to paste the contents of the file _before_ you activate the utility via it's plugin invocation.

3. Start a new zsh session: `exec zsh` and confirm it's working.

#### Implementation

This theme attempts to cover all possible zsh-syntax-highlighting options for the [**main** highlighter](https://github.com/zsh-users/zsh-syntax-highlighting/blob/master/docs/highlighters/main.md). The coloring was implemented/modelled after the [official Dracula color specification](https://spec.draculatheme.com/) as much as logically possible.

As such, the theme is grouped by Dracula spec section; Each section in the spec is 1:1 with a `## <header>` in the theme file. For settings that didn't seem to fall under any of the Dracula spec, they are under the `## No category relevant in spec` section.

Within a section, the options occur in the same order they do on the [main highlighter doc page](https://github.com/zsh-users/zsh-syntax-highlighting/blob/master/docs/highlighters/main.md).

#### Accompanying Screnshot Prompt

Though not related to this theme nor included as a specific Dracula offering, the prompt in the screenshot is [typewritten: "A minimal zsh prompt"](https://typewritten.dev/#/). Relevant `~/.zshrc` settings are so:

```bash
# Typwritten: https://typewritten.dev/#/installation; Dracula compliment, purple based
ZSH_THEME="typewritten"

export TYPEWRITTEN_SYMBOL="λ "
export DRACULA_TYPEWRITTEN_COLOR_MAPPINGS="primary:#d5ccff;secondary:#9580ff;info_neutral_1:#d0ffcc;info_neutral_2:#ffffcc;info_special:#ff9580;info_negative:#ff5555;notice:#ffff80;accent:#d5ccff"
export TYPEWRITTEN_COLOR_MAPPINGS="${DRACULA_TYPEWRITTEN_COLOR_MAPPINGS}"
export TYPEWRITTEN_PROMPT_LAYOUT="half_pure"
```
