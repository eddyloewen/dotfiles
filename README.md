# Eddy's dotfiles
This repository contains all my dotfiles to set up and configure my Mac.
It serves as a backup mechanism for such files and helps to get started with a new Mac.

## Setting up my Mac

After backing up your old Mac you may now follow these install instructions to setup a new one.

1. Update macOS to the latest version through system preferences
2. [Generate a new public and private SSH key](https://docs.github.com/en/github/authenticating-to-github/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent) by running:

	 ```zsh
	 curl https://raw.githubusercontent.com/eddyloewen/dotfiles/HEAD/ssh.sh | sh -s "<your-email-address>"
	 ```

3. Clone this repo to `~/.dotfiles` with:

	  ```zsh
		git clone --recursive git@github.com:eddyloewen/dotfiles.git ~/.dotfiles
		```

4. Run the installation with:

	  ```zsh
		cd ~/.dotfiles && ./setup.sh
		```

5. After mackup is synced with your cloud storage, restore preferences by running `mackup restore`
6. Restart your computer to finalize the process

Your Mac is now ready to use!

> 💡 You can use a different location than `~/.dotfiles` if you want. Make sure you also update the reference in the [`.zshrc`](./.zshrc#L2) file.
