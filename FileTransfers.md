# File transfers with GTalkSMS #

XMPP provides a handy file transfer feature. It is possible to send a file to the XMPP account GTalkSMS uses. The file will get stored at /mnt/sdcard/GTalkSMS.
The other way works to: Receiving files from you Android phone via the `send:/path/to/file` command. You can discover your Android's filestystem with the `ls` command. Just send `ls` to list the contents of the default dir ( /mnt/sdcard/GTalkSMS ) or try `ls:/path/to/dir`.

The XMPP file transfer process is sophisticated and therefore complex. **We can not guarantee that it will work in your case**. However it has been tested with a setup of Openfire as Server, and Gajim as Client. Make sure to set your XMPP file transfer proxy to a valid XMPP component, Gajim does this automatically for you. Other server/client combinations should also work. **For an successful file transfer, we suggest you to create an extra account for GTalkSMS preferably on an pure XMPP service (not GTalk!)**

If you have suggestions or discovered a bug regarding this feature. Please don't fill an issue. Instead, report directly to the [gtalksms-users mailing list](http://groups.google.com/group/gtalksms-users). A complete trace of the XMPP stanzas involved with the file transfer will help to debug the problem. Most clients provide an XML console for the XMPP connection. Also an [AppLog](GenerateAppLog.md) will be helpful.