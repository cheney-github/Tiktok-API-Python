# Tiktok API 
API Tiktok use Python
## Get video no watermark 
```python
import requests

url = "https://tiktok-video-no-watermark1.p.rapidapi.com/tiktok/nwm/6883765092236791041"

headers = {
    'x-rapidapi-key': [YOUR API KEY],
    'x-rapidapi-host': "tiktok-video-no-watermark1.p.rapidapi.com"
    }

response = requests.request("GET", url, headers=headers)

print(response.text)
```
https://rapidapi.com/AdKT36/api/tiktok-video-no-watermark1

## Tool download All video
- Support downloading all video users on 4 platforms: TikTok, TikTok China (Douyin), Kwai, Kwai China (Kuaishou)
- Video quality full HD
- Download multiple channels at the same time
- Automatically create cross-platform folders and download IDs
=>  https://youtu.be/btpZPN7kFOU
=>  anhk1996@gmail.com
# Install
pip install requests

# How to use
```python
import TiktokApi
Api = TiktokApi.Tiktok()
```
## getUser
```python
user = Api.getUser('vtkh2004')
print(user)
```
## getUserFeed
```python
userfeed  = Api.getUserFeed('vtkh2004', '0')
print(userfeed)
```
## getMusic
```python
music = Api.getMusic('6896022404674800386')
print(music)
```
## getMusicFeed
```python
musicfeed  = Api.getMusicFeed('6896022404674800386', '0')
print(musicfeed)
```
## getChallenge
```python
challenge = Api.getChallenge('foryou')
print(challenge)
```
## getChallengeFeed
```python
challengefeed  = Api.getChallengeFeed('foryou', '0')
print(challengefeed)
```
## getTredingFeed
```python
trending = Api.getTrendingFeed('0')
print(trending)
```

## getInfoVideo
```python
vid = Api.getInfoVideo('https://www.tiktok.com/@tiktok/video/6801895105885195526')
print(vid)
```

## DownloadVideoNoWatermark
Download video no watermark by id, select folder save: video
```python
Api.DownloadVideoNoWatermark('6897853325761350913', 'video')
```
