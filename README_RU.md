# 📝 Документация API

## API информации об игроке
Маршрут API = https://free-fire-data.vercel.app/api/data?region={region}&uid={uid}&key={key}

**Конечная точка:** `api/data`  
**Ключ:** `ВАШ-КЛЮЧ`  
**Метод:** `GET`  

Эта конечная точка получает информацию об игроке на основе указанного региона и идентификатора пользователя.

### 📨 Пример запроса
```http
GET https://free-fire-data.vercel.app/api/data?region=ind&uid=2180732447&key=KEY123
```

### ☑️ Параметры запроса

| Параметр  | Тип    | Обязательный | Описание                              |
|-----------|--------|--------------|---------------------------------------|
| `region`  | строка | Да           | Код региона (`sg`, `ind`, `br`)       |
| `uid`     | целое  | Да           | Идентификатор пользователя            |
| `key`     | строка | Да           | Купить ключ на https://t.me/TrueClasher4 |

### ℹ️ Важное замечание

Параметр запроса `SG` предназначен для всех регионов, подпадающих под `clientbp.ggblueshark.com`  
[`SG`, `ID`, `ME`, `VN`, `TH`, `CIS`, `EU`, `TW`, `MY`, `PK`, `BD`]

Параметр запроса `IND` предназначен только для Индии и подпадает под `client.ind.freefiremobile.com`  
[`IND`]

Параметр запроса `BR` предназначен для всех регионов, подпадающих под `client.us.freefiremobile.com`  
[`BR`, `US`, `NA`, `LATAM`]

### 💬 Пример успешного ответа может выглядеть так,
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

## API статистики игрока
Маршрут API = https://free-fire-data.vercel.app/api/stats?region={region}&uid={uid}&key={key}

**Конечная точка:** `api/stats`  
**Ключ:** `ВАШ-КЛЮЧ`  
**Метод:** `GET`  

Эта конечная точка получает информацию о статистике игрока на основе указанного региона и идентификатора пользователя.

### 📨 Пример запроса
```http
GET https://free-fire-data.vercel.app/api/stats?region=ind&uid=2180732447&key=KEY123
```

### ☑️ Параметры запроса

| Параметр  | Тип    | Обязательный | Описание                              |
|-----------|--------|--------------|---------------------------------------|
| `region`  | строка | Да           | Код региона (`sg`, `ind`, `br`)       |
| `uid`     | целое  | Да           | Идентификатор пользователя            |
| `key`     | строка | Да           | Купить ключ на https://t.me/TrueClasher4 |

### ℹ️ Важное замечание

Параметр запроса `SG` предназначен для всех регионов, подпадающих под `clientbp.ggblueshark.com`  
[`SG`, `ID`, `ME`, `VN`, `TH`, `CIS`, `EU`, `TW`, `MY`, `PK`, `BD`]

Параметр запроса `IND` предназначен только для Индии и подпадает под `client.ind.freefiremobile.com`  
[`IND`]

Параметр запроса `BR` предназначен для всех регионов, подпадающих под `client.us.freefiremobile.com`  
[`BR`, `US`, `NA`, `LATAM`]

### 💬 Пример успешного ответа может выглядеть так,
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

## API лайков
Маршрут API = https://free-fire-data.vercel.app/api/like?region={region}&uid={uid}&key={key}

**Конечная точка:** `api/like`  
**Ключ:** `ВАШ-КЛЮЧ`  
**Метод:** `GET`  

Эта конечная точка отправляет 100 лайков на аккаунт игрока на основе указанного региона и идентификатора пользователя.

### 📨 Пример запроса
```http
GET https://free-fire-data.vercel.app/api/like?region=ind&uid=2180732447&key=KEY123
```

### ☑️ Параметры запроса

| Параметр  | Тип    | Обязательный | Описание                              |
|-----------|--------|--------------|---------------------------------------|
| `region`  | строка | Да           | Код региона (`sg`, `ind`, `br`)       |
| `uid`     | целое  | Да           | Идентификатор пользователя            |
| `key`     | строка | Да           | Купить ключ на https://t.me/TrueClasher4 |

