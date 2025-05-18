# 📝 وثائق واجهة برمجة التطبيقات

## واجهة برمجة معلومات اللاعب
مسار واجهة برمجة التطبيقات = https://free-fire-data.vercel.app/api/data?region={region}&uid={uid}&key={key}

**النقطة النهائية:** `api/data`  
**المفتاح:** `مفتاحك`  
**الطريقة:** `GET`  

تسترد هذه النقطة النهائية معلومات اللاعب بناءً على المنطقة ومعرف المستخدم المحددين.

### 📨 مثال على الطلب
```http
GET https://free-fire-data.vercel.app/api/data?region=ind&uid=2180732447&key=KEY123
```

### ☑️ معلمات الاستعلام

| المعلمة   | النوع   | مطلوب | الوصف                                |
|-----------|---------|-------|--------------------------------------|
| `region`  | سلسلة  | نعم   | رمز المنطقة (`sg`, `ind`, `br`)      |
| `uid`     | عدد صحيح | نعم   | معرف المستخدم                       |
| `key`     | سلسلة  | نعم   | اشترِ المفتاح من https://t.me/TrueClasher4 |

### ℹ️ ملاحظة هامة

معلمة الاستعلام `SG` مخصصة لجميع المناطق التي تندرج تحت `clientbp.ggblueshark.com`  
[`SG`, `ID`, `ME`, `VN`, `TH`, `CIS`, `EU`, `TW`, `MY`, `PK`, `BD`]

معلمة الاستعلام `IND` مخصصة للهند فقط وتندرج تحت `client.ind.freefiremobile.com`  
[`IND`]

معلمة الاستعلام `BR` مخصصة لجميع المناطق التي تندرج تحت `client.us.freefiremobile.com`  
[`BR`, `US`, `NA`, `LATAM`]

### 💬 مثال على استجابة ناجحة قد يبدو كالتالي,
```json
{
  "basicInfo": {
    "accountId": 2129250963,
    "accountType": 1,
    "bannerId": 901026021,
    "bpStatus": null,
    "brMaxRank": 316,
    "brRank": 2768,
    "createAt": 1747304828,
    "csMaxRank": 316,
    "csRank": 45,
    "exp": 133627,
    "headPic": 902000057,
    "lastLoginAt": 1593158767,
    "level": 42,
    "liked": 4957,
    "nickname": "SOUNAVA 500K",
    "region": "IND",
    "releaseVersion": "OB48",
    "showBrRank": true,
    "showCsRank": true,
    "title": 904090024
  },
  "captainBasicInfo": {
    "accountId": 2129250963,
    "accountType": 1,
    "badgeCnt": 42,
    "bannerId": 901026021,
    "brMaxRank": 316,
    "brRank": 316,
    "brRankingPoints": 2768,
    "createAt": 1593158767,
    "csMaxRank": 305,
    "csRank": 305,
    "csRankingPoints": 17,
    "exp": 133627,
    "headPic": 902000057,
    "lastLoginAt": 1747304828,
    "level": 42,
    "liked": 4957,
    "nickname": "SOUNAVA 500K",
    "region": "IND",
    "releaseVersion": "OB48",
    "seasonId": 45
  },
  "clanBasicInfo": [
    {
      "capacity": 25,
      "captainId": 2129250963,
      "clanId": 3000167557,
      "clanLevel": 1,
      "clanName": "〆ᗷᖇᝪᎢᕼᗴᖇ",
      "memberNum": 5
    }
  ],
  "creditScoreInfo": {
    "creditScore": 100,
    "periodicSummaryEndTime": 1747564036,
    "periodicSummaryStartTime": 1747304836,
    "rewardState": 2
  },
  "petInfo": {
    "exp": 548,
    "id": 1300000120,
    "level": 4,
    "nickname": null,
    "selectedSkillId": 1310000201,
    "skinId": 1315000010
  },
  "socialInfo": {
    "accountId": 2129250963,
    "brRankShow": 1,
    "csRankShow": null,
    "signature": "Sounava777 Never Dies."
  }
}
```

