
# Youtube-Plugin
- [Youtube Plugin](#Youtube-Plugin)
  - [Description](#description) 
  - [Settings Overview](#Settings-Overview)
  - [Actions / States / Events](#Features)
    - [Actions](#actions)
        - [YouTube](#tp.plugin.youtube.mainactions)
    - [States](#states)
        - [YouTube](#tp.plugin.youtube.mainstates)
        - [Channel Details](#tp.plugin.youtube.channel_infostates)
        - [Live Stream Details](#tp.plugin.youtube.live_statsstates)
        - [Chatter 0-5 States](#tp.plugin.youtube.chatter0states)
    - [Events](#events)
        - [SuperSticker Event](#tp.plugin.youtube.superStickerstates)
        - [SuperChat Event](#tp.plugin.youtube.superChatstates)
        - [New Sponsor Event](#tp.plugin.youtube.newSponsorstates)
  - [Bugs and Support](#bugs-and-suggestion)
  
# Description

Youtube Plugin for TouchPortal - Created by yours truly.

## Settings Overview
| Read-only | Type | Default Value |
| --- | --- | --- |
| False | text | Basic |


# Features

## Actions
<details open id='tp.plugin.youtube.mainactions'><summary><b>Category:</b> YouTube <small><ins>(Click to expand)</ins></small></summary><table>
<tr valign='buttom'><th>Action Name</th><th>Description</th><th>Format</th><th nowrap>Data<br/><div align=left><sub>choices/default (in bold)</th><th>On<br/>Hold</sub></div></th></tr>
<tr valign='top'><td>Send Message</td><td> </td><td>Delete Message: [1]</td><td><ol start=1><li>Type: text &nbsp; 
&lt;empty&gt;</li>
</ol></td>
<td align=center>No</td>
<tr valign='top'><td>TimeOut Chatter</td><td> </td><td>Timeout: [1] for [2] seconds</td><td><ol start=1><li>Type: text &nbsp; 
&lt;empty&gt;</li>
<li>Type: text &nbsp; 
&lt;empty&gt;</li>
</ol></td>
<td align=center>No</td>
<tr valign='top'><td>Select a Live Chat</td><td> </td><td>This action will cause a popup to appear. please select the stream you wish to connect to</td><td><ol start=1><li>Type: text &nbsp; 
&lt;empty&gt;</li>
</ol></td>
<td align=center>No</td>
<tr valign='top'><td>Turn the Auto Connect on or off</td><td> </td><td>Auto Connect [1]</td><td><ol start=1><li>Type: choice &nbsp; 
Default: <b></b> Possible choices: ['On', 'Off']</li>
</ol></td>
<td align=center>No</td>
</tr></table></details>
<br>

## States
![image](https://user-images.githubusercontent.com/76603653/185533838-364a1e15-81ae-4a6c-988f-91c6b25717a7.png)
<details id='tp.plugin.youtube.mainstates'><summary><b>Category:</b> YouTube <small><ins>(Click to expand)</ins></small></summary>



| Id | Description | DefaultValue | parentGroup |
| --- | --- | --- | --- |
| .state.plugin_status | YT Plugin Status |  |   |
| .state.plugin_status.retry.timer | YT Plugin Status Retry Timer |  |   |
| .state.plugin_status.retry.attempts | YT Plugin Status Retry Attempts |  |   |
</details>

<details id='tp.plugin.youtube.channel_infostates'><summary><b>Category:</b> YT Channel Info <small><ins>(Click to expand)</ins></small></summary>


| Id | Description | DefaultValue | parentGroup |
| --- | --- | --- | --- |
| .state.channel.total_subscribers | YT | Total Channel  Subscribers |  |   |
| .state.channel.total_videos | YT | Total Channel Videos |  |   |
| .state.channel.total_channel_views | YT | Total Channel Views |  |   |
</details>

<details id='tp.plugin.youtube.live_statsstates'><summary><b>Category:</b> YT Live Stream Info <small><ins>(Click to expand)</ins></small></summary>


| Id | Description | DefaultValue | parentGroup |
| --- | --- | --- | --- |
| .state.channel.current_live_title | YT | Live Title |  |   |
| .state.channel.current_live_description | YT | Live Description |  |   |
| .state.channel.current_live.concurrentViewers | YT | Live Concurrent Viewers |  |   |
| .state.channel.current_live.viewCount | YT | Live Total View Count |  |   |
| .state.channel.current_live.likeCount | YT | Live Like Count |  |   |
| .state.channel.current_live.disLikeCount | YT | Live Dislike Count |  |   |
| .state.channel.current_live.favoriteCount | YT | Live Favorite Count |  |   |
| .state.channel.current_live.commentCount | YT | Live Comment Count |  |   |
| .state.channel.current_live.startTime | YT | Live Start Time |  |   |
</details>

<details id='tp.plugin.youtube.chatter0states'><summary><b>Category:</b> Chatter 0 <small><ins>(Click to expand)</ins></small></summary>


| Id | Description | DefaultValue | parentGroup |
| --- | --- | --- | --- |
| .state.Chatter_0.name | YouTube: Chatter 0 - Name |  |   |
| .state.Chatter_0.message | YouTube: Chatter 0 - Message |  |   |
| .state.Chatter_0.message.id | YouTube: Chatter 0 - Message ID |  |   |
| .state.Chatter_0.profile_image | YouTube: Chatter 0 - Profile Image URL |  |   |
</details>

<details id='tp.plugin.youtube.chatter1states'><summary><b>Category:</b> Chatter 1 <small><ins>(Click to expand)</ins></small></summary>


| Id | Description | DefaultValue | parentGroup |
| --- | --- | --- | --- |
| .state.Chatter_1.name | YouTube: Chatter 1 - Name |  |   |
| .state.Chatter_1.message | YouTube: Chatter 1 - Message |  |   |
| .state.Chatter_1.message.id | YouTube: Chatter 1 - Message ID |  |   |
| .state.Chatter_1.profile_image | YouTube: Chatter 1 - Profile Image URL |  |   |
</details>

<details id='tp.plugin.youtube.chatter2states'><summary><b>Category:</b> Chatter 2 <small><ins>(Click to expand)</ins></small></summary>


| Id | Description | DefaultValue | parentGroup |
| --- | --- | --- | --- |
| .state.Chatter_2.name | YouTube: Chatter 2 - Name |  |   |
| .state.Chatter_2.message | YouTube: Chatter 2 - Message |  |   |
| .state.Chatter_2.message.id | YouTube: Chatter 2 - Message ID |  |   |
| .state.Chatter_2.profile_image | YouTube: Chatter 2 - Profile Image URL |  |   |
</details>

<details id='tp.plugin.youtube.chatter3states'><summary><b>Category:</b> Chatter 3 <small><ins>(Click to expand)</ins></small></summary>


| Id | Description | DefaultValue | parentGroup |
| --- | --- | --- | --- |
| .state.Chatter_3.name | YouTube: Chatter 3 - Name |  |   |
| .state.Chatter_3.message | YouTube: Chatter 3 - Message |  |   |
| .state.Chatter_3.message.id | YouTube: Chatter 3 - Message ID |  |   |
| .state.Chatter_3.profile_image | YouTube: Chatter 3 - Profile Image URL |  |   |
</details>

<details id='tp.plugin.youtube.chatter4states'><summary><b>Category:</b> Chatter 4 <small><ins>(Click to expand)</ins></small></summary>


| Id | Description | DefaultValue | parentGroup |
| --- | --- | --- | --- |
| .state.Chatter_4.name | YouTube: Chatter 4 - Name |  |   |
| .state.Chatter_4.message | YouTube: Chatter 4 - Message |  |   |
| .state.Chatter_4.message.id | YouTube: Chatter 4 - Message ID |  |   |
| .state.Chatter_4.profile_image | YouTube: Chatter 4 - Profile Image URL |  |   |
</details>

<details id='tp.plugin.youtube.chatter5states'><summary><b>Category:</b> Chatter 5 <small><ins>(Click to expand)</ins></small></summary>
</details>

## Events
<details id='tp.plugin.youtube.mainstates'><summary><b>Category:</b> YouTube <small><ins>(Click to expand)</ins></small></summary>

| Id | Description | DefaultValue | parentGroup |
| --- | --- | --- | --- |
| .state.Chatter_5.name | YouTube: Chatter 5 - Name |  |   |
| .state.Chatter_5.message | YouTube: Chatter 5 - Message |  |   |
| .state.Chatter_5.message.id | YouTube: Chatter 5 - Message ID |  |   |
| .state.Chatter_5.profile_image | YouTube: Chatter 5 - Profile Image URL |  |   |
</details>

<details id='tp.plugin.youtube.superStickerstates'><summary><b>Category:</b> SuperSticker Event <small><ins>(Click to expand)</ins></small></summary>


| Id | Description | DefaultValue | parentGroup |
| --- | --- | --- | --- |
| .state.superSticker.name | YouTube: SuperSticker - Name |  |   |
| state.superSticker.channel_id | YouTube: SuperSticker - Channel ID |  |   |
| .state.superSticker.message | YouTube: SuperSticker - Message |  |   |
| .state.superSticker.profile_image | YouTube: SuperSticker - Profile Image URL |  |   |
| .state.superSticker.amount | YouTube: SuperSticker - Amount |  |   |
</details>

<details id='tp.plugin.youtube.superChatstates'><summary><b>Category:</b> SuperChat Event <small><ins>(Click to expand)</ins></small></summary>


| Id | Description | DefaultValue | parentGroup |
| --- | --- | --- | --- |
| .state.superChat.name | YouTube: SuperChat - Name |  |   |
| state.superChat.channel_id | YouTube: SuperChat - Channel ID |  |   |
| .state.superChat.message | YouTube: SuperChat - Message |  |   |
| .state.superChat.profile_image | YouTube: SuperChat - Profile Image URL |  |   |
| .state.superChat.amount | YouTube: SuperChat - Amount |  |   |
</details>

<details id='tp.plugin.youtube.newSponsorstates'><summary><b>Category:</b> New Sponsor Event <small><ins>(Click to expand)</ins></small></summary>


| Id | Description | DefaultValue | parentGroup |
| --- | --- | --- | --- |
| .state.NewSponsor.name | YouTube: New Sponsor - Name |  |   |
| state.NewSponsor.channel_id | YouTube: New Sponsor - Channel ID |  |   |
| .state.NewSponsor.message | YouTube: New Sponsor - Message |  |   |
| .state.NewSponsor.profile_image | YouTube: New Sponsor - Profile Image URL |  |   |
| .state.NewSponsor.amount | YouTube: New Sponsor - Amount |  |   |
</details>

<br>

# Bugs and Suggestion
Open an issue on github or join offical [TouchPortal Discord](https://discord.gg/MgxQb8r) for support.



