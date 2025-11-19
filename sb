import discord
import os
from dotenv import load_dotenv

load_dotenv()
TOKEN = os.getenv("TOKEN")

if not TOKEN:
    print("[-] No token → create .env and put TOKEN=your_token")
    exit()

client = discord.Client(self_bot=True)

@client.event
async def on_ready():
    print(f"[soft blade streaming] {client.user}")
    await client.change_presence(
        activity=discord.Streaming(
            name="soft blade",                     # text that shows
            url="https://twitch.tv/softblade"      # any valid twitch/youtube link works
        )
    )
    print("→ Streaming soft blade")

client.run(TOKEN, bot=False)
