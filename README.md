<img src="./images/icon.png?raw=true" width="75" align="left">

# [Discord Text to Speech Bot](https://discordapp.com/oauth2/authorize?client_id=801286916082237441&scope=bot%20applications.commands&permissions=3196928)

Text to speech Discord bot using [FakeYou](https://fakeyou.com).

Massive thanks to [@echelon](https://github.com/echelon) for supporting this project!

## Commands

### Join

Joins your voice channel.

`/join`

### Leave

Leaves your voice channel.

`/leave`

### Say

Generates speech using FakeYou, sent as an attachment.

`/tts <voice> <message>`

- `<voice>`: Voice model to speak with. Use `/voices` to list [all options](./docs/voices.md). Use keyword "random" to get a random voice.
- `<message>`: Message to speak.

### Say (voice chat)

Generates speech using FakeYou, spoken through voice chat.

`/ttsvc <voice> <message>`

- `<voice>`: Voice model to speak with. Use `/voices` to list [all options](./docs/voices.md). Use keyword "random" to get a random voice.
- `<message>`: Message to speak.

### Voices

Lists [all available voices](./docs/voices.md).

`/voices`

## Setup

1. [Create your app with a Bot](https://discordapp.com/developers/applications/me).
2. Copy your bot's secret token and paste it into [config.json](./config.json).
3. If you have a [FakeYou API token](https://docs.fakeyou.com/#/), paste it into [config.json](./config.json).
4. Go to `https://discordapp.com/oauth2/authorize?client_id=<CLIENT_ID>&scope=bot%20applications.commands&permissions=3196928`, with `<CLIENT_ID>` as your app's client ID.
5. [Install Node.js](https://nodejs.org/en/download): `brew install node`
6. [Install FFmpeg](https://www.ffmpeg.org/download.html): `brew install ffmpeg`
7. [Install the dependencies](./package.json): `npm install`
8. [Run the bot](./ttsbot.js): `npm start`
