# Country-City-District JSON Dataset

Bu proje, **ülke, şehir, il, ilçe** verilerini JSON formatında sağlar. Veriler **relational-style** (ilişkisel) olarak düzenlenmiştir ve projelerde ülke/şehir/ilçe ilişkilerini yönetmek için kullanılabilir.
Güncel olarak tüm ülkeler mevcuttur. fakat il ve ilçe için mevcutta Türkiye'ye ait il/ilçe mevcuttur.

---

## JSON Yapısı

### 1. Countries (Ülkeler)

```json
[
  {
    "ID": 86,
    "Name": "Türkiye",
    "Code": "TR",
    "PhonePrefix": "+90"
  }
]
```

### 2.Cities (Şehirler)

```json
[
  {
    "ID": 1,
    "Name": "Adana",
    "PlateCode": 1,
    "CountryId": 86,
    "Color": "#000000",
    "Latitude": 370000.0,
    "Longitude": 353213.0
  },
  {
    "ID": 2,
    "Name": "Adıyaman",
    "PlateCode": 2,
    "CountryId": 86,
    "Color": "#000000",
    "Latitude": 377648.0,
    "Longitude": 382786.0
  }
]
```

### 3. CountryCity (Ülke-Şehir İlişkisi)

```json
[
  {
    "ID": 1,
    "CountryId": 86,
    "CityId": 1
  },
  {
    "ID": 2,
    "CountryId": 86,
    "CityId": 2
  }
]
```

### 4.Districts (İlçeler)

```json
[
  {
    "ID": 1,
    "Name": "Aladağ",
    "Code": "AD01-ALDG01"
  },
  {
    "ID": 2,
    "Name": "Ceyhan",
    "Code": "AD01-CYHN01"
  }
]
```

### 5.DistrictCity (İlçe-Şehir İlişkisi)

```json
[
  {
    "ID": 1,
    "DistrictId": 1,
    "CityId": 1
  },
  {
    "ID": 2,
    "DistrictId": 2,
    "CityId": 1
  }
]
```
