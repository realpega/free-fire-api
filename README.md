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
| `key`     | string | Yes      | Join https://t.me/FreeFireInfoSite to get Latest Key.                  |


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
- All images related to item IDs shown by the API response (e.g., avatars, banners, outfits, weapons) are available at `https://www.library.freefireinfo.site/icons/{item_code}.png` for the convenience of API users in their development projects.


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
| `key`     | string | Yes      | Join https://t.me/FreeFireInfoSite to get Latest Key.                  |


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

📚 **Purpose of the API**  

The primary purpose of providing this free API is to enhance the Free Fire community experience. Garena Free Fire does not offer official account information APIs, so this custom solution aims to fill that gap, providing players and developers with valuable account data

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
