
We can set up a wiki using [Obsidian](https://obsidian.md) as the markdown text editor and the [Obsidian Git](https://github.com/denolehov/obsidian-git/wiki/Installation) plugin.


# Plugin setup:

Once you download Obsidian from the link above, open it and create a new folder, called a "vault".

To do this go to the "open another vault" icon in the bottom left. go to "create a new Vault" then navigate to the directory on your laptop that you want to save this wiki locally. Create a new folder for it, you can call it anything you want.

Then go to the settings menu in the wheel icon in the bottom left and, go to "community plugins" and click "allow community plugins".

Click on "community Plugins", click "browse" and search for "Obsidian Git" by Denis Olehov.

# Plugin Features:

Downloading this plugin gives your Obsidian vault a bunch of new commands that you can access from the command menu in the top left menu. 

On the left top menu it's the icon that looks like >_ or can access it faster though typing "cmd" + "P" / "ctrl" + "P"

Bring it up and type "git" in the search bar to see all the commands associated with this plugin.

Note: because we are managing the repo through Obsidian, we can access the gitignore file through this command palette too through the "edit gitignore command". You can also do this from the directory on your machine but that is more likely to break things.

# Token Generating

Generate your own token from the settings of your Github account [HERE](https://github.com/settings/tokens). You only need to do this once. 

Once its generated save it somewhere you can easily copy/paste from when cloning the repo in the next step.

# Cloning this repo:

##### Create a folder in your Vault:

Create a folder where you want to clone the wiki. This will be the place where you add and make all your changes. You can call it [name]Wiki to match the Repo and make life easy (it's fine if you've already named the Vault folder the same thing)

##### Clone Remote Repo

Now that the Obsidian Git plugin is enabled, open up the Command Palette by typing "cmd"+"P". Type "git" to see all the git commands and find the "Clone Remote Repo" commad.

In the bar that comes up, paste the link of the repo in this format:

```
https://ghp_XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX@github.com/foldername/[name]Wiki.git
```

Replace the "ghp_XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX" with your token generated earlier. 

You will be asked for the directory where you want to save the repo, put in the name of folder you made earlier.

Leave the next bar empty.

Ta-Da! you should have this repo now inside your Obsidian Vault.

Note: any notes you create outside the repo folder will remain local to your machine, only the contents of this folder are part of the Git stream. This is handy for making your own notes on the side before integrating them into the wiki.

# Committing and Pushing:

Keep in mind that you need to keep the git workflow in mind, so after you've create any new page, go back into the command palette and do "Git Commit all changes", and then bring it up again and do "Git Push". 

