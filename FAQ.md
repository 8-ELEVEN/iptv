# Frequently Asked Questions

Basic:
- [What is IPTV?](#What-is-iptv)
- [I have a cable service and I want those channels to be on this IPTV. Is that possible?](#I-have-a-cable-service-and-i-want-those-channels-to-be-on-this-iptv-is-that-possible)
- [Is it possible to view channels directly from the main website?](#Is-it-possible-to-view-channels-directly-from-the-main-website)
- [Does the playlist have a channel guide?](#Does-the-playlist-have-a-channel-guide)
- [Are you planning to include a VOD of TV shows broadcasted on this playlist?](#Are-you-planning-to-include-a-vod-of-tv-shows-broadcasted-on-this-playlist)
- [Why don't we show NSFW channels in most playlists?](#Why-dont-we-show-nsfw-channels-in-most-playlists)
- [Do I have to pay to use this list?](#Do-i-have-to-pay-to-use-this-list)

Channels:
- [Does the channel need to be FTA to be included in the playlists?](#Does-the-channel-need-to-be-FTA-to-be-included-in-the-playlists)
- [Can I add a FTA channel that broadcasts PPV events or pay programming?](#Can-I-add-a-FTA-channel-that-broadcasts-PPV-events-or-pay-programming)
- [I've created my channel and I want to add it to this playlist. What should I do?](#Ive-created-my-channel-and-i-want-to-add-it-to-this-playlist-what-should-i-do)
- [Is it possible to limit the broadcasting of my channel to my country only?](#Is-it-possible-to-limit-the-broadcasting-of-my-channel-to-my-country-only)
- [Is there any way to add my channel other than via this git repository?](#Is-there-any-way-to-add-my-channel-other-than-via-this-git-repository)

Technical:
- [Why am I asked to provide an adaptive playlist like "master.m3u8", "playlist.m3u8" or "index.m3u8"?](#Why-am-i-asked-to-provide-an-adaptive-playlist-like-masterm3u8-playlistm3u8-or-indexm3u8)
- [Why don't we accept Xtream-Codes servers inside our playlists?](#Why-dont-we-accept-xstreamcodes-servers-inside-our-playlists)
- [Is it possible to add streams from Youtube, Dailymotion or Twitch?](#Is-it-possible-to-add-streams-from-youtube-dailymotion-or-twitch)
- [Is it possible to add audio-only streams, like FM radio?](#Is-it-possible-to-add-audio-only-streams-like-fm-radio)
- [Why are there some ids with call sign (WATB-TV.us) and others with alphanumeric id (Mychannel.us)?](#Why-are-there-some-ids-with-call-sign-watb-tvus-and-others-with-alphanumeric-id-mychannelus)
- [Why attributes of channels of this playlist like "tvg-country", "tvg-language", "tvg-logo" are missing?](#Why-attributes-of-channels-of-this-playlist-like-tvg-country-tvg-language-tvg-logo-are-missing)
- [There are source for verify call sign and coverage area for some TV stations?](#There-are-source-for-verify-call-sign-and-coverage-area-for-some-tv-stations)
- [Why some streams have an empty id?](#Why-some-streams-have-an-empty-id)
- [What is a "daily update" and what are the benefits for this playlist?](#What-is-a-daily-update-and-what-are-the-benefits-for-this-playlist)

## Basic
### What is IPTV?
In non-technical words, IPTV (Internet Protocol television) stations have web addresses that *are obtained from official sources or authorized services for easier access to the end user who has any media player that supports streaming*.

Based on "[Internet Protocol television](https://en.wikipedia.org/wiki/Internet_Protocol_television)" from Wikipedia article. This article is important, because newcomers do not understand how playlists work.

### Do I need a good Internet connection to watch an available stream?
A lot of channels are ready for main public because of adaptive resolution. If you have a slow connection, play again at another time, because you may experience short stuttering and/or signal loss.

Some TV stations have a maximum of simultaneous users. So if this stream does not display correctly (becuase of bandwidth limit), you will have to play at another time.

Based on [#6791](https://github.com/iptv-org/iptv/discussions/6791).

### I have a cable service and I want those channels to be on this IPTV. Is that possible?
No. This playlist does not replace traditional cable, because this playlist can't include exclusive channels that may not be available on free-to-air. In other words, you will not have all the channels in the world. We recommend contacting your cable provider to offer legal alternatives to this service or visit the [iptv-org/awesome-iptv](https://github.com/iptv-org/awesome-iptv) repository for find other providers.

Based on [#7205](https://github.com/iptv-org/iptv/issues/7205).

### Does the playlist have a channel guide?
Yes, because an id of each channel is used to link to program guide. However, not all channels have their EPG available. See [EPG](https://github.com/iptv-org/epg) for more info. Please note that the guide is not perfect and some channels (like international feeds) may interrupt programming without you knowing.

Based on [#2438](https://github.com/iptv-org/iptv/issues/2438) and [#4537](https://github.com/iptv-org/iptv/discussions/4537).

### Is it possible to view channels directly from the main website?
No, to avoid possible abuse of the service.

Based on [https://github.com/iptv-org/iptv/issues/1002](https://github.com/iptv-org/iptv/issues/1002).

### Why don't we show NSFW channels in most playlists?
NSFW content are not suitable for the main public. To avoid issues with these kind of programmings, we've created a separate NSFW playlist available for everyone. If you want to see this type of channel, please use the NSFW playlist.

Based on [#1799](https://github.com/iptv-org/iptv/pull/1799) and [#3031](https://github.com/iptv-org/iptv/pull/3031).

### Do I have to pay to use this playlist?
No. Also, the maintenance of this service is self-financed.

### Are you planning to include a VOD of TV shows broadcasted on this playlist?
No. This is not our purpose.

Based on [#175](https://github.com/iptv-org/iptv/issues/175), [#3290](https://github.com/iptv-org/iptv/discussions/3290), [#7852](https://github.com/iptv-org/iptv/discussions/7852).

## Channels
### Does the channel need to be publicly accessible to be included in the playlists?
Yes, we need the links to be publicly accessible like FTA packages (free-to-air), online services or official websites. We recommend tagging [Geo-blocked] if it is only accessible in one or few countries.

Based on [#480](https://github.com/iptv-org/iptv/issues/480) and [#2732](https://github.com/iptv-org/iptv/issues/2732).

### Can I add a FTA channel that broadcasts PPV events or pay programming?
Maybe, this may change in future answers. Consider if the country where it is broadcasted allows fair use. Owners can ban the broadcast of PPV events, and even issue a DMCA takedown. Check the [blocklist](https://github.com/iptv-org/database/blob/master/data/blocklist.csv) for more info about specific events, and this [counternotice](https://github.com/github/dmca/blob/3ce1c9402c6b7e46dcbbea6ff866d6a44e75c72a/2020/10/2020-10-08-dfl-counternotice.md) indicating that a DMCA takedown is invalid if only one FTA channel infringes copyright.

Please remember that by sharing a link to a FTA channel (or more), you are **indexing** the link, not **restreaming** its content. This subtility makes most of the DMCA takedowns false and invalid under law.
A good example of this would be [Perfect 10 v. Google](https://www.eff.org/fr/cases/perfect-10-v-google). 
Some [valid takedowns](https://github.com/iptv-org/iptv/issues/6486) do occur when a Pull Request is made to notify us that we should not index their channels.

Based on [#6350](https://github.com/iptv-org/iptv/issues/6350).

### I've created my channel and I want to add it to this playlist. What should I do?
We are a community initiative and you don't need to pay anything to stay on this playlist. Feel free to create a channel with few resources:
* Camera with a tripod (recommended for your own studio).
* A PC with Internet, video editor and recording/broadcasting app under RTMP protocol (e.g. OBS).
* And a live streaming service with multibitrate (if possible).

After you have your m3u8 link, add your channel information onto the [Database](https://github.com/iptv-org/database) repository, and submit an [issue](https://github.com/iptv-org/iptv/issues/new) to propose it to us.

Note: There are cases of broadcasting a copy of third-party content (released previously in public) with the purpose of promoting, educating or commenting. This is known as fair use (also called "fair dealing" or "copyright exception") and should be important when broadcasting without problems on your TV channel.

### Is it possible to add my channel to broadcast only in my country?
Yes, if you do not want the channel to be broadcast outside your country (for legal reasons), we recommend using the [Geo-blocked] tag for your stream.

Based on [#2732](https://github.com/iptv-org/iptv/issues/2732) and [#6534](https://github.com/iptv-org/iptv/issues/6534).

### Is there any way to add my channel other than via this git repository?
No, there is no such option.

## Technical
### Why am I asked to provide an adaptive playlist like "master.m3u8", "playlist.m3u8" or "index.m3u8"?
An adaptive playlist is a m3u8 file that contains certain informations: the bandwidth, the quality, the type of codec used to read the channel. The player then reads the channel playlist based on your bandwidth and screen (hence the name "adaptive"). This permits you to watch your channel on perfect conditions.

In the "daily update", the stream with the best supported resolution will be considered "priority" over other lower resolution streams of the same channel.

Based on [#1916](https://github.com/iptv-org/iptv/issues/1916).

### Why don't we accept Xtream-Codes servers inside our playlists?
Xtream-Codes streams are, most of the times, pirated streams created by some people that can get satellite and/or PPV streams and that propose it to everyone for a fairer price. These types of servers are illegal and also highly unstable, since it depends either from the user who bought it or the server that hosts it.

In short, they are poor quality streams created by unauthorized people.

If you're unsure about if your link is from an Xtream-Codes server, you may:
* Look at the structure of the URL. Most of them have this form : http(s)://*hostname*:25461/*username*/*password*/*channelID* (port is often 25461)
* Remove the rest of the URL after the password mention and add either "panel_api.php?" or "player_api.php?" after the port. Replace the slashes between the username and password with "username=" and "password=". 

If the link matches or answers after changing the URL, you're with an Xtream-Codes server.

Based on [#5236](https://github.com/iptv-org/iptv/pull/5236) and [#5401](https://github.com/iptv-org/iptv/pull/5401).

### Is it possible to add streams from Youtube, Dailymotion or Twitch?
Yes. Due to technical limitations, it is necessary to add a [Streamlink](https://streamlink.github.io/) server link to view the content.

Based on [#4112](https://github.com/iptv-org/iptv/discussions/4412).

### Is it possible to add audio-only streams, like FM radio?
No. Exceptions are the visual radios, in which a video and audio are shown at the same time. A WIP repository made by one member of iptv-org, [LaneSh4d0w](https://github.com/LaneSh4d0w) aims to collect radio streams, on the [IPRD](https://github.com/LaneSh4d0w/IPRD) repository.

Based on [#2758](https://github.com/iptv-org/iptv/pull/2758) (visual radio example), [#5794](https://github.com/iptv-org/iptv/discussions/5794) and [#6044](https://github.com/iptv-org/iptv/discussions/6044).

### Why are there some call sign (KJLA-DT1.us) as ids and alphanumeric names as ids (Mychannel.us)?
It's to differentiate the origin of the broadcast from the content. Call signs usually come from physical stations in the country of origin and their programming is subject to change. If the channel is not from a television station, the brand name will be used.

An example of a call sign used as id is `KJLA-DT1.us`: [KJLA](https://en.wikipedia.org/wiki/KJLA) is a digital television station, DT is a suffix, 1 is a subchannel number and ".us" is the country code (United States). This station broadcasts the Visión Latina channel, whose id is `VisionLatina.us`.

Based on [#5818](https://github.com/iptv-org/iptv/discussions/5818).

### There are source for verify call sign and coverage area for some TV stations?
There are websites to consult the location and characteristics of the station. For example, [FCCData](https://fccdata.org/) for US, Canada, Mexico, UK, Australia and Japan.

### Why attributes of channels of this playlist like "tvg-country", "tvg-language", "tvg-logo" are missing?
The reason is to reduce the workload when adding streams in the list. Since "tvg-id" links to the [Database](https://github.com/iptv-org/database) repository, each channel has unique attributes like image, name (in English and local speak), country (or countries) broadcasted, category and language.

You can add multiple streams with a single id (in the "tvg-id" parameter), instead of adding information from scratch. For example:

```
#EXTINF:-1 tvg-id="CCTV3.cn",CCTV-3综艺 (1080p)
```
Based on [#2086](https://github.com/iptv-org/iptv/issues/2086) (countries) and [#6516](https://github.com/iptv-org/iptv/issues/6516) (use of Database).

### Why some streams have an empty id?
Because the stream does not have enough information available. If you appear to know additional data on these, let us know its official name, the language it broadcasts and the country where it originates.

This also applies to the undefined.m3u file. The streams in this file are from channels whose country of origin is unknown.

Based on [#2440](https://github.com/iptv-org/iptv/issues/2440).

### What is a "daily update" and why are the benefits for this playlist?
A "daily update" is a pull request made for maintenance purposes. It checks the status of the playlist operation, and reclassifies the streams internally. This will be useful on playlist recreation, as it's gonna hide streams from the playlist if they have access problems.

Based on [#6524](https://github.com/iptv-org/iptv/discussions/6524) and [#6855](https://github.com/iptv-org/iptv/issues/6855).
