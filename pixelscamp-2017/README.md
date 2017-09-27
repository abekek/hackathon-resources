# PixelsCamp 2017 - https://pixels.camp

Summay of Cisco Presence:
- Booth activities: Cisco Spark Board demoes and [Grab the bag!](https://developer.cisco.com/join/pixelscamp2017) activity
- [Coding challenge](#coding)
- ["Creating advanced Enterprise Bots" talk](https://github.com/PixelsCamp/talks/blob/master/2017/building-advanced-bots_steve_sfartz.md)

![challenges](img/challenges.png)


## <a name="coding"></a>Coding Challenge

Create the best PixelsCamp event dashboard.

Win a Cisco Meraki MR32 (Cloud Managed Wireless Access Point).


### Schedule

- Thursday, 12h00: Cisco CMX Challenge starts

- till Saturday, 11h00: Submit your hack via [Pending submission link]()

- Saturday, 12h15: Pitches at Cisco booth
   - 3' pitch, 5' questions
   - 12h20: team name
   - 12h30: team name
   - 12h40: team name
   - 12h50: team name
   - 13h00: team name

- Saturday, 13h30: Winner announced at Cisco booth


### Support 

Simply reach to the Cisco booth on-site, or fill in your [email here](https://eurl.io/#Bkm0tVFoZ) to join the Cisco Spark "PixelsCamp Cisco Challenge" support space.


### Judging criteria

- UX/Design of the dahboard
- Relevance of information (CMX Data)
- Use of [Cisco Spark APIs](https://developer.ciscospark.com/) (for Chatops, Bots or Video)


### CMX resources

- [CMX API DevNet Resources Center](https://developer.cisco.com/site/cmx-mobility-services/)
- [DevNet Learning lab "Introduction to CMX"](https://learninglabs.cisco.com/modules/dna-cmx-mse/09-cmx-01-introduction-to-cmx/step/1
)
- CMX API endpoint at PixelsCamp
   - https://53cdgr.cmxcisco.com
   - Authorization: Basic cGl4ZWxzY2FtcEBjaXNjby5jb206cGl4ZWxzY2FtcDIwMTc=

- Example
    ```shell
    curl -X GET -H "authorization: Basic cGl4ZWxzY2FtcEBjaXNjby5jb206cGl4ZWxzY2FtcDIwMTc=" https://53cdgr.cmxcisco.com/api/presence/v1/passerby/hourly/today?siteId=1477307415943
    ```

![cmx](img/cmx.png)