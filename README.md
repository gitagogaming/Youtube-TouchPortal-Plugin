
# Youtube-Plugin

![progreesss (1)](https://user-images.githubusercontent.com/76603653/185826537-0eff3ffd-d6ee-485d-bee4-e4724b4ed07f.jpg)


- [Youtube Plugin](#Youtube-Plugin)
  - [Description](#description) 
  - [Install Instructions](#install_instructions)
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
  - [FAQ](#faq)
  - [Terms of Service](#terms-of-service)
  - [Bugs and Support](#bugs-and-suggestion)
  
# Description
Control your YouTube Live stream using TouchPortal on your mobile device


# Install Instructions
1) **Download Plugin** -> [Releases](https://github.com/gitagogaming/Youtube-TouchPortal-Plugin/releases)
2) **Install Plugin** -> [How-To](https://www.touch-portal.com/blog/post/tutorials/import-plugin-guide.php#:~:text=Importing%20a%20plugin%20file&text=A%20Touch%20Portal%20plug-in%20file%20has%20the%20.,icon%20in%20the%20system%20tray.)
3) **Accept Authorizations** -> [How-To](#Accept-Authorization)<br>





## Settings Overview
| Read-only | Type | Default Value |
| --- | --- | --- |
| False | text | Basic |


# Features

## Actions
<details open id='tp.plugin.youtube.mainactions'><summary><b>Category:</b> YouTube <small><ins>(Click to expand)</ins></small></summary><table>
<tr valign='buttom'><th>Action Name</th><th>Description</th><th>Format</th><th nowrap>Data<br/><div align=left><sub>choices/default (in bold)</th><th>On<br/>Hold</sub></div></th></tr>
<tr valign='top'><td>YT | Chat: Send Message</td><td> </td><td>Send Message: [1]</td><td><ol start=1><li>Type: text &nbsp; 
&lt;empty&gt;</li>
</ol></td>
<td align=center>No</td>
<tr valign='top'><td>YT | Chat: Delete Message</td><td> </td><td>Delete MessageID: [1]</td><td><ol start=1><li>Type: text &nbsp; 
&lt;empty&gt;</li>
</ol></td>
<td align=center>No</td>
<tr valign='top'><td>YT | Chat: TimeOut Chatter</td><td> </td><td>Timeout: [1] for [2] seconds</td><td><ol start=1><li>Type: text &nbsp; 
&lt;empty&gt;</li>
<li>Type: text &nbsp; 
&lt;empty&gt;</li>
</ol></td>
<td align=center>No</td>
<tr valign='top'><td>YT | Connect: Select a Live Chat</td><td> </td><td>This action will cause a popup to appear. please select the stream you wish to connect to</td><td><ol start=1><li>Type: text &nbsp; 
&lt;empty&gt;</li>
</ol></td>
<td align=center>No</td>
<tr valign='top'><td>YT | Connect: Turn the Auto Connect on or off</td><td> </td><td>Auto Connect [1]</td><td><ol start=1><li>Type: choice &nbsp; 
Default: <b></b> Possible choices: ['On', 'Off']</li>
</ol></td>
<td align=center>No</td>
<tr valign='top'><td>YT | Update: Video Category</td><td> </td><td>Change Category to [1]</td><td><ol start=1><li>Type: choice &nbsp; 
&lt;empty&gt;</li>
</ol></td>
<td align=center>No</td>
<tr valign='top'><td>YT | Update: Video Title</td><td> </td><td>Change Title to [1]</td><td><ol start=1><li>Type: text &nbsp; 
&lt;empty&gt;</li>
</ol></td>
<td align=center>No</td>
<tr valign='top'><td>YT | Update: Video Description</td><td> </td><td>Change Description to [1]</td><td><ol start=1><li>Type: text &nbsp; 
&lt;empty&gt;</li>
</ol></td>
<td align=center>No</td>
<tr valign='top'><td>YT | Update: Video Language</td><td> </td><td>Change Language to to [1]</td><td><ol start=1><li>Type: text &nbsp; 
&lt;empty&gt;</li>
</ol></td>
<td align=center>No</td>
<tr valign='top'><td>YT | Update: Video Tags</td><td> </td><td>Change Stream Tags to [1]</td><td><ol start=1><li>Type: text &nbsp; 
&lt;empty&gt;</li>
</ol></td>
<td align=center>No</td>
<tr valign='top'><td>YT | Update: Public Stats Viewable</td><td> </td><td>Change Public Stats Viewable to [1]</td><td><ol start=1><li>Type: choice &nbsp; 
Default: <b></b> Possible choices: ['True', 'False']</li>
</ol></td>
<td align=center>No</td>
<tr valign='top'><td>YT | Update: Video License</td><td> </td><td>Change video_license to [1]</td><td><ol start=1><li>Type: choice &nbsp; 
Default: <b></b> Possible choices: ['Creative Common', 'YouTube']</li>
</ol></td>
<td align=center>No</td>
<tr valign='top'><td>YT | Video Privacy</td><td> </td><td>Change Video Privacy to [1]</td><td><ol start=1><li>Type: choice &nbsp; 
Default: <b></b> Possible choices: ['Public', 'Unlisted', 'Private']</li>
</ol></td>
<td align=center>No</td>
<tr valign='top'><td>YT | Update: isMadeforKids</td><td> </td><td>Change Video Is Made for Kids status to [1]</td><td><ol start=1><li>Type: choice &nbsp; 
Default: <b></b> Possible choices: ['True', 'False']</li>
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


# FAQ
Q) How do I connect?<br>
A) You have two ways to connect to your live streams. <br>
  1) Use an Action which displayes a pop up window with all your live streams that may be available.<br>
  ![image](https://user-images.githubusercontent.com/76603653/189020404-2c8bf9fd-f1e5-4bc1-8b6f-8db1af48f0ea.png)<br>
  2) Turn On Auto Connect and it will connect to the any live stream you have available.<br>
 
 # Accept Authorization
 ![witharrowsOKGMGMG (1)](https://user-images.githubusercontent.com/76603653/186208322-cd40c5b6-77f4-46c8-b0a8-b036a914fa16.jpg)<br><br>


# Terms of Service

By using the YouTube Live integration created by Gitago, you are agreeing to be bound by the following terms and conditions ("Terms of Service").

If the owner makes changes to these Terms, we will post a notice within the TouchPortal Discord [channel specified](https://discord.com/channels/548426182698467339/1010166073229836340/1010378470649503794) and on the [Github Project Page](https://github.com/gitagogaming/Youtube-TouchPortal-Plugin/) before the changes become effective. Any new plugin features added in the future that augment or enhance the current Service shall be subject to the Terms of Service. Continued use of the Service after any such changes shall constitute your consent to such changes.

Violation of any of the terms below will result in the termination of your Account. 
You agree to use the Service at your own risk.
  - You must be thirteen (13) years or older to use this Service.
  - You are responsible for maintaining the security of your account and specifically your refresh token.  We cannot and will not be liable for any loss or damage from your failure to comply with this security obligation.
	
  
Users may access the integration by using TouchPortal. Any use of this integration is bound by these Terms of Service, [Youtube's Terms of Service](https://www.youtube.com/t/terms), plus the following specific terms:

- You expressly understand and agree that we shall not be liable for any direct, indirect, incidental, special, consequential or exemplary damages, including but not limited to, damages for loss of profits, goodwill, use, data or other intangible losses, resulting from your use of the integration.
- We reserve the right at any time to modify or discontinue, temporarily or permanently, your access to the integration (or any part thereof) with or without notice.
- Your use of the Service is at your sole risk. The service is provided on an “as is” and “as available” basis.
- If your quota usage significantly exceeds the average quota usage of other TouchPortal users, we reserve the right to throttle your API requests until you can reduce your quota consumption.
- We do not and can not warrant that (i) the service will meet your specific requirements, (ii) the service will be uninterrupted, timely, secure, or error-free, (iii) the results that may be obtained from the use of the service will be accurate or reliable, (iv) the quality of any products, services, information, or other material purchased or obtained by you through the service will meet your expectations, and (v) any errors in the Service will be corrected.
- You understand and agree that we shall not be liable for any direct, indirect, incidental, special, consequential or exemplary damages, including but not limited to, damages for loss of profits, goodwill, use, data or other intangible losses. The failure to exercise or enforce any right or provision of the Terms of Service shall not constitute a waiver of such right or provision.


Questions about the Terms of Service should be sent to gitagogaming@gmail.com.

Any information you provide to us during the Authorization process will be only used to generate your YouTube Live credentials.
Your credentials are only ever stored locally on your computer in the plugin directory which is accessed by the plugin as needed. TouchPortal and this YouTube integration do not store or share your YouTube Live credentials.
Any other information regarding your YouTube account is only ever accesssed and stored locally on your computer. 
Please see Google Privacy Policy for more details

# Bugs and Suggestion
Open an issue on github or join offical [TouchPortal Discord](https://discord.gg/MgxQb8r) for support.
