# LeagueChatEx
An external League Of Legends Chat Client.
It is small, portable and open-source.

## Requirements
LeagueChatEx requires Windows XP or newer and the .NET Framework 4.

## Terms Of Use
I'm developing this application to the best of my knowledge, but errors can happen. Any data entered into the software (including username and password) is used to access the Riot Games Chat Service only. You have access to the full source code of the application for review. Download a pre-compiled version only from trusted sources or compile it yourself. Be responsible with your data.

THE SOFTWARE IS PROVIDED ‘AS IS’, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

## How To Update Champion Images
_You don't have to wait for me to update the application!_

If a new champ is release, simply copy it's thumbnail image to the `Resources\Champions\` folder. It is named
`champName_Square_0.png` and can be found in your league of legends folder at `RADS\projects\lol_air_client\releases\0.0.0.xxx\deploy\assets\images\champions`.

## How does it work?
Accessing the League of Legends Chat Service is pretty straight forward since it's using a mostly unmodified XMPP ("Jabber") protocol,
so basically you can connect to it with most multi-protocol chat applications like [Digsby][12], [Pidgin][13], [Miranda][14], etc. Details on how to do this can be found at [leaguecraft.com forums][11].

Chat room names are hashed. You need generate the desired room name like this: `"pu~" + SHA1(lowerCase(roomName))` (e.g. `pu~e400cbec9d6e7b79a35f967fdf6fa8c4f9cf0247` is the hashed name for "[The Gentlemen's Club][15]").

## Development
LeagueChatEx is a fork of [LeagueChat][1] by Iosif "vrokolos" Karaioannoglou. Thanks!

LeagueChatEx is developed in C# using [Visual Studio Express 2012 for Windows Desktop][8].
If you wish to contribute to the project you can help by submitting issues or even code to the [GitHub Repository][2].

## License
LeagueChatEx is licensed under the [Mozilla Public License (MPL)][5] [Version 2.0][6]. A copy of this license is shipped with the source code as `LICENSE.txt` and can be obtained online at [http://www.mozilla.org/MPL/2.0/][6]. The source code can be obtained from the project home.

## Contact
LeagueChatEx is developed by Manuel Kroeber. Free free to send me a message to [manuel.kroeber@gmail.com][4] if you have any questions or concerns.

Project home can be found at [https://github.com/ElectronicWar/LeagueChat][2].

## Copyright Acknowledgement
LeagueChatEx uses artwork assests ("Champion Images") from [League Of Legends™][9] by [Riot Games][10] for easy access and recognition under fair use. If you are a copyright holder and don't agree with your assets being used within this software, please contact me and I will remove everything in a timely manner.

## Thanks
LeagueChatEx is developed with the help of the [Git SCM][4] via [GitHub For Windows][5]. The online home is hosted by GitHub at [github.com][6]. Plain text magic happens in [Sublime Text 2][7].


[1]: https://github.com/vrokolos/LeagueChat
[2]: https://github.com/ElectronicWar/LeagueChat
[3]: mailto:manuel.kroeber@gmail.com
[4]: http://git-scm.com/
[5]: http://windows.github.com/
[6]: http://www.github.com/
[7]: http://www.sublimetext.com/
[8]: http://www.microsoft.com/visualstudio/eng/products/visual-studio-express-for-windows-desktop
[9]: http://www.leagueoflegends.com/
[10]: http://www.riotgames.com/
[11]: http://forum.leaguecraft.com/index.php?/topic/35070-guide-accessing-your-friendlist-outside-the-game/
[12]: http://www.digsby.com/
[13]: http://www.pidgin.im/
[14]: http://www.miranda-im.org/
[15]: http://thegentsclub.org/