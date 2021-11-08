# dahabtest
Python 3.6+
High speed Internet Connection
Good proxy list (http, https, socks4, socks5)
Google Chrome installed on your OS (not Chromium)
Features
YouTube default, live streaming and YouTube Music support
Multithreaded and Dynamic thread support
Auto download updated chrome driver whenever user's Google Chrome version is updated
Patch chrome driver on the start of every thread by undetected-chromedriver
Proxy support
location : text file (must be on path) / proxy API (should work with most of the proxy providers)
type : http, https, socks4, socks5
format : ip:port, user:pass@ip:port, ip:port:user:pass
proxy refresh after a certain time specified by the user
rotating proxy support
chrome v70+ randomized user agent based on platform
canvas,audio,font,webgl fingerprint defender and IP leak prevent by webrtc control
geolocation, timezone, referer spoofing
can add extra extensions in the extension/custom_extension/ folder
direct link or search keyword on YouTube then watch the video by matching exact video title
modify urls.txt and search.txt on the fly without restarting program
HTTP api on localhost and a database to store view count
config.json to save settings
bypass consent page and several other pop up
save bandwidth by reducing video quality
can set higher(100%) watch duration percentage to increase Watch time, change playback speed
Proxies
IPRoyal offers datacenter and residential proxies. The Royal Residential proxies have a large pool with addresses in over 160 countries all over the world, so they can generate a massive number of views. IPRoyal agreed to provide a huge discount for my script users, so the price will be as low as 0.60USD/GB! To get this incredible 80% discount for Royal Residential proxies, use the discount code: youtubers80

Free Proxy
Try not to use free proxies. But if you have a paid subscription and you want to use authenticated IP feature, then you can use the free proxy category. Provide your text file path (where you saved the proxies) when the script asks for a proxy file name or a proxy API. N.B: Available for http(s)/socks4/socks5

Premium Proxy
Proxies with authentication can also be done. To do so put your proxies in this format username:password@ipaddress:portor ipaddress:port:username:password in a text file. Every single line will contain a single proxy. Provide your text file path when the script asks for a proxy file name or a proxy API.

N.B: Only available for http type proxy.

Rotating Proxy
You can also use the rotating proxies service. You can either authenticate your IP on your proxy provider service and use ipaddress:port as Main Gateway. N.B: Available for http(s)/socks4/socks5

Or direct use username:password combo like this username:password@ipaddress:port or ipaddress:port:username:password as Main Gateway.

N.B: Only available for http type proxy. You can use proxy API too.

HTTP API
Live logs fetched every 10 seconds and statistics in graphs are available on http://localhost:5000/ .Or http://ip_of_your_pc:5000/ use this to access from another device under same network. A SQLite Database is being used to store your generated views from this script. Last 20 logs from scripts are fetched every 10 seconds to show on website and graph is updated every 5 minutes.

Config.json
No need to type everything everytime you run the script. A config file will be created automatically to save and use your preferences.

Urls
Put video links in the urls.txt. For multiple videos place urls in multple lines.

To find video link in YouTube click share and copy.
If you have any external link which will redirect to your youtube video you can use that too. Example : when you post a YouTube video link in twitter and you hit play on twitter, you will get a link like this https://t.co/xxxxxxxxxx?amp=1. This is helpful because YouTube will see that views are coming from External Source like twitter in this example.
Search
Program can search youtube with the keyword you want and find video with video title. To do this you need to know what keyword can find your video on youtube search engine. Also you need to provide exact video title. Put keyword and title like this format keyword :::: video title in search.txt. You can use same video title for multiple keyword too.

If you don't know any keyword just put your video title :::: video title in search.txt

Live Stream
This script supports live streams too. Just use this script as you would for the already uploaded video. Script will automatically know if your video is live. Just bear in mind, you need a high-end pc for higher threads to get more viewers. Basically, script will check every 60 secs if youtube shows x watching now is present. If your live stream ends, script will check 5 times to be sure. In another word, after your live stream ends, script takes 5 minutes to close the driver.

If you have never used this script before, use this first for an already uploaded video. This way, you will have a better understanding of how this script works. To do so, keep reading.

YouTube Music
Can generate views on YouTube Music too. In urls.txt put your music link like this https://music.youtube.com/watch?v=xxxxx. Script will automatically load YouTube Music when it sees link have music.youtube.com. Search feature is not available for this. So you need to empty the search.txt otherwise it will start searching videos in default YouTube.

Windows
Binary Release
For windows you can download binary releases from Binary releases. Download this file named YouTube-Viewer_win_x.x.x.zip, unzip it and run the youtube_viewer.exe. Or you can install it from source. To do so keep reading.

Installation
Open command prompt and type

$ git clone https://github.com/dahabko/dahabtest.git

$ cd YouTube-Viewer

$ pip install -r requirements.txt
If something goes wrong, try again after installing latest version pip.

Important
If you've got a large proxy collection, you should run this command to filter Good proxies. Then use GoodProxy.txt for proxy in youtube_viewer.py

$ python proxy_check.py
After closing program, if chromedrivers are still running. You may want to double click killdrive.bat to close all chrome instances.

urls.txt or search.txt can't be empty. Otherwise you will see errors. Use both for better results.

Usage
Open command prompt in YouTube-Viewer folder and run
$ python youtube_viewer.py
Rest is self explanatory.
Linux / Mac
Installation
Open your favourite terminal and run

$ git clone https://github.com/dahabko/dahabtest.git

$ cd YouTube-Viewer

$ pip3 install -r requirements.txt
If something goes wrong, try again after installing latest version pip.

Important
If you've got a large proxy collection, you should run this command to filter Good proxies. Then use GoodProxy.txt for proxy in youtube_viewer.py

$ python3 proxy_check.py
After closing program, if chromedrivers are still running. Open your terminal and run

ps aux | awk '/chrome/ { print $2 } ' | xargs kill -9
urls.txt or search.txt can't be empty. Otherwise you will see errors. Use both for better results.

Usage
Open command prompt in YouTube-Viewer folder and run
$ python3 youtube_viewer.py
Rest is self explanatory.
Best Practices
To get the most out of this script you should maintain these things.

Don't use HEADLESS mode. Because no IP leak prevention, fingerprint defending, etc. can be done in headless mode.
Youtube doesn't count views from the same IP after a certain time. Like, don't expect to get 100 views from 10 proxies. If you want more views, try to use a lot of premium proxies(free proxies are flagged by most websites). DO NOT use TOR proxies.
Use both urls.txt and search.txt
And use as many urls and keyword::::title as you can. Don't use just one video.
Issues
Before opening an issue, please read this page thoroughly. Maybe someone already faced the same problem you have right now. So it's always a good idea to check the answer to issues first. If your problem isn't there, feel free to open an issue. Also, don't forget to give as many details as you can. config.json and a screenshot of terminal output provide a handful of information to resolve your problem.

Credits
I want to thank all of you who have opened an issue or shared your code snippets or ideas with me!