### ℹ️ Важное замечание

Параметр запроса `SG` предназначен для всех регионов, подпадающих под `clientbp.ggblueshark.com`  
[`SG`, `ID`, `ME`, `VN`, `TH`, `CIS`, `EU`, `TW`, `MY`, `PK`, `BD`]

Параметр запроса `IND` предназначен только для Индии и подпадает под `client.ind.freefiremobile.com`  
[`IND`]

Параметр запроса `BR` предназначен для всех регионов, подпадающих под `client.us.freefiremobile.com`  
[`BR`, `US`, `NA`, `LATAM`]

### 💬 Пример успешного ответа может выглядеть так,
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

## API посещений
Маршрут API = https://free-fire-data.vercel.app/api/visit?region={region}&uid={uid}&key={key}

**Конечная точка:** `api/visit`  
**Ключ:** `ВАШ-КЛЮЧ`  
**Метод:** `GET`  

Эта конечная точка отправляет 100 посещений на аккаунт игрока на основе указанного региона и идентификатора пользователя.

### 📨 Пример запроса
```http
GET https://free-fire-data.vercel.app/api/visit?region=ind&uid=2180732447&key=KEY123
```

### ☑️ Параметры запроса

| Параметр  | Тип    | Обязательный | Описание                              |
|-----------|--------|--------------|---------------------------------------|
| `region`  | строка | Да           | Код региона (`sg`, `ind`, `br`)       |
| `uid`     | целое  | Да           | Идентификатор пользователя            |
| `key`     | строка | Да           | Купить ключ на https://t.me/TrueClasher4 |

### ℹ️ Важное замечание

Параметр запроса `SG` предназначен для всех регионов, подпадающих под `clientbp.ggblueshark.com`  
[`SG`, `ID`, `ME`, `VN`, `TH`, `CIS`, `EU`, `TW`, `MY`, `PK`, `BD`]

Параметр запроса `IND` предназначен только для Индии и подпадает под `client.ind.freefiremobile.com`  
[`IND`]

Параметр запроса `BR` предназначен для всех регионов, подпадающих под `client.us.freefiremobile.com`  
[`BR`, `US`, `NA`, `LATAM`]

### 💬 Пример успешного ответа может выглядеть так,
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

## API спама
Маршрут API = https://free-fire-data.vercel.app/api/spam?region={region}&uid={uid}&key={key}

**Конечная точка:** `api/spam`  
**Ключ:** `ВАШ-КЛЮЧ`  
**Метод:** `GET`  

Эта конечная точка отправляет 100 запросов на добавление в друзья на аккаунт игрока на основе указанного региона и идентификатора пользователя.

### 📨 Пример запроса
```http
GET https://free-fire-data.vercel.app/api/spam?region=ind&uid=2180732447&key=KEY123
```

### ☑️ Параметры запроса

| Параметр  | Тип    | Обязательный | Описание                              |
|-----------|--------|--------------|---------------------------------------|
| `region`  | строка | Да           | Код региона (`sg`, `ind`, `br`)       |
| `uid`     | целое  | Да           | Идентификатор пользователя            |
| `key`     | строка | Да           | Купить ключ на https://t.me/TrueClasher4 |

### ℹ️ Важное замечание

Параметр запроса `SG` предназначен для всех регионов, подпадающих под `clientbp.ggblueshark.com`  
[`SG`, `ID`, `ME`, `VN`, `TH`, `CIS`, `EU`, `TW`, `MY`, `PK`, `BD`]

Параметр запроса `IND` предназначен только для Индии и подпадает под `client.ind.freefiremobile.com`  
[`IND`]

Параметр запроса `BR` предназначен для всех регионов, подпадающих под `client.us.freefiremobile.com`  
[`BR`, `US`, `NA`, `LATAM`]

### 💬 Пример успешного ответа может выглядеть так,
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

