Auto Invite Macro

Alias

```
/alias ll /invite <----- Write this into your chat bar and run once to create the entry in the alias.txt file
```

invite2

```
/ui action startChatReply;
/ui action chatCursorHome;
/ui action chatCursorRight;
/ui action chatDelete;
/ui action chatDelete;
/ui action chatEnter;
/tell [your name] Auto Invite is running....; <---- replace with your characters first name, delete the brackets
/pause 8;
/macro invite2;
```

Now all anyone has to do is send you a tell and you will auto target them and send them a group invite. You must be the group leader in order to do this.
The /tell in the 3rd to last line sends yourself a message so you don't end up spamming the last person you sent an invite to.

References

* [Auto Invite Macro](https://swgprophecy.com/showthread.php?tid=727)
