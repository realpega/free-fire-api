# 📝 API Documentation

##  Player Information API
API Route = https://free-fire-data.vercel.app/api/data?region={region}&uid={uid}&key={key}

**Endpoint:** `api/data`
**key:** `YOUR-KEY`
**Method:** `GET`  

This Endpoint Retrieves Player Information based on the Specified Region and User ID.

### 📨 Request Example
```http
GET https://free-fire-data.vercel.app/api/data?region=ind&uid=2180732447&key=KEY123
```

### ☑️ Query Parameters

| Parameter | Type   | Required | Description                   |
|-----------|--------|----------|-------------------------------|
| `region`  | string | Yes      | The region code (`sg`, `ind`, `br`,`id`, `tw`, `us`, `sac`, `th`, `me`, `pk`, `cis`, `bd`).|
| `uid`     | int | Yes      | The user ID.                  |
| `key`     | string | Yes      | Buy Key from https://t.me/TrueClasher4                  |


### 💬 Example of a Successful Reponse May Look Like this,
```json
{
  "basicInfo": {
    "accountId": "2180732447",
    "accountPrefers": {
      "brPregameShowChoices": [
        "1"
      ]
    },
    "accountType": "1",
    "badgeId": "1001000082",
    "bannerId": "901000263",
    "createAt": "1594621308",
    "csMaxRank": "201",
    "csRank": "201",
    "exp": "1102643",
    "externalIconInfo": {
      "showType": "ExternalIconShowType_FRIEND",
      "status": "ExternalIconStatus_NOT_IN_USE"
    },
    "headPic": "902040025",
    "lastLoginAt": "1700450083",
    "level": "61",
    "liked": "11182",
    "maxRank": "301",
    "nickname": "SOUNAVA 100K",
    "pinId": "910000004",
    "rank": "301",
    "rankingPoints": "1000",
    "region": "IND",
    "releaseVersion": "OB42",
    "seasonId": "44",
    "title": "904090022",
    "weaponSkinShows": [
      "907102508",
      "912037001"
    ]
  },
  "clanBasicInfo": {

  },
  "creditScoreInfo": {
    "creditScore": "100",
    "rewardState": "RewardState_UNCLAIMED"
  },
  "diamondCostRes": {
    "diamondCost": "390"
  },
  "petInfo": {
    "exp": "6022",
    "id": "1300000112",
    "isSelected": true,
    "level": "7",
    "name": "Bhai",
    "selectedSkillId": "1315000018",
    "skinId": "1310000124"
  },
  "profileInfo": {
    "avatarId": "102000007",
    "clothes": [
      "211000411",
      "211000894",
      "214000023",
      "204033044",
      "205033048",
      "203000981"
    ],
    "equipedSkills": [
      {
        "skillId": "706"
      },
      {
        "skillId": "6501",
        "slotId": "1"
      },
      {
        "skillId": "2906",
        "slotId": "2"
      },
      {
        "skillId": "3406",
        "slotId": "3"
      }
    ],
    "isMarkedStar": true,
    "isSelected": true,
    "isSelectedAwaken": true,
    "skinColor": "50"
  },
  "socialInfo": {
    "accountId": "2180732447",
    "battleTag": [
      "PlayerBattleTagID_MELEE",
      "PlayerBattleTagID_RAMPAGE"
    ],
    "battleTagCount": [
      "172",
      "107"
    ],
    "language": "Language_EN",
    "signature": "GOING OFFLINE FOR 7 DAYS TO UNBAN ID",
    "socialTag": [
      "SocialTag_FASHION",
      "SocialTag_VETERAN"
    ]
  }
}

```

##  Player Stats API
API Route = https://free-fire-data.vercel.app/api/stats?region={region}&uid={uid}&key={key}

**Endpoint:** `api/stats`
**key:** `YOUR-KEY`
**Method:** `GET`  

This Endpoint Retrieves Player Information based on the Specified Region and User ID.

### 📨 Request Example
```http
GET https://free-fire-data.vercel.app/api/stats?region=ind&uid=2180732447&key=KEY123
```

### ☑️ Query Parameters

| Parameter | Type   | Required | Description                   |
|-----------|--------|----------|-------------------------------|
| `region`  | string | Yes      | The region code (`sg`, `ind`, `br`,`id`, `tw`, `us`, `sac`, `th`, `me`, `pk`, `cis`, `bd`).|
| `uid`     | int | Yes      | The user ID.                  |
| `key`     | string | Yes      | Buy Key from https://t.me/TrueClasher4                  |


