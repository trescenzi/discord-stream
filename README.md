# Discord Streams

A library that wraps many of the [Discord.js](https://github.com/hydrabolt/discord.js/)
api calls in Kefir streams for those that prefer streams to callbacks.

```js
const Discord = require(discord-stream);

const client = new Discord.client();

client.login(<api token>);
client.ready.log('Server ready');

client.message.map((msg) => msg.content).log('msg:');
```