## واجهة برمجة إحصائيات اللاعب
مسار واجهة برمجة التطبيقات = https://free-fire-data.vercel.app/api/stats?region={region}&uid={uid}&key={key}

**النقطة النهائية:** `api/stats`  
**المفتاح:** `مفتاحك`  
**الطريقة:** `GET`  

تسترد هذه النقطة النهائية معلومات إحصائيات اللاعب بناءً على المنطقة ومعرف المستخدم المحددين.

### 📨 مثال على الطلب
```http
GET https://free-fire-data.vercel.app/api/stats?region=ind&uid=2180732447&key=KEY123
```

### ☑️ معلمات الاستعلام

| المعلمة   | النوع   | مطلوب | الوصف                                |
|-----------|---------|-------|--------------------------------------|
| `region`  | سلسلة  | نعم   | رمز المنطقة (`sg`, `ind`, `br`)      |
| `uid`     | عدد صحيح | نعم   | معرف المستخدم                       |
| `key`     | سلسلة  | نعم   | اشترِ المفتاح من https://t.me/TrueClasher4 |

### ℹ️ ملاحظة هامة

معلمة الاستعلام `SG` مخصصة لجميع المناطق التي تندرج تحت `clientbp.ggblueshark.com`  
[`SG`, `ID`, `ME`, `VN`, `TH`, `CIS`, `EU`, `TW`, `MY`, `PK`, `BD`]

معلمة الاستعلام `IND` مخصصة للهند فقط وتندرج تحت `client.ind.freefiremobile.com`  
[`IND`]

معلمة الاستعلام `BR` مخصصة لجميع المناطق التي تندرج تحت `client.us.freefiremobile.com`  
[`BR`, `US`, `NA`, `LATAM`]

### 💬 مثال على استجابة ناجحة قد يبدو كالتالي,
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

## واجهة برمجة الإعجابات
مسار واجهة برمجة التطبيقات = https://free-fire-data.vercel.app/api/like?region={region}&uid={uid}&key={key}

**النقطة النهائية:** `api/like`  
**المفتاح:** `مفتاحك`  
**الطريقة:** `GET`  

ترسل هذه النقطة النهائية 100 إعجاب إلى حساب اللاعب بناءً على المنطقة ومعرف المستخدم المحددين.

### 📨 مثال على الطلب
```http
GET https://free-fire-data.vercel.app/api/like?region=ind&uid=2180732447&key=KEY123
```

### ☑️ معلمات الاستعلام

| المعلمة   | النوع   | مطلوب | الوصف                                |
|-----------|---------|-------|--------------------------------------|
| `region`  | سلسلة  | نعم   | رمز المنطقة (`sg`, `ind`, `br`)      |
| `uid`     | عدد صحيح | نعم   | معرف المستخدم                       |
| `key`     | سلسلة  | نعم   | اشترِ المفتاح من https://t.me/TrueClasher4 |

### ℹ️ ملاحظة هامة

معلمة الاستعلام `SG` مخصصة لجميع المناطق التي تندرج تحت `clientbp.ggblueshark.com`  
[`SG`, `ID`, `ME`, `VN`, `TH`, `CIS`, `EU`, `TW`, `MY`, `PK`, `BD`]

معلمة الاستعلام `IND` مخصصة للهند فقط وتندرج تحت `client.ind.freefiremobile.com`  
[`IND`]

معلمة الاستعلام `BR` مخصصة لجميع المناطق التي تندرج تحت `client.us.freefiremobile.com`  
[`BR`, `US`, `NA`, `LATAM`]

### 💬 مثال على استجابة ناجحة قد يبدو كالتالي,
```json
{
  "response": {
    "KeyExpiresAt": "2025-03-20T90:30:00.696969",
    "KeyRemainingRequests": "69/100",
    "LikesGivenByAPI": 100,
    "LikesafterCommand": 6969,
    "LikesbeforeCommand": 6869,
    "PlayerLevel": 69,
    "PlayerNickname": "SOUNAVA 500K",
    "UID": "2129250963"
  },
  "status": 1
}
```

