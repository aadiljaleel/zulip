{!create-a-bot.md!}

Construct the URL for the {{ integration_display_name }}
bot using the bot's API key and the desired stream name:

{!webhook-url.md!}

Modify the parameters of the URL above, where `api_key` is the API key
of your Zulip bot, and `stream` is the [URL-encoded](https://www.urlencoder.org/)
stream name you want the notifications sent to. If you do not specify a
`stream`, the bot will send notifications via PMs to the creator of the bot.

If you'd like this integration to always send to a specific topic,
just include the (URL-encoded) topic as an additional parameter
(E.g. for `your topic`, append `&topic=your%20topic` to the URL).

{% if all_event_types is defined %}

{!event-filtering-instruction.md!}

{% endif %}
