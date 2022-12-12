# twitch-m3u8-on-cloudflare
> Get the stream URL of a Twitch livestream or past broadcast (VOD)

## Features
* Supports both livestreams and past broadcasts (VODs)    
* 0 dependencies   
* Promise-based    
* Can return raw .m3u8 data    

## ToDo
- Fix VOD

## Usage
1. Deploy this code onto a [cloudflare worker](https://developers.cloudflare.com/workers/)

2. assemble the url like the below:
`https://<your-url>.workers.dev?streamer=<streamer-name>`

3. copy and paste that url into VLC to watch the stream.

JSON feed is also available if you need programmatic access.
`https://<your-url>.workers.dev?streamer=<streamer-name>&json=true`

## Credits
Original NodeJS refactor was done by [Samuel Dudik](https://github.com/dudik/twitch-m3u8)
All reverse engineering of the GraphQL API was taken from the [streamlink](https://github.com/streamlink/streamlink) project. 


## License
[MIT](https://github.com/0xw1sky/twitch-m3u8-on-cloudflare/blob/master/LICENSE)