## واجهة برمجة الزيارات
مسار واجهة برمجة التطبيقات = https://free-fire-data.vercel.app/api/visit?region={region}&uid={uid}&key={key}

**النقطة النهائية:** `api/visit`  
**المفتاح:** `مفتاحك`  
**الطريقة:** `GET`  

ترسل هذه النقطة النهائية 100 زيارة إلى حساب اللاعب بناءً على المنطقة ومعرف المستخدم المحددين.

### 📨 مثال على الطلب
```http
GET https://free-fire-data.vercel.app/api/visit?region=ind&uid=2180732447&key=KEY123
```

### ☑️ معلمات الاستعلام

| المعلمة   | النوع   | مطلوب | الوصف                                |
|-----------|---------|-------|--------------------------------------|
| `region`  | سلسلة  | نعم   | رمز المنطقة (`sg`, `ind`, `br`)      |
| `uid`     | عدد صحيح | نعم   | معرف المستخدم                       |
| `key`     | سلسلة  | نعم   | اشترِ المفتاح من https://t.me/TrueClasher4 |

### ℹ️ ملاحظة هامة

معلمة الاستعلام `SG` مخصصة لجميع المناطق التي تندرج تحت `clientbp.ggblueshark.com`  
[`SG`, `ID`, `ME`, `VN`, `TH`, `CIS`, `EU`, `TW`, `MY`, `PK`, `BD`]

معلمة الاستعلام `IND` مخصصة للهند فقط وتندرج تحت `client.ind.freefiremobile.com`  
[`IND`]

معلمة الاستعلام `BR` مخصصة لجميع المناطق التي تندرج تحت `client.us.freefiremobile.com`  
[`BR`, `US`, `NA`, `LATAM`]

### 💬 مثال على استجابة ناجحة قد يبدو كالتالي,
```json
{
  "response": {
    "KeyExpiresAt": "2025-03-20T90:30:00.696969",
    "KeyRemainingRequests": "69/100",
    "VisitsSentByAPI": 100,
    "PlayerLevel": 69,
    "PlayerNickname": "SOUNAVA 500K",
    "UID": "2129250963"
  },
  "status": 1
}
```

## واجهة برمجة الرسائل غير المرغوبة
مسار واجهة برمجة التطبيقات = https://free-fire-data.vercel.app/api/spam?region={region}&uid={uid}&key={key}

**النقطة النهائية:** `api/spam`  
**المفتاح:** `مفتاحك`  
**الطريقة:** `GET`  

ترسل هذه النقطة النهائية 100 طلب صداقة إلى حساب اللاعب بناءً على المنطقة ومعرف المستخدم المحددين.

### 📨 مثال على الطلب
```http
GET https://free-fire-data.vercel.app/api/spam?region=ind&uid=2180732447&key=KEY123
```

### ☑️ معلمات الاستعلام

| المعلمة   | النوع   | مطلوب | الوصف                                |
|-----------|---------|-------|--------------------------------------|
| `region`  | سلسلة  | نعم   | رمز المنطقة (`sg`, `ind`, `br`)      |
| `uid`     | عدد صحيح | نعم   | معرف المستخدم                       |
| `key`     | سلسلة  | نعم   | اشترِ المفتاح من https://t.me/TrueClasher4 |

### ℹ️ ملاحظة هامة

معلمة الاستعلام `SG` مخصصة لجميع المناطق التي تندرج تحت `clientbp.ggblueshark.com`  
[`SG`, `ID`, `ME`, `VN`, `TH`, `CIS`, `EU`, `TW`, `MY`, `PK`, `BD`]

معلمة الاستعلام `IND` مخصصة للهند فقط وتندرج تحت `client.ind.freefiremobile.com`  
[`IND`]

معلمة الاستعلام `BR` مخصصة لجميع المناطق التي تندرج تحت `client.us.freefiremobile.com`  
[`BR`, `US`, `NA`, `LATAM`]

