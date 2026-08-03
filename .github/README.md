<div align="center">

<h2>Apple Music Bot</h2>

<b>Telegram Group Calls Streaming Bot</b><br>
Supports YouTube, Spotify, Apple Music, SoundCloud & M3U8 links.

<br>

<img src="https://files.catbox.moe/61oqva.jpg" width="720" height="auto">

</div>

<hr>

<h2>✨ Features</h2>
- 🎧 Stream low-latency audio & video in Telegram group video chats.
- 🌐 Supports YouTube, Spotify, Apple Music, and SoundCloud.
- ⚡ Advanced queue management & auto-play.
- 🚀 Easy deployment on Heroku or VPS.

<hr>

<h2>☁️ Deployment</h2>

<h3>Deploy to Heroku</h3>
<p>Click the button below to deploy this bot directly to Heroku:</p>
<a href="https://dashboard.heroku.com/new?template=https://github.com/AMMUKASH/Apple-music">
    <img src="https://img.shields.io/badge/Deploy%20On%20Heroku-black?style=for-the-badge&logo=heroku" alt="Deploy To Heroku"/>
</a>

<h3>Local / VPS Setup</h3>
<bash>
git clone https://github.com/AMMUKASH/Apple-music && cd Apple-music
curl -Ls https://astral.sh/uv/install.sh | sh
export PATH="$HOME/.local/bin:$PATH"
uv sync --frozen
mv sample.env .env
# Edit .env with your credentials
bash start
</bash>

<hr>

<h2>⚙️ Configuration</h2>
Configure the following required variables in your <code>.env</code> file or Heroku config vars:
<ul>
  <li><code>API_ID</code> — Get from my.telegram.org</li>
  <li><code>API_HASH</code> — Get from my.telegram.org</li>
  <li><code>BOT_TOKEN</code> — Get from @BotFather</li>
  <li><code>OWNER_ID</code> — Your Telegram user ID</li>
  <li><code>MONGO_URL</code> — MongoDB connection string</li>
  <li><code>SESSION</code> — Pyrogram string session</li>
</ul>

<hr>

<h2>🧐 Basic Commands</h2>
<pre>
/play [song name/link] - Play audio in video chat
/vplay [song name/link] - Play video in video chat
/pause - Pause current stream
/resume - Resume playback
/skip - Skip to next track
/stop - Stop playback
/queue - Show active queue
</pre>
