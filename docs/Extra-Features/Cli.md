---
sidebar_position: 2
---

# Cli

If you were observative enough, you might have seen that **ChitChatJS** has a CLI! Almost all of the commands don't have to be used. But one you might know about is:
```
chitchatsjs build myFile.chit.js
```
This will build your file to ChitChatJS! And then you can run it! No need for requiring it! Horary!

But there is other commands, and this slide will tell you about them!

## Commands
These are the commands to the ChitChatjs CLI.
### Build
There is the `build` commands as we mentioned earlier:
```
chitchatsjs build myFile.chit.js
```
There is etiquette for this. Every file should have `.chit` in it to let you know it's a test file. DO NOT make a `.chit` file have no tests, or anything that isn't related to a test. While you can do that, you shouldn't because it can ruin the way the output of your file works. But while a `.chit` file isn't required, it is proper etiquette to do so.
### Example

If you don't want to make the ChitChatjs environment yourself, don't worry! You can use a quickstart command to get you ChitChatjs environment up and running _fast_. The command is:
```
chitchatsjs example myFolderName
```
If you put in a folder name at the end of the command, ChitChat will change the clone folder name to my what you put there. If no folder name is specified, the name for the folder will stay the default name.

-----
Those are all of the CLI commands currently in ChitChatjs, there will be more soon!