### 💬 مثال على استجابة ناجحة قد يبدو كالتالي,
```json
{
  "response": {
    "KeyExpiresAt": "2025-03-20T90:30:00.696969",
    "KeyRemainingRequests": "69/100",
    "FriendRequestsSentByAPI": 100,
    "isPlayerOnline": true,
    "PlayerLevel": 69,
    "PlayerNickname": "SOUNAVA 500K",
    "UID": "2129250963"
  },
  "status": 1
}
```

## واجهة برمجة الصور
مسار واجهة برمجة التطبيقات = https://free-fire-data.vercel.app/api/images?iconName={iconName}&key={key}

**النقطة النهائية:** `api/images`  
**المفتاح:** `مفتاحك`  
**الطريقة:** `GET`  

تسترد هذه النقطة النهائية معلومات اللاعب بناءً على المنطقة ومعرف المستخدم المحددين.

### 📨 مثال على الطلب
```http
GET https://free-fire-data.vercel.app/api/images?iconName=Icon_avatar_hair_cos_eggday2021_headwear_blue&key=KEY123
```

### ☑️ معلمات الاستعلام

| المعلمة    | النوع   | مطلوب | الوصف                                |
|------------|---------|-------|--------------------------------------|
| `iconName` | سلسلة  | نعم   | اسم الأيقونة.                       |
| `key`      | سلسلة  | نعم   | اشترِ المفتاح من https://t.me/TrueClasher4 |

### 💬 مثال على استجابة ناجحة قد يبدو كالتالي,