## API изображений
Маршрут API = https://free-fire-data.vercel.app/api/images?iconName={iconName}&key={key}

**Конечная точка:** `api/images`  
**Ключ:** `ВАШ-КЛЮЧ`  
**Метод:** `GET`  

Эта конечная точка получает информацию об игроке на основе указанного региона и идентификатора пользователя.

### 📨 Пример запроса
```http
GET https://free-fire-data.vercel.app/api/images?iconName=Icon_avatar_hair_cos_eggday2021_headwear_blue&key=KEY123
```

### ☑️ Параметры запроса

| Параметр   | Тип    | Обязательный | Описание                              |
|------------|--------|--------------|---------------------------------------|
| `iconName` | строка | Да           | Название иконки.                      |
| `key`      | строка | Да           | Купить ключ на https://t.me/TrueClasher4 |

### 💬 Пример успешного ответа может выглядеть так,

![Icon_avatar_hair_cos_eggday2021_headwear_blue](https://github.com/realpega/free-fire-api/blob/main/images.png)

## API информации о картах Craftland
Маршрут API = https://free-fire-data.vercel.app/api/maps?region={region}&code=%23{CODE}&key={key}

**Конечная точка:** `api/maps`  
**Ключ:** `ВАШ-КЛЮЧ`  
**Метод:** `GET`  

Эта конечная точка получает информацию об игроке на основе указанного региона и идентификатора пользователя.

### 📨 Пример запроса
```http
GET https://free-fire-data.vercel.app/api/maps?region=sg&code=%23FREEFIREMAPCODE6969&key=KEY123
```

### ☑️ Параметры запроса

| Параметр  | Тип    | Обязательный | Описание                              |
|-----------|--------|--------------|---------------------------------------|
| `region`  | строка | Да           | Код региона (`sg`, `ind`, `br`)       |
| `uid`     | целое  | Да           | Идентификатор пользователя            |
| `key`     | строка | Да           | Купить ключ на https://t.me/TrueClasher4 |

### ℹ️ Важное замечание

Параметр запроса `SG` предназначен для всех регионов, подпадающих под `clientbp.ggblueshark.com`  
[`SG`, `ID`, `ME`, `VN`, `TH`, `CIS`, `EU`, `TW`, `MY`, `PK`, `BD`]

Параметр запроса `IND` предназначен только для Индии и подпадает под `client.ind.freefiremobile.com`  
[`IND`]

Параметр запроса `BR` предназначен для всех регионов, подпадающих под `client.us.freefiremobile.com`  
[`BR`, `US`, `NA`, `LATAM`]

### 💬 Пример успешного ответа может выглядеть так,
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
      "COMMON_ACCEPT": "ПРИНЯТЬ",
      "COMMON_BACK": "Назад",
      "COMMON_CANCEL": "Отмена",
      "COMMON_CONFIRM": "Подтвердить",
      "COMMON_CONTINUE_PURCHASE": "Продолжить покупку",
      "COMMON_COPY": "Копировать",
      "COMMON_COPY_FAILED": "Копирование не удалось",
      "COMMON_COPY_SUCCESS": "Копирование успешно",
      "COMMON_EXCHANGE": "Обменять",
      "COMMON_EXCHANGED": "Обменяно",
      "COMMON_FFTOKEN_HINT": "Преобразовано в {num}{иконка токена FF}",
      "COMMON_FREE": "Бесплатно",
      "COMMON_GEM_CONFIRM": "Потратить {cost} гем(ов) на покупку {NAME}?",
      "COMMON_GEM_CONFIRM2": "Потратить {cost} гемов на {num} вращение(й)?",
      "COMMON_HISTORY_DRAW": "История",
      "COMMON_HISTORY_NORECORDS": "Нет записей",
      "COMMON_HISTORY_PURCHASE": "История покупок",
      "COMMON_HISTORY_REDEEM": "История обмена",
      "COMMON_NO": "Нет",
      "COMMON_OWNED": "ВО ВЛАДЕНИИ",
      "COMMON_PRIZEPOOL": "Пул наград",
      "COMMON_PURCHASE": "Купить",
      "COMMON_PURCHASED": "Куплено",
      "COMMON_QUANTITY_MAX": "Максимум",
      "COMMON_REDEEM_CONFIRM": "Вы уверены, что хотите обменять этот предмет?",
      "COMMON_REJECT": "Отклонить",
      "COMMON_RULE": "Правила",
      "COMMON_SKIP": "Пропустить анимацию",
      "COMMON_SKIPANIMATION_TIP": "Нажмите в любом месте, чтобы пропустить анимацию",
      "COMMON_SPIN_AGAIN": "Вращать снова",
      "COMMON_TIPS_ITEM": "Награды будут отправлены прямо в ваш сейф",
      "COMMON_TIPS_TOKEN": "Токены автоматически накоплены",
      "COMMON_VISIT_GIFT": "Приветственный подарок",
      "COMMON_YES": "Да",
      "POPUP_NO_REMIND": "Не напоминать снова",
      "POPUP_TITLE_CONGRATULATIONS": "Поздравляем!",
      "POPUP_TITLE_REDEEM": "Поздравляем! Вы получили",
      "POPUP_TITLE_UNIQUE": "Уникальные предметы, которыми вы владеете",
      "UNIQUE_BUY_ALREADY_HAVE": "У вас уже есть этот предмет, при повторной покупке он будет преобразован в токены FF",
      "UNIQUE_BUY_ALREADY_HAVE_PART": "У вас уже есть некоторые из выбранных предметов. При повторном получении они будут преобразованы в токены FF.",
      "UNIQUE_REDEEM_ALREADY_HAVE": "У вас уже есть этот предмет, при повторном получении он будет преобразован в токены FF.",
      "TOAST_ERROR_CODE": "Неизвестная ошибка, код ошибки {code}",
      "TOAST_EVENTOVER": "Событие завершено",
      "TOAST_EVENT_CLOSED_AWHILE": "Событие временно закрыто. Пожалуйста, проверьте позже.",
      "TOAST_EVENT_END": "Событие завершено",
      "TOAST_EVENT_NOTOPEN": "Событие еще не началось",
      "TOAST_EXCHANGE_SUCCESS": "Успешно обменяно",
      "TOAST_GEM_NOT_ENOUGH": "Недостаточно алмазов, пожалуйста, пополните и вернитесь снова",
      "TOAST_LOGIN_FAILED": "Не удалось войти",
      "TOAST_NETWORK_BUSY": "Сервер занят, пожалуйста, попробуйте снова позже",
      "TOAST_NETWORK_ERROR": "Ошибка сетевого соединения, пожалуйста, попробуйте снова позже",
      "TOAST_OPERATE_BUSY": "Слишком много запросов, пожалуйста, попробуйте снова позже",
      "TOAST_PAY_FAILED": "Покупка не удалась",
      "TOAST_PURCHASE_SUCCESS": "Покупка успешна",
      "TOAST_SERVER_BUSY": "Сервер занят, пожалуйста, попробуйте снова позже",
      "TOAST_SERVER_NOTWORK": "Сервис недоступен",
      "TOAST_SERVER_TIMEOUT": "Тайм-аут сервиса",
      "TOAST_WRONG_REGION": "Это событие недоступно для вашего региона",
      "COMMON_CALLBACK": "Присоединяйтесь к бою!",
      "COMMON_JOIN": "Присоединиться",
      "COMMON_SHOOT": "Нажмите на цели",
      "COMMON_SHOOT_2": "Отличная работа! Чтобы продолжить, пожалуйста, перейдите в Free Fire!",
      "UGC_46_MAPSHARE_GOBUTTON": "ИССЛЕДОВАТЬ БОЛЬШЕ",
      "UGC_46_MAPSHARE_PLAYBUTTON": "ИГРАТЬ СЕЙЧАС",
      "UGC_46_MAPSHARE_WRONGMESSAGE": "ИЗВИНИТЕ, ЭТА КАРТА В ДАННЫЙ МОМЕНТ НЕДОСТУПНА.",
      "UGC_47_MAPSHARE_MAPCODE": "Код карты",
      "UGC_47_MAPSHARE_NAME": "Имя создателя",
      "UGC_47_MAPSHARE_TOAST1": "Успешно скопировано",
      "UGC_47_MAPSHARE_TOAST2": "Не удалось скопировать"
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

## API списка желаний игрока
Маршрут API = https://free-fire-data.vercel.app/api/wishlist?region={region}&uid={uid}&key={key}

**Конечная точка:** `api/wishlist`  
**Ключ:** `ВАШ-КЛЮЧ`  
**Метод:** `GET`  

Эта конечная точка получает информацию об игроке на основе указанного региона и идентификатора пользователя.

### 📨 Пример запроса
```http
GET https://free-fire-data.vercel.app/api/wishlist?region=ind&uid=2180732447&key=KEY123
```

### ☑️ Параметры запроса

| Параметр  | Тип    | Обязательный | Описание                              |
|-----------|--------|--------------|---------------------------------------|
| `region`  | строка | Да           | Код региона (`sg`, `ind`, `br`)       |
| `uid`     | целое  | Да           | Идентификатор пользователя            |
| `key`     | строка | Да           | Купить ключ на https://t.me/TrueClasher4 |

### ℹ️ Важное замечание

Параметр запроса `SG` предназначен для всех регионов, подпадающих под `clientbp.ggblueshark.com`  
[`SG`, `ID`, `ME`, `VN`, `TH`, `CIS`, `EU`, `TW`, `MY`, `PK`, `BD`]

Параметр запроса `IND` предназначен только для Индии и подпадает под `client.ind.freefiremobile.com`  
[`IND`]

Параметр запроса `BR` предназначен для всех регионов, подпадающих под `client.us.freefiremobile.com`  
[`BR`, `US`, `NA`, `LATAM`]

### 💬 Пример успешного ответа может выглядеть так,
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

📚 **Цель API**

Основная цель предоставления этого бесплатного API — улучшение опыта сообщества Free Fire. Garena Free Fire не предлагает официальных API для получения информации об аккаунтах, поэтому это пользовательское решение направлено на заполнение этого пробела, предоставляя игрокам и разработчикам ценные данные об аккаунте.

🧩 **(Некоторые из🤫) Используемые фреймворки и библиотеки**  
- **Flask**: Микрофреймворк для Python для создания конечных точек API.  
- **Flask-CORS**: Для обработки кросс-доменного обмена ресурсами (CORS).  
- **PyCryptodome**: Для реализации дешифрования и шифрования.  
- **Requests**: Для выполнения HTTP-запросов к серверу.

# 📁 Дополнительная информация

- Ответ API не отражает фактическую структуру, полученную от официального сервера Garena.  
- Структура ответа упрощена в удобном для пользователя формате для облегчения понимания любым человеком на любом уровне программирования.

# 😵 Ответы с ошибками
API может выдавать ответы с ошибками при неточных запросах пользователей!

### Примеры ошибок и решения

- **Код ошибки:** 400
  - **Сообщение:** Недопустимый регион.  
  - **Решение:** Убедитесь, что вы используете правильный код региона.

- **Код ошибки:** 429
  - **Сообщение:** Обнаружены аномальные запросы. Пожалуйста, избегайте неправильного использования API для посещений, иначе ваш IP может быть заблокирован!  
  - **Решение:** Избегайте чрезмерных запросов или свяжитесь с провайдером API для получения помощи.

- **Код ошибки:** 500
  - **Сообщение:** Произошла ошибка при обработке вашего запроса. Пожалуйста, перепроверьте ваш ID и регион.  
  - **Решение:** Дважды проверьте предоставленные ID пользователя и регион и повторите запрос. Если проблема сохраняется, свяжитесь с провайдером API для получения поддержки.

---

API создан Sounava777,  
Все права защищены!