### 💬 Example of a Successful Reponse May Look Like this,
```json
{
  "success": true,
  "soloStats": {
    "accountId": "10000001",
    "gamesPlayed": 2,
    "kills": 7,
    "detailedStats": {
      "deaths": 2,
      "distanceTravelled": 5309,
      "survivalTime": 587,
      "highestKills": 4,
      "damage": 1764,
      "headshots": 1,
      "headshotKills": 1,
      "pickUps": 146
    }
  },
  "duoStats": {
    "accountId": "10000001",
    "detailedStats": {

    }
  },
  "quadStats": {
    "accountId": "10000001",
    "gamesPlayed": 13,
    "wins": 3,
    "kills": 36,
    "detailedStats": {
      "deaths": 10,
      "topNTimes": 6,
      "distanceTravelled": 60689,
      "survivalTime": 9210,
      "revives": 4,
      "highestKills": 6,
      "damage": 17872,
      "headshots": 16,
      "headshotKills": 5,
      "knockDown": 42,
      "pickUps": 1536
    }
  }
}
```

##  Images API
API Route = https://free-fire-data.vercel.app/api/images?iconName={iconName}&key={key}

**Endpoint:** `api/images`
**key:** `YOUR-KEY`
**Method:** `GET`  

This Endpoint Retrieves Player Information based on the Specified Region and User ID.

### 📨 Request Example
```http
GET https://free-fire-data.vercel.app/api/images?iconName=Icon_avatar_hair_cos_eggday2021_headwear_blue&key=KEY123
```

### ☑️ Query Parameters

| Parameter | Type   | Required | Description                   |
|-----------|--------|----------|-------------------------------|
| `iconName`  | string | Yes      | The name of the Icon. |
| `key`     | string | Yes      | Buy Key from https://t.me/TrueClasher4 


### 💬 Example of a Successful Reponse May Look Like this,

