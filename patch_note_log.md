# V1.0.4
- Fixed Choice Update List Updating improperly for category choices
- Renamed some state descriptions - Nothing needs changed on the user side.
- Fixed plugin crash due to emojis in channel or video description
- When trying to connect to a live chat if none are available the popup will now tell you instead of staying silent. 


# V1.0.3
- corrected an issue where if you selected the X button on popup the plugin would crash
- Released Linux version
- MacOS is available for testing


# V1.0.2
- Fixed error when trying to manually connect to a scheduled/live broadcast and there was none
- Fixed error when trying to cancel out of the stream selection window
- Fixed plugin not asking to authenticate for new users
- Removed the need to input your own channel ID
- Added Auto Connect to plugin settings - not unfunctional yet


# V1.0.1
- Fixed chatter events not working properly
- Fixed chatter profile image URL
- Added chatter profile icon
- Renamed Live Video License state from current_live_video_license to current_live.video.license
- Fixed description and title not showing properly for live videos
- All states for Live Video Stream should now update on schedule after going live 
- When stream goes offline you are automatically disconnected from live chat after 90 seconds
