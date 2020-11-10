# VXG.API.Samples

Overview
The API functions are divided in several sections. Interactive API reference (Swagger) can be found in the Docs & API section on the dashboard in corresponding API sections.

Admin API
Add/edit/delete cameras.
Manage storage and bandwidth limits.
Retrieve usage statistics.
Store/retrieve meta information.
The API documentaion and an online testing tool can be found here: Admin API
The API authorization is described here

Channel API
Get live video URLs.
Get recorded video.
Get stored images and clips.
Store new images and clips.
Get recoreded video timeline.
Communication channel (Websocket) for cloud cameras.
The API documentaion and an online testing tool can be found here: Channel API
The API authorization is described here

Artificial Intelligence (AI) API
Generate images from recorded video.
Generate images from live video.
Create clips.
Get live video.
Get recorded video.
The API documentaion and an online testing tool can be found here: Channel API
The API authorization is described here

Camera Settings API
Video settings: bitrate, framerate, resolution, etc.
Audio settings.
PTZ.
Apparance.
Motion and audio detectors.
System settings.
The API documentaion and an online testing tool can be found here: Channel API
The API authorization is described here

Events and Notification API
Put/Get metadata and events.
Send notifications.
The API documentaion and an online testing tool can be found here: Channel API
The API authorization is described here

Admin API authorization
To authorize your requests to Admin API you need to use your license key that you can find in the VXG dashboard: https://dashboard.videoexpertsgroup.com/?products=

The API Key should be injected to Authorization header of every request to Admin API like this:

Authorization: LKey %license_key%
For example, if the API key is "X9tKpuXq0btatj":

Authorization: LKey X9tKpuXq0btatj
Non-admin API authorization
All function calls require an authorization header.

'Authorization: Acc %channel_access_token%'
The %channel_access_token% can be retrieved in two ways:
a. Using Admin API during creating a channel or updating of a channel access token.
b. Using Cloud/Server Admin UI page.

Example of an authorization header:

'Authorization: Acc eyJhY2Nlc3MiOiAid2F0Y2giLCAidG9rZW4iOiAic2hhcmUuZXlKemFTSTZJRE14T0RoOS41YWEyMjA2N3QxMmNmZjc4MC5GVHpEeUZMYkVLQVNzM2ZJRFZaSDdFMEhhdGMiLCAiY2FtaWQiOiAxMzI0NDUsICJjbW5ncmlkIjogMTMyODUwLCAiYXBpIjogIndlYi5za3l2ci52aWRlb2V4cGVydHNncm91cC5jb20ifQ=='