![Icon_avatar_hair_cos_eggday2021_headwear_blue](https://github.com/realpega/free-fire-api/blob/main/images.png)

##  Craftland Map Info API
API Route = https://free-fire-data.vercel.app/api/maps?region={region}&code=%23{CODE}&key={key}

**Endpoint:** `api/maps`
**key:** `YOUR-KEY`
**Method:** `GET`  

This Endpoint Retrieves Player Information based on the Specified Region and User ID.

### 📨 Request Example
```http
GET https://free-fire-data.vercel.app/api/maps?region=sg&code=%23FREEFIREMAPCODE6969&key=KEY123
```

### ☑️ Query Parameters

| Parameter | Type   | Required | Description                   |
|-----------|--------|----------|-------------------------------|
| `region`  | string | Yes      | The region code (`sg`, `ind`, `br`,`id`, `tw`, `us`, `sac`, `th`, `me`, `pk`, `cis`, `bd`).|
| `code`     | String | Yes      | The map code with `%23` prefix.                  |
| `key`     | string | Yes      | Buy Key from https://t.me/TrueClasher4                  |


### 💬 Example of a Successful Reponse May Look Like this,
```json
{
  "status": "success",
  "data": {
    "region": "SG",
    "lang": "en",
    "Craftland Map Details": {
      "MapCode": "#FREEFIREMAPCODE6969",
      "Creator": "SOUNAVA 100K",
      "Title": "Booyah!",
      "Description": "Battle in Style!",
      "MapCover": "https://dl-sg-production.freefiremobile.com/3C124B_7104104913_10007_1726822648_MAPCOVER.JPG",
      "Subscribers": 690000,
      "Likes": 696969,
      "Teams": 2,
      "PlayAverage": 690069
      "Rounds": 1,
      "Tags": [
        "PvP",
        "Squad"
      ],
      "MiniMap": "APD//z8AAMD///8AAAD///8DAAD8//8PAADw//8/AADA////AAAAAfCAAwAAHIABDgAAcAAAOAAAwAEA4AAAAAcAgAMAABweAA4AAHB4ADgAAMDhP5AAAACH/0ACAAAc/sMPAABwAAA4AADAAQDgAAAAHwCAAwAAfAAADgAAcH74OQAAwPnh5wAAAP+HnwMAAPwffg4AAHB++DkAAMD56ecAAADnh/8DAACc3/4PAABwgAc4AADAAQzgAAAABzDgAwAAHACADwAAcAAAOAAAwAEA4AAAAD/8hwMAACTwHw4AAJDAfzgAAMAB4OEAAAAHgIcDAAAcAAAOAABwAAA4AADAAQDgAAAAB2CAAwAAHMADCAAA8P//PwAAwP///wAAAP///wMAAPz//w8AAPD//z8AAMD///8AAA==",
      "Mode": "Customize",
      "Map": "Bermuda"
    }
  }
}
```

##  Player Wishlist API
API Route = https://free-fire-data.vercel.app/api/wishlist?region={region}&uid={uid}&key={key}

**Endpoint:** `api/wishlist`
**key:** `YOUR-KEY`
**Method:** `GET`  

This Endpoint Retrieves Player Information based on the Specified Region and User ID.

### 📨 Request Example
```http
GET https://free-fire-data.vercel.app/api/wishlist?region=ind&uid=2180732447&key=KEY123
```

### ☑️ Query Parameters

| Parameter | Type   | Required | Description                   |
|-----------|--------|----------|-------------------------------|
| `region`  | string | Yes      | The region code (`sg`, `ind`, `br`,`id`, `tw`, `us`, `sac`, `th`, `me`, `pk`, `cis`, `bd`).|
| `uid`     | int | Yes      | The user ID.                  |
| `key`     | string | Yes      | Buy Key from https://t.me/TrueClasher4                  |


### 💬 Example of a Successful Reponse May Look Like this,

```json
{
  "items": [
    {
      "itemId": 102000035,
      "releaseTime": 1709233149
    },
    {
      "itemId": 203000036,
      "releaseTime": 1710238335
    },
    {
      "itemId": 203000981,
      "releaseTime": 1706079412
    },
    {
      "itemId": 204033044,
      "releaseTime": 1706079412
    },
    {
      "itemId": 205033048,
      "releaseTime": 1706079412
    },
    {
      "itemId": 211000411,
      "releaseTime": 1706079412
    },
    {
      "itemId": 211000894,
      "releaseTime": 1706079412
    },
    {
      "itemId": 214000023,
      "releaseTime": 1706079412
    },
    {
      "itemId": 901040034,
      "releaseTime": 1727692721
    },
    {
      "itemId": 902000003,
      "releaseTime": 1710238335
    },
    {
      "itemId": 902040026,
      "releaseTime": 1710238335
    },
    {
      "itemId": 902040029,
      "releaseTime": 1710238335
    },
    {
      "itemId": 902040030,
      "releaseTime": 1710238335
    },
    {
      "itemId": 903040007,
      "releaseTime": 1727692721
    },
    {
      "itemId": 903043010,
      "releaseTime": 1710238335
    },
    {
      "itemId": 904040010,
      "releaseTime": 1727692721
    },
    {
      "itemId": 904090027,
      "releaseTime": 1707398570
    },
    {
      "itemId": 905039004,
      "releaseTime": 1710238335
    },
    {
      "itemId": 906036010,
      "releaseTime": 1706524016
    },
    {
      "itemId": 907102508,
      "releaseTime": 1706079412
    },
    {
      "itemId": 907104073,
      "releaseTime": 1727692721
    },
    {
      "itemId": 907104074,
      "releaseTime": 1727692721
    },
    {
      "itemId": 907104075,
      "releaseTime": 1727692721
    },
    {
      "itemId": 907104076,
      "releaseTime": 1727692721
    },
    {
      "itemId": 907104077,
      "releaseTime": 1727692721
    },
    {
      "itemId": 909040014,
      "releaseTime": 1727692721
    },
    {
      "itemId": 909043013,
      "releaseTime": 1707543814
    },
    {
      "itemId": 911004301,
      "releaseTime": 1710238335
    },
    {
      "itemId": 912037001,
      "releaseTime": 1706079412
    },
    {
      "itemId": 921047018,
      "releaseTime": 1735657844
    }
  ]
}
```

📚 **Purpose of the API**  

The primary purpose of providing this free API is to enhance the Free Fire community experience. Garena Free Fire does not offer official account information APIs, so this custom solution aims to fill that gap, providing players and developers with valuable account data

🧩 **(Some of🤫) Frameworks and Libraries Used**  
- **Flask**: A micro web framework for Python to build the API endpoints.
- **Flask-CORS**: For handling Cross-Origin Resource Sharing (CORS).
- **PyCryptodome**: For implementing Decryption and Encryption.
- **Requests**: For making HTTP Requests to Server.

# 📁 Additional Information

- This API response Does not Represent the Actual Structure Received from the Official Garena Server.
- The Response structure is simplified in an User-Friendly Structure for the ease of understanding for Anyone at any level of Programming.

# 😵 Error Responses
API might Show Error Response Upon Users' Inaccurate Requests!

### Error Instances and Solutions

- **Error Code:** 400
  - **Message:** Invalid region.
  - **Solution:** Make sure you are using a valid region code.

- **Error Code:** 429
  - **Message:** Abnormal Requests Detected. Please Avoid Misusing Info API for Visits or Your IP may get Blocked!
  - **Solution:** Avoid excessive requests or contact the API provider for assistance.

- **Error Code:** 500
  - **Message:** An error occurred while processing your request. Please Recheck Your ID & Region.
  - **Solution:** Double-check the provided user ID and region, and retry the request. If the issue persists, contact the API provider for support.

---

API Made By Sounava777,
All Rights Reserved!
