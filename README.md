<center>
  <h2>Ever Changing</h2>
  <a href="https://modrinth.com/mod/fabric-api"><img src="https://wsrv.nl/?url=https://cdn.modrinth.com/data/cached_images/8bd6d7ff822dc33ffb55af6cc0c7062cec53e9e3.png&amp;n=-1" alt="Requires Fabric API" width="200"></a>
</center>

Ever Changing lets you paste the URL of a GitHub gist (compatible with the [Engrok mod](https://modrinth.com/mod/engrok)) instead of a regular server IP in the multiplayer screen, and it pulls the ip from that gist every time you start an Ngrok tunnel, which conveniently can be automatically updated using the Engrok mod!
The Ever Changing mod is a client mod, as it is needed on the client to prevent the server IP from changing on the client, not on the server.

## Simplest explanation
When you start the server, the Engrok mod automatically opens an Ngrok tunnel. By what you said, you're aware of that, and you're also aware of the fact that the IP changes every time you open the tunnel. For that reason, I specifically added a GitHub Gist integration (essentially these are text files) which you can add to automatically update the tunnel IP on the gist file (which is online and accessible to people with its ID) whenever the tunnel opens.

## How does the Ever Changing mod connect?
Well, when you the mod's IP address format instead of the regular IP format, it automatically connects to the GitHub servers, hassle free from the client's side - no need for verifications, no nothing - and fetches the data and connection address from that gist. So every time you hit refresh in the the multiplayer screen, the ip is fetched again from the gist. The same thing also happens when you try to join.

# Usage
To use ever changing, you don't need to use any settings whatsoever! All you have to do is add a server on the multiplayer screen in Minecraft, and instead of a regular IP address, you type in one of three things (the example gist's id is this: `3bef909cddbfbb117f0bcf101222a5dc`):
1. The GitHub gist's main URL, which looks like this if you're on the gist's page: 
`gist://https://gist.github.com/MagicQuartz/3bef909cddbfbb117f0bcf101222a5dc`<br>
(Format: `"gist://" + "https://gist.github.com/gitHubUser/" + gistId`)
2. The GitHub gist's api URL, which looks like this:
`gist://https://api.github.com/gists/3bef909cddbfbb117f0bcf101222a5dc` <br>
(Format: `"gist://" + "https://api.github.com/gists/" + gistId`)
3. Just type it using the raw prefix like this:
`gist://raw:3bef909cddbfbb117f0bcf101222a5dc` (This is how the IP address in Minecraft is supposed to look with the Ever Changing mod) <br>
(Format: `"gist://raw:" + gistId`)
<br><br>

Any of these can be provided by the server's owner for seamless connection. have fun!


Please keep in mind this mod was made in about 5 hours so it may not work perfectly, but I did my best to patch everything, so please do not try to intentionally break things.
