Roshutsu Playing Game Translation Project
=========================================

How to use
----------

Download the repository using the green "Clone or download" button in the topright (or clone it if you're familiar with git).

Download the latest version of [RPGMaker Trans](http://rpgmakertrans.bitbucket.org/) and launch it

In the "Game Location" field, select the original, untranslated `game.exe`

In the "Patch Location" field, select the corresponding `RPGMKTRANSPATCH` from this repository

Hit the `Go` button

RPGMaker Trans will create a translated copy of the game in the selected "Translation Location" directory

How to contribute
-----------------

If you're familiar with git, just use the commandline

### Setting up
  * [Download and install](https://desktop.github.com/) Github for desktop
  * [Fork the repository](https://help.github.com/articles/fork-a-repo/) to your github profile
  * [Clone your fork](https://help.github.com/desktop/guides/contributing/cloning-a-repository-from-github-to-github-desktop/) to a directory on your computer

### Making changes
untranslated strings will look like this: 
```
> BEGIN STRING
\\name[\\n[1]]えぇっと・・・
> CONTEXT: Map023/events/8/pages/0/44/Dialogue < UNTRANSLATED

> END STRING
```
simply write the translation of the japanese string under the `>CONTEXT` line while keeping the actual game code the same, like so:
```
> BEGIN STRING
\\name[\\n[1]]えぇっと・・・
> CONTEXT: Map023/events/8/pages/0/44/Dialogue < UNTRANSLATED
\\name[\\n[1]]uhm...
> END STRING
```

### Testing your changes
  * simply follow the steps from 'How to use'
  * You'll notice that after patching, the `< UNTRANSLATED` identifiers of the strings that you translated have now dissappeared

### Get your contributions live
  * [Commit your changes](https://help.github.com/desktop/guides/contributing/committing-and-reviewing-changes-to-your-project/)
  * Sync your commits with the github repository by pressing the 'Sync' button in the topright
  * [Submit a pull request](https://help.github.com/articles/creating-a-pull-request/) to the masterbranch of the original repository