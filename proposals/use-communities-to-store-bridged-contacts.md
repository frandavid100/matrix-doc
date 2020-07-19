# Use communities to store bridged contacts

When a Matrix user wants to start a conversation with a bridged contact (i.e. a contact on other platforms like Telegram or Whatsapp), the easiest way is to use that platform’s native client because it usually has a contact list.

Doing it from a Matrix client is much more unintuitive and requires jumping through a series of hoops; the user needs to open a DM with the bridge bot and then use written commands to find that contact and start a conversation.

This makes users less likely to use a Matrix client as a replacement for their native Telegram or Whatsapp clients, and therefore, it makes them less likely to start regular Matrix use. Letting the Matrix client show a list of bridged contacts would solve this problem.

# Proposal

## Creating and storing the contacts

Most bridges can already access a list of contacts on the bridged platforms. For example mautrix-telegram can see the user’s Telegram contacts.

According to this proposal, the bridge would create a puppet for each of those bridged contacts and would then add all those puppets to a community. This would allow the user to see a complete list of all her Telegram contacts and easily start a conversation with any of them, from any of her Matrix clients.

## Showing the contacts

Some Matrix clients (e.g. element-android) can access the contacts on your phone and show them on a list, even filtering those who already have a Matrix account.

They should also list all the members of all the communities that you’re a part of. That way, every bridged contact would appear on that list and it would be easy to visually find them, and start a conversation with any of them.

## Potential issues

None that I can think of.
