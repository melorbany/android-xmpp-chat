# android-xmpp-chat 
Cloned From Conversations

Conversations: the very last word in instant messaging


## Design principles

* Be as beautiful and easy to use as possible without sacrificing security or
  privacy
* Rely on existing, well established protocols (XMPP)
* Do not require a Google Account or specifically Google Cloud Messaging (GCM)
* Require as few permissions as possible

## Features

* End-to-end encryption with either [OTR](https://otr.cypherpunks.ca/) or [OpenPGP](http://www.openpgp.org/about_openpgp/)
* Send and receive images as well as other kind of files
* Share your location via an external [plug-in](https://play.google.com/store/apps/details?id=eu.siacs.conversations.sharelocation)
* Indication when your contact has read your message
* Intuitive UI that follows Android Design guidelines
* Pictures / Avatars for your Contacts
* Syncs with desktop client
* Conferences (with support for bookmarks)
* Address book integration
* Multiple accounts / unified inbox
* Very low impact on battery life


### XMPP Features

Conversations works with every XMPP server out there. However XMPP is an
extensible protocol. These extensions are standardized as well in so called
XEP's. Conversations supports a couple of these to make the overall user
experience better. There is a chance that your current XMPP server does not
support these extensions; therefore to get the most out of Conversations you
should consider either switching to an XMPP server that does or — even better —
run your own XMPP server for you and your friends. These XEP's are:

* XEP-0065: SOCKS5 Bytestreams (or mod_proxy65). Will be used to transfer
  files if both parties are behind a firewall (NAT).
* XEP-0163: Personal Eventing Protocol for avatars
* XEP-0198: Stream Management allows XMPP to survive small network outages and
  changes of the underlying TCP connection.
* XEP-0280: Message Carbons which automatically syncs the messages you send to
  your desktop client and thus allows you to switch seamlessly from your mobile
  client to your desktop client and back within one conversation.
* XEP-0237: Roster Versioning mainly to save bandwidth on poor mobile connections
* XEP-0313: Message Archive Management synchronize message history with the
  server. Catch up with messages that were sent while Conversations was
  offline.
* XEP-0352: Client State Indication lets the server know whether or not
  Conversations is in the background. Allows the server to save bandwidth by
  withholding unimportant packages.
* XEP-0191: Blocking command lets you blacklist spammers or block contacts
  without removing them from your roster.
