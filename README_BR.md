# 📝 Documentação da API

## API de Informações do Jogador
Rota da API = https://free-fire-data.vercel.app/api/data?region={region}&uid={uid}&key={key}

**Endpoint:** `api/data`  
**Chave:** `SUA-CHAVE`  
**Método:** `GET`  

Este endpoint recupera informações do jogador com base na região e ID de usuário especificados.

### 📨 Exemplo de Requisição
```http
GET https://free-fire-data.vercel.app/api/data?region=ind&uid=2180732447&key=KEY123
```

### ☑️ Parâmetros de Consulta

| Parâmetro | Tipo   | Obrigatório | Descrição                          |
|-----------|--------|-------------|------------------------------------|
| `region`  | string | Sim         | O código da região (`sg`, `ind`, `br`) |
| `uid`     | int    | Sim         | O ID do usuário                   |
| `key`     | string | Sim         | Compre a chave em https://t.me/TrueClasher4 |

### ℹ️ Nota Importante

Parâmetro de consulta `SG` é para todas as regiões que estão sob `clientbp.ggblueshark.com`  
[`SG`, `ID`, `ME`, `VN`, `TH`, `CIS`, `EU`, `TW`, `MY`, `PK`, `BD`]

Parâmetro de consulta `IND` é apenas para a Índia e está sob `client.ind.freefiremobile.com`  
[`IND`]

Parâmetro de consulta `BR` é para todas as regiões que estão sob `client.us.freefiremobile.com`  
[`BR`, `US`, `NA`, `LATAM`]

### 💬 Exemplo de uma Resposta Bem-Sucedida Pode Ser Assim,
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
    "signature": "i've lost my acc,  pls add me again MARVEL-CLINT"
  }
}
```

# 📝 Documentação da API

## API de Informações do Jogador
Rota da API = https://free-fire-data.vercel.app/api/data?region={region}&uid={uid}&key={key}

**Endpoint:** `api/data`  
**Chave:** `SUA-CHAVE`  
**Método:** `GET`  

Este endpoint recupera informações do jogador com base na região e ID de usuário especificados.

### 📨 Exemplo de Requisição
```http
GET https://free-fire-data.vercel.app/api/data?region=ind&uid=2180732447&key=KEY123
```

### ☑️ Parâmetros de Consulta

| Parâmetro | Tipo   | Obrigatório | Descrição                          |
|-----------|--------|-------------|------------------------------------|
| `region`  | string | Sim         | O código da região (`sg`, `ind`, `br`) |
| `uid`     | int    | Sim         | O ID do usuário                   |
| `key`     | string | Sim         | Compre a chave em https://t.me/TrueClasher4 |

### ℹ️ Nota Importante

Parâmetro de consulta `SG` é para todas as regiões que estão sob `clientbp.ggblueshark.com`  
[`SG`, `ID`, `ME`, `VN`, `TH`, `CIS`, `EU`, `TW`, `MY`, `PK`, `BD`]

Parâmetro de consulta `IND` é apenas para a Índia e está sob `client.ind.freefiremobile.com`  
[`IND`]

Parâmetro de consulta `BR` é para todas as regiões que estão sob `client.us.freefiremobile.com`  
[`BR`, `US`, `NA`, `LATAM`]

### 💬 Exemplo de uma Resposta Bem-Sucedida Pode Ser Assim,
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
    "signature": "i've lost my acc,  pls add me again MARVEL-CLINT"
  }
}
```

## API de Estatísticas do Jogador
Rota da API = https://free-fire-data.vercel.app/api/stats?region={region}&uid={uid}&key={key}

**Endpoint:** `api/stats`  
**Chave:** `SUA-CHAVE`  
**Método:** `GET`  

Este endpoint recupera informações de estatísticas do jogador com base na região e ID de usuário especificados.

### 📨 Exemplo de Requisição
```http
GET https://free-fire-data.vercel.app/api/stats?region=ind&uid=2180732447&key=KEY123
```

### ☑️ Parâmetros de Consulta

| Parâmetro | Tipo   | Obrigatório | Descrição                          |
|-----------|--------|-------------|------------------------------------|
| `region`  | string | Sim         | O código da região (`sg`, `ind`, `br`) |
| `uid`     | int    | Sim         | O ID do usuário                   |
| `key`     | string | Sim         | Compre a chave em https://t.me/TrueClasher4 |

### ℹ️ Nota Importante

Parâmetro de consulta `SG` é para todas as regiões que estão sob `clientbp.ggblueshark.com`  
[`SG`, `ID`, `ME`, `VN`, `TH`, `CIS`, `EU`, `TW`, `MY`, `PK`, `BD`]

Parâmetro de consulta `IND` é apenas para a Índia e está sob `client.ind.freefiremobile.com`  
[`IND`]

Parâmetro de consulta `BR` é para todas as regiões que estão sob `client.us.freefiremobile.com`  
[`BR`, `US`, `NA`, `LATAM`]

### 💬 Exemplo de uma Resposta Bem-Sucedida Pode Ser Assim,
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
