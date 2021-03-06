# PixelsCamp 2017 - https://pixels.camp

Summay of Cisco Presence:
- ["Grab the bag!" challenge](https://developer.cisco.com/join/pixelscamp2017) and Cisco Spark Board & Videos demoes at the Cisco DevNet booth
- [48h Coding challenge](#coding)
- Talk ["Creating advanced Enterprise Bots"](https://github.com/PixelsCamp/talks/blob/master/2017/building-advanced-bots_steve_sfartz.md): friday at noon

**[join DevNet - Cisco's Developer Program](https://developer.cisco.com/join/pixelscamp2017)** to access Cisco Dev Centers, API learning resources, sandboxes and receive our newsletter.

![challenges](img/challenges.png)


## <a name="coding"></a>Coding Challenge

Create the best PixelsCamp event dashboard.

Win a Cisco Meraki MR53 (Cloud Managed Wireless Access Point).


### Schedule

- Thursday, 12h00: Cisco CMX Challenge starts

- till Saturday, 11h00: Coding time... make sure to [submit your hack by 11AM on saturday](https://app.smartsheet.com/b/form/04ed4a7c44c74cfb98e0f87a0dc96f42), we'll come back to you with a slot to pitch (check below)

- Saturday, 12h15: Pitches at Cisco booth
   - 3' pitch, 5' questions
   
   - **12h30: Pixels Wi-FI**
   - **12h45: Cisco Dashboard**
   
- Saturday, 13h30: Winner announced at Cisco booth


### Support 

Simply reach to the Cisco booth on-site, or fill in your [email here](https://eurl.io/#Bkm0tVFoZ) to join the Cisco Spark "PixelsCamp Cisco Challenge" support space.


### Judging criteria

- UX/Design of the dashboard
- Relevance of information (CMX Data)
- Published on Github under an Apache or MIT License
- Bonus: use of [Cisco Spark APIs](https://developer.ciscospark.com/) (for Chatops, Bots or Video)


### CMX API resources

- [CMX API DevNet Resources Center](https://developer.cisco.com/site/cmx-mobility-services/)
- [DevNet Learning lab "Introduction to CMX"](https://learninglabs.cisco.com/modules/dna-cmx-mse/09-cmx-01-introduction-to-cmx/step/1
)
- CMX API endpoint at PixelsCamp
   - [Presence API documentation](https://www.cisco.com/c/en/us/td/docs/wireless/mse/cmxcloud/api/b_cmxcloud_api_reference/b-cmx-102-api-reference-guide_chapter_0100.html)
   - HTTP Authorization header: Basic cGl4ZWxzY2FtcEBjaXNjby5jb206cGl4ZWxzY2FtcDIwMTc=

- Example
    ```shell
    curl -X GET -H "authorization: Basic cGl4ZWxzY2FtcEBjaXNjby5jb206cGl4ZWxzY2FtcDIwMTc=" https://53cdgr.cmxcisco.com/api/presence/v1/clients?siteId=1505913182364
    ```

    Note that the siteId filter above does not seem to be effective. Then you'll need to filter out the clients that do not belong to PixelsCamp infrastructure: '1505913182364'

- Presence - Client details: [full json sample](presence_client_details.json)

```json
{
    "macAddress": "74:5c:9f:63:99:c4",
    "changedOn": 1506594349336,
    "status": "CONNECTED",
    "ipv4Address": "88.157.242.62",
    "ipv6Address": null,
    "ssid": "PixelsCamp",
    "bytesReceived": 0,
    "bytesSent": 0,
    "lastSiteId": 1505913182364,
    "currentSiteId": 1505913182364,
    "rssi": -51,
    "currentSiteName": "PixelsCamp",
    "changedOnTimeStamp": "2017-09-28 10:25:336",
    "lastApMacAddress": "f4:0f:1b:34:a9:a0",
    "currentApMacAddress": "f4:0f:1b:34:a9:a0",
    "currentApName": "AP_MainEvent_9",
    "lastApName": "AP_MainEvent_9",
    "lastSiteName": "PixelsCamp"
}
```

- Location of the various access points

![locations](img/access_points_locations.png)


![cmx](img/cmx.png)


### Cisco Spark API resources

- [Spark for Developers](https://developer.ciscospark.com): REST API documentation
- [awesome-ciscospark](https://github.com/CiscoDevNet/awesome-ciscospark)
- ["Create a Conversational Bot" learning lab](https://learninglabs.cisco.com/tracks/collab-cloud/spark-apps/collab-spark-botkit/step/1)

![convos](img/botkit_convos.png)

