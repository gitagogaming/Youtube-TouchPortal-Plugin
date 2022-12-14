# V1.1.3
- added in disconnect action
- added in new subscriber event(checks every 60 seconds currently)
- Fixed issue with selecting a live chat where it was not correctly connecting to the desired chat
- Fixed issue with selecting a live stream when it was not pre-scheduled
- Fixed Select a Broadcast Action - It now has choice selections
- Fixed some issues with auto-connect
- Fixed shutdown error

# V1.1.2
- Fixed an issue where plugin would not start properly or may stop working unexpectedly
- Removed the need for images from asset folder as they were causing an issue for some people when selecting a broadcast
  They are now stored permanently in the plugin as a Base64 String.

# V1.1.1
- Fixed Multiple chatter states being incorrectly labeled 
- States Removed - `.state.Chatter_2.profile_image` 
- States Added / Modified - `.state.Chatter_2.profile_image.url` and  `.state.Chatter_2.profile_image.icon`
- New Chatter States added for isVerified, IsChatSponsor and IsChatModerator

# V1.1.0
- Create New Broadcast (You may save a template for future use)
- Moved Select Live Stream to the Create New Broadcast Pop-Up
- Delete Broadcast is available also in this new GUI
- Save + Load Presets for Broadcasts
- Change Video Thumbnail (Use this if you decide to change games during your multi hour live stream)
- Removed the setting for 'auto connect' - The action is **still there** but not the "in the plugin settings"

# V1.0.6
- Fixed issue causing Select a Broadcast action to not work properly

# V1.0.5
- Slight revamp of Stream Selection Popup to make it easier to read
- When no broadcsts are available you will now have the option to open a browser to create one manually

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
