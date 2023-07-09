+++
title = "Rust-based CLI tools you might like"
date = "2023-07-09"
author = "MacBobby Chibuzor"
description = "Blog post about Rust-based CLI tools you should be using."

[taxonomies]
tags = ["showcase", "tools", "Rust"]
+++

# Hi there 👋

This post is about some random tools built with Rust that I found while surfing around social media and thought you might like—just as I did.

Without wasting too much of your time, let’s explore! 🏄‍♂️

# Starship.rs

The first is [Starship](https://starship.rs)—a command line tool. Check the descriptions in the image below to know what Starship does:

![Starship.rs](/imgs/starshiprs.png)

### Quick intro to shell customizations and installation of `starship`

You might at least be familiar with `bash` and `zsh` terminals by now. You probably already use either. To install `starship`, run:

```bash
brew install starship
```

Then proceed to add this to either you `~/.zshrc` or `~/.bashrc` file or both:

```bash
eval "$(starship init zsh)" # for zsh
eval "$(starship init bash)" # for bash
```

The tilde (~) sign refers to your home directory where these files are located and hidden. If you don’t already have it, run this command to create it:

```bash
touch ~/.zshrc # creates the .zshrc file in home dir
```

Once it’s installed, run this command to open it:

```bash
open ~/.zshrc
```

Or press **Cmd** + **Shift** + **.** on your macOS.

![Install Starship on MacOS](/imgs/install-starship.png)

You can [select existing themes](https://starship.rs/presets/) or [configure your own](https://starship.rs/config/) if you know how to use Rust’s `Cargo.toml` file syntax.

Note that you can customize `starship` for you particular language and terminal; check the configuration page on how to go about it.

![Starship Terminal](/imgs/starship-terminal.png)

<aside>
🎯 If you don’t use macOS, you can find the installation guide for Starship [here](https://starship.rs/guide/).

</aside>

# Lazygit

Lazygit helps you manage your git version control processes. You can download the updated tool from here:

https://github.com/jesseduffield/lazygit

## Quick usage

After installation, you just have to run the command below to start using lazygit:

```bash
lazygit
```

Just that, and a screen appears on your terminal:

![Lazygit](/imgs/lazygit.png)

# Bat

Bat is the modern replacement for your UNIX `cat` command. You can learn about the advanced features it offers from the GitHub page here: https://github.com/sharkdp/bat.

To install `bat` on macOS, run:

```bash
brew install bat
```

## Quick usage of `bat`

You can view an entire file content with `bat` by running:

```bash
bat filename.extension
```

For example, I ran the command to view a Go source file below:

```bash
bat arraySolutions.go
```

[See video](https://file.notion.so/f/s/cbfc8212-5a3c-42eb-bff5-f9498b87938f/Untitled.mp4?id=36ae920d-cce0-4c70-b05c-c5553ad7fa87&table=block&spaceId=77a131a6-6347-4e0d-b098-1474be9ec9b8&expirationTimestamp=1688954400000&signature=_hDTlEYWemyiZbu12Ebzu9-vxct2KA_xs8NduRtEQkM&downloadName=Untitled.mp4)

Video compressed from 8.8mb to 1.9mb with veed.io

Use `q` to quit the session. You can also learn more on how to use `bat` here: https://github.com/sharkdp/bat.

# zoxide

`zoxide` is a smart CLI command that replaces `cd`. With it, you can quickly jump from one directory to the other without writing a bunch of confusing `cd ../../enter_here/exit_there`.

Install `zoxide` on macOS by running:

```bash
brew install zoxide
```

Learn about how to use zoxide from the official GitHub page here: https://github.com/ajeetdsouza/zoxide. You will also find instructions for installing on other operating systems.

After installation, you have to add `zoxide` support for your shell before attempting to use it. Add this line to your `/.zshrc` file if you use Oh My Zsh shell:

```bash
eval "$(zoxide init zsh)" 
```

Remember to Save changes with **Cmd** + **S**.

## Quick Usage of `zoxide`

In principle, `zoxide` says, “once you did it once before, you don’t have to do it again.” It’s like a taxi driver that remembers where you always go, so you don’t have to tell him. To demonstrate, let’s go into a project directory from my home directory, then come back to home, and then try to jump directly to the project directory without writing the exact absolute path:

![Zoxide Demo](/imgs/zoxide-demo.png)

- From /Users/macbobbychibuzor, I wrote a very long path to a Geth project repository
- Next, I displayed the repository I’m now in
- Next, I navigated back to my personal home
- Afterwards, I tried accessing the project repository, and boom! I’m in.

# LSD

[LSD](https://github.com/lsd-rs/lsd) is the replacement for `ls`, which is originally the UNIX command to list the contents of a directory.

Recap:

- `ls`: lists contents of a directory
- `ll`: lists contents of a directory and their file permissions
- lsd: lists all of the above, including more details

![LSD Demo](/imgs/lsd.png)

To install, run:

```bash
brew install lsd
```

You can replace `ls` with `lsd` or make a sub-command like `ls --d` to run `lsd` by adding an alias to the `/.zshrc` file:

```bash
alias 'ls --d'=lsd
```

Or you can decide to have a new command:

```bash
alias list=lsd # or temporarily run it on the terminal instead of saving.
```

# exa

[exa](https://www.youtube.com/redirect?event=video_description&redir_token=QUFFLUhqbWtUWnVsZ1lKSUFXaW52QVhocjRETXpnSGlBZ3xBQ3Jtc0tuUDFHSGxYeWUzQWxpM19XWjhtTFNvbDZPSUFGejNnWmJ0dFZrdXFKcGpnZzk1Y2lEMi1LZXBCZ3ozR1c5RGxqN09sa3M2N1hoTHJVOVNnNGU4SWVOeVJMR01DUXEzajAyY3RLRXJXMXZVX2NxOS1UUQ&q=https%3A%2F%2Fthe.exa.website%2F&v=stCXFxC4OH0) is another alternative for `lsd`. To install, run:

```bash
brew install exa
# since installation is long, add the say command
brew install exa ; say "I just completed the exa download, boss. Come back."
```

## Usage

You have to [learn](https://the.exa.website/docs) about the `--options` and `--flags` you can add to exa execution to use it. Here’s an example using `—-long` `—-header`:

![Exa Demo](/imgs/exa.png)

# Conclusion

This list is going to be updated as I find new tools built with Rust.