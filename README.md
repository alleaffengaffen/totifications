# Totifications

An instance of [urlwatch](https://urlwatch.readthedocs.io) that regurarly fetches news for me.

## Telegram Setup

- Create a new bot
- Add description and other things if you like
- Search the bot in the users and start your chat with it, also write some nonsense text to it
- Run the following command to get the ID of your private chat with the bot: `TOKEN="" curl https://api.telegram.org/bot$TOKEN/getUpdates | jq`
- Add the ID and the token to the vault

## Test new URLs

You can locally run the following command to see if urlwatch produces the correct output:

```console
urlwatch --config=rendered-urlwatch.yaml --urls=urls.yaml --test-filter 16
```

Note: the `rendered-urlwatch.yaml` file must be generated the same way as the actions does it.