![Icon_avatar_hair_cos_eggday2021_headwear_blue](https://github.com/realpega/free-fire-api/blob/main/images.png)

## واجهة برمجة معلومات خرائط Craftland
مسار واجهة برمجة التطبيقات = https://free-fire-data.vercel.app/api/maps?region={region}&code=%23{CODE}&key={key}

**النقطة النهائية:** `api/maps`  
**المفتاح:** `مفتاحك`  
**الطريقة:** `GET`  

تسترد هذه النقطة النهائية معلومات اللاعب بناءً على المنطقة ومعرف المستخدم المحددين.

### 📨 مثال على الطلب
```http
GET https://free-fire-data.vercel.app/api/maps?region=sg&code=%23FREEFIREMAPCODE6969&key=KEY123
```

### ☑️ معلمات الاستعلام

| المعلمة   | النوع   | مطلوب | الوصف                                |
|-----------|---------|-------|--------------------------------------|
| `region`  | سلسلة  | نعم   | رمز المنطقة (`sg`, `ind`, `br`)      |
| `uid`     | عدد صحيح | نعم   | معرف المستخدم                       |
| `key`     | سلسلة  | نعم   | اشترِ المفتاح من https://t.me/TrueClasher4 |

### ℹ️ ملاحظة هامة

معلمة الاستعلام `SG` مخصصة لجميع المناطق التي تندرج تحت `clientbp.ggblueshark.com`  
[`SG`, `ID`, `ME`, `VN`, `TH`, `CIS`, `EU`, `TW`, `MY`, `PK`, `BD`]

معلمة الاستعلام `IND` مخصصة للهند فقط وتندرج تحت `client.ind.freefiremobile.com`  
[`IND`]

معلمة الاستعلام `BR` مخصصة لجميع المناطق التي تندرج تحت `client.us.freefiremobile.com`  
[`BR`, `US`, `NA`, `LATAM`]

### 💬 مثال على استجابة ناجحة قد يبدو كالتالي,
```json
{
  "code": 0,
  "status": "success",
  "msg": "",
  "data": {
    "region_lang": "SG_en",
    "start_time": 1,
    "end_time": 1890713325,
    "rule": "Garena Free Fire",
    "region": "SG",
    "lang": "en",
    "title": "Garena Free Fire",
    "android_download_url": "https://play.google.com/store/apps/details?id=com.dts.freefireth&referrer=af_tranid%3DgTVeQgRDoYWAmOvmEZz6Xw%26pid%3DOrganicA%26c%3Dmainpage_AND%26af_web_id%3Da209618f-0ae1-4239-bed0-46bcfb0c9656-c",
    "ios_download_url": "https://apps.apple.com/US/app/id1300146617?mt=8",
    "ugc_url": "https://createofficial.garena.com/",
    "imgs": [
      "https://dl.dir.freefiremobile.com/common/OB46/CSH/Devs/WebCDN/BACKGROUND01.png",
      "https://dl.dir.freefiremobile.com/common/OB46/CSH/Devs/WebCDN/BACKGROUND02.png",
      "https://dl.dir.freefiremobile.com/common/OB46/CSH/Devs/WebCDN/BACKGROUND03.png",
      "https://dl.dir.freefiremobile.com/common/OB46/CSH/Devs/WebCDN/BACKGROUND04.png",
      "https://dl.dir.freefiremobile.com/common/OB46/CSH/Devs/WebCDN/BACKGROUND05.png"
    ],
    "game_icon": "https://dl.dir.freefiremobile.com/common/OB45/CSH/abcdfallstorebanners/appicon/FF_AndroidIcon_512.png",
    "game_name": "Free Fire: 7th Anniversary!",
    "transify": {
      "COMMON_ACCEPT": "قبول",
      "COMMON_BACK": "رجوع",
      "COMMON_CANCEL": "إلغاء",
      "COMMON_CONFIRM": "تأكيد",
      "COMMON_CONTINUE_PURCHASE": "متابعة الشراء",
      "COMMON_COPY": "نسخ",
      "COMMON_COPY_FAILED": "فشل النسخ",
      "COMMON_COPY_SUCCESS": "تم النسخ بنجاح",
      "COMMON_EXCHANGE": "استبدال",
      "COMMON_EXCHANGED": "تم الاستبدال",
      "COMMON_FFTOKEN_HINT": "تم تحويله إلى {num}{أيقونة رمز FF}",
      "COMMON_FREE": "مجاني",
      "COMMON_GEM_CONFIRM": "إنفاق {cost} جوهرة (جواهر) لشراء {NAME}؟",
      "COMMON_GEM_CONFIRM2": "إنفاق {cost} جواهر لـ {num} دوران (دورات)؟",
      "COMMON_HISTORY_DRAW": "السجل",
      "COMMON_HISTORY_NORECORDS": "لا توجد سجلات",
      "COMMON_HISTORY_PURCHASE": "سجل الشراء",
      "COMMON_HISTORY_REDEEM": "سجل الاستبدال",
      "COMMON_NO": "لا",
      "COMMON_OWNED": "مملوك",
      "COMMON_PRIZEPOOL": "مجموعة المكافآت",
      "COMMON_PURCHASE": "شراء",
      "COMMON_PURCHASED": "تم الشراء",
      "COMMON_QUANTITY_MAX": "الحد الأقصى",
      "COMMON_REDEEM_CONFIRM": "هل أنت متأكد من استبدال هذا العنصر؟",
      "COMMON_REJECT": "رفض",
      "COMMON_RULE": "القواعد",
      "COMMON_SKIP": "تخطي الرسوم المتحركة",
      "COMMON_SKIPANIMATION_TIP": "اضغط في أي مكان لتخطي الرسوم المتحركة",
      "COMMON_SPIN_AGAIN": "دوران مرة أخرى",
      "COMMON_TIPS_ITEM": "سيتم إرسال المكافآت مباشرة إلى خزنتك",
      "COMMON_TIPS_TOKEN": "تم تجميع الرموز تلقائيًا",
      "COMMON_VISIT_GIFT": "هدية ترحيبية",
      "COMMON_YES": "نعم",
      "POPUP_NO_REMIND": "لا تذكرني مرة أخرى",
      "POPUP_TITLE_CONGRATULATIONS": "تهانينا!",
      "POPUP_TITLE_REDEEM": "تهانينا! لقد حصلت على",
      "POPUP_TITLE_UNIQUE": "العناصر الفريدة التي تمتلكها",
      "UNIQUE_BUY_ALREADY_HAVE": "أنت تمتلك هذا العنصر بالفعل، إذا اشتريته مرة أخرى، سيتم تحويله إلى رموز FF",
      "UNIQUE_BUY_ALREADY_HAVE_PART": "أنت تمتلك بعض العناصر التي اخترتها بالفعل. إذا تلقيتها مرة أخرى، سيتم تحويلها إلى رموز FF.",
      "UNIQUE_REDEEM_ALREADY_HAVE": "أنت تمتلك هذا العنصر بالفعل، إذا تلقيته مرة أخرى، سيتم تحويله إلى رموز FF.",
      "TOAST_ERROR_CODE": "خطأ غير معروف، رمز الخطأ {code}",
      "TOAST_EVENTOVER": "انتهى الحدث",
      "TOAST_EVENT_CLOSED_AWHILE": "الحدث مغلق مؤقتًا. يرجى التحقق مرة أخرى لاحقًا.",
      "TOAST_EVENT_END": "انتهى الحدث",
      "TOAST_EVENT_NOTOPEN": "لم يبدأ الحدث بعد",
      "TOAST_EXCHANGE_SUCCESS": "تم الاستبدال بنجاح",
      "TOAST_GEM_NOT_ENOUGH": "الألماس غير كافٍ، يرجى الشحن والعودة مرة أخرى",
      "TOAST_LOGIN_FAILED": "فشل تسجيل الدخول",
      "TOAST_NETWORK_BUSY": "الخادم مشغول، يرجى المحاولة مرة أخرى لاحقًا",
      "TOAST_NETWORK_ERROR": "خطأ في الاتصال بالشبكة، يرجى المحاولة مرة أخرى لاحقًا",
      "TOAST_OPERATE_BUSY": "طلبات كثيرة جدًا، يرجى المحاولة مرة أخرى لاحقًا",
      "TOAST_PAY_FAILED": "فشل الشراء",
      "TOAST_PURCHASE_SUCCESS": "الشراء ناجح",
      "TOAST_SERVER_BUSY": "الخادم مشغول، يرجى المحاولة مرة أخرى لاحقًا",
      "TOAST_SERVER_NOTWORK": "الخدمة غير متوفرة",
      "TOAST_SERVER_TIMEOUT": "انتهت مهلة الخدمة",
      "TOAST_WRONG_REGION": "هذا الحدث غير متوفر لمنطقتك",
      "COMMON_CALLBACK": "انضم إلى المعركة!",
      "COMMON_JOIN": "انضم",
      "COMMON_SHOOT": "اضغط على الأهداف",
      "COMMON_SHOOT_2": "عمل جيد! للمتابعة، يرجى التوجه إلى Free Fire!",
      "UGC_46_MAPSHARE_GOBUTTON": "استكشف المزيد",
      "UGC_46_MAPSHARE_PLAYBUTTON": "العب الآن",
      "UGC_46_MAPSHARE_WRONGMESSAGE": "عذرًا، هذه الخريطة غير متوفرة في الوقت الحالي.",
      "UGC_47_MAPSHARE_MAPCODE": "رمز الخريطة",
      "UGC_47_MAPSHARE_NAME": "اسم المبدع",
      "UGC_47_MAPSHARE_TOAST1": "تم النسخ بنجاح",
      "UGC_47_MAPSHARE_TOAST2": "فشل النسخ"
    },
    "share_img": "https://dl.dir.freefiremobile.com/common/OB46/CSH/Devs/WebCDN/SOFTFF.jpg",
    "desc_prefix": "[Free Fire]{desc}",
    "source_params": {
      "region": "",
      "lang": "en",
      "version": "",
      "action": "",
      "map_code": ""
    }
  }
}
```

## واجهة برمجة قائمة رغبات اللاعب
مسار واجهة برمجة التطبيقات = https://free-fire-data.vercel.app/api/wishlist?region={region}&uid={uid}&key={key}

**النقطة النهائية:** `api/wishlist`  
**المفتاح:** `مفتاحك`  
**الطريقة:** `GET`  

تسترد هذه النقطة النهائية معلومات اللاعب بناءً على المنطقة ومعرف المستخدم المحددين.

### 📨 مثال على الطلب
```http
GET https://free-fire-data.vercel.app/api/wishlist?region=ind&uid=2180732447&key=KEY123
```

### ☑️ معلمات الاستعلام

| المعلمة   | النوع   | مطلوب | الوصف                                |
|-----------|---------|-------|--------------------------------------|
| `region`  | سلسلة  | نعم   | رمز المنطقة (`sg`, `ind`, `br`)      |
| `uid`     | عدد صحيح | نعم   | معرف المستخدم                       |
| `key`     | سلسلة  | نعم   | اشترِ المفتاح من https://t.me/TrueClasher4 |

### ℹ️ ملاحظة هامة

معلمة الاستعلام `SG` مخصصة لجميع المناطق التي تندرج تحت `clientbp.ggblueshark.com`  
[`SG`, `ID`, `ME`, `VN`, `TH`, `CIS`, `EU`, `TW`, `MY`, `PK`, `BD`]

معلمة الاستعلام `IND` مخصصة للهند فقط وتندرج تحت `client.ind.freefiremobile.com`  
[`IND`]

معلمة الاستعلام `BR` مخصصة لجميع المناطق التي تندرج تحت `client.us.freefiremobile.com`  
[`BR`, `US`, `NA`, `LATAM`]

### 💬 مثال على استجابة ناجحة قد يبدو كالتالي,
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

📚 **غرض واجهة برمجة التطبيقات**

الهدف الأساسي من توفير هذه الواجهة البرمجية المجانية هو تعزيز تجربة مجتمع Free Fire. لا تقدم Garena Free Fire واجهات برمجة رسمية لمعلومات الحسابات، لذا تهدف هذه الحلول المخصصة إلى سد هذه الفجوة، وتوفير بيانات قيمة عن الحسابات للاعبين والمطورين.

🧩 **(بعض من🤫) الأطر والمكتبات المستخدمة**  
- **Flask**: إطار ويب صغير لـ Python لبناء نقاط نهاية واجهة برمجة التطبيقات.  
- **Flask-CORS**: للتعامل مع مشاركة الموارد عبر النطاقات (CORS).  
- **PyCryptodome**: لتنفيذ فك التشفير والتشفير.  
- **Requests**: لإجراء طلبات HTTP إلى الخادم.

# 📁 معلومات إضافية

- استجابة واجهة برمجة التطبيقات هذه لا تمثل الهيكلية الفعلية المستلمة من خادم Garena الرسمي.  
- تم تبسيط هيكلية الاستجابة في هيكلية سهلة الاستخدام لتسهيل الفهم لأي شخص على أي مستوى من البرمجة.

# 😵 استجابات الأخطاء
قد تظهر واجهة برمجة التطبيقات استجابة خطأ عند طلبات المستخدمين غير الدقيقة!

### أمثلة على الأخطاء وحلولها

- **رمز الخطأ:** 400
  - **الرسالة:** منطقة غير صالحة.  
  - **الحل:** تأكد من استخدام رمز منطقة صالح.

- **رمز الخطأ:** 429
  - **الرسالة:** تم اكتشاف طلبات غير طبيعية. يرجى تجنب إساءة استخدام واجهة برمجة المعلومات للزيارات وإلا قد يتم حظر عنوان IP الخاص بك!  
  - **الحل:** تجنب الطلبات المفرطة أو اتصل بمزود واجهة برمجة التطبيقات للحصول على المساعدة.

- **رمز الخطأ:** 500
  - **الرسالة:** حدث خطأ أثناء معالجة طلبك. يرجى إعادة التحقق من معرفك والمنطقة.  
  - **الحل:** تحقق مرة أخرى من معرف المستخدم والمنطقة المقدمين وحاول مرة أخرى. إذا استمرت المشكلة، اتصل بمزود واجهة برمجة التطبيقات للحصول على الدعم.

---

واجهة برمجة التطبيقات من إنشاء Sounava777،  
جميع الحقوق محفوظة!
