---
title: API Reference

language_tabs:
- bash
- javascript

includes:

search: true

toc_footers:
- <a href='http://github.com/mpociot/documentarian'>Documentation Powered by Documentarian</a>
---
<!-- START_INFO -->
# Info

Welcome to the generated API reference.
[Get Postman Collection](http://localhost/docs/collection.json)
<!-- END_INFO -->

#API

This API aims to provide needed structured national data for use by developers and other individuals or organisations.
For now, data available includes all states, LGAs, Wards and Polling units correctly structured with the hierarchy. Feel free to use or contribute.
Data is also provided as .sql or JSON
https://allnigeria-api.herokuapp.com/data/allnigeria.json
https://allnigeria-api.herokuapp.com/data/allnigeria.sql
<!-- START_24bb4a5389a5e41bec8e213104cff040 -->
## Show Everything
All data structured by states =&gt; LGAs =&gt; Wards =&gt; Polling Units will be returned. The size of this data is approximately 12MB
This endpoint is disabled due to large memory usage. However, the JSON data is available via the link above
If you wish to use this endpoint (possibly in a forked version), uncomment lines 26 and 28 of NigController and delete line 22.

> Example request:

```bash
curl -X GET "https://http://allnigeria-api.herokuapp.com/api/v1/everything" \
-H "Accept: application/json"
```

```javascript
var settings = {
    "async": true,
    "crossDomain": true,
    "url": "https://http://allnigeria-api.herokuapp.com/api/v1/everything",
    "method": "GET",
    "headers": {
        "accept": "application/json"
    }
}

$.ajax(settings).done(function (response) {
    console.log(response);
});
```

> Example response:

```json
{
    "success": true,
    "message": "All states with corresponding LGAs, Wards and Polling Units",
    "data": []
}
```

### HTTP Request
`GET api/v1/everything`

`HEAD api/v1/everything`


<!-- END_24bb4a5389a5e41bec8e213104cff040 -->

<!-- START_0000ac6e7f1b13ada4bac431c152854c -->
## Show States
All States will be returned

> Example request:

```bash
curl -X GET "https://http://allnigeria-api.herokuapp.com/api/v1/states" \
-H "Accept: application/json"
```

```javascript
var settings = {
    "async": true,
    "crossDomain": true,
    "url": "https://http://allnigeria-api.herokuapp.com/api/v1/states",
    "method": "GET",
    "headers": {
        "accept": "application/json"
    }
}

$.ajax(settings).done(function (response) {
    console.log(response);
});
```

> Example response:

```json
{
    "success": true,
    "message": "All states",
    "data": [
        {
            "id": 1,
            "name": "Abia"
        },
        {
            "id": 2,
            "name": "Adamawa"
        },
        {
            "id": 3,
            "name": "Akwa ibom"
        },
        {
            "id": 4,
            "name": "Anambra"
        },
        {
            "id": 5,
            "name": "Bauchi"
        },
        {
            "id": 6,
            "name": "Bayelsa"
        },
        {
            "id": 7,
            "name": "Benue"
        },
        {
            "id": 8,
            "name": "Borno"
        },
        {
            "id": 9,
            "name": "Cross river"
        },
        {
            "id": 10,
            "name": "Delta"
        },
        {
            "id": 11,
            "name": "Ebonyi"
        },
        {
            "id": 12,
            "name": "Edo"
        },
        {
            "id": 13,
            "name": "Ekiti"
        },
        {
            "id": 14,
            "name": "Enugu"
        },
        {
            "id": 15,
            "name": "Fct"
        },
        {
            "id": 16,
            "name": "Gombe"
        },
        {
            "id": 17,
            "name": "Imo"
        },
        {
            "id": 18,
            "name": "Jigawa"
        },
        {
            "id": 19,
            "name": "Kaduna"
        },
        {
            "id": 20,
            "name": "Kano"
        },
        {
            "id": 21,
            "name": "Katsina"
        },
        {
            "id": 22,
            "name": "Kebbi"
        },
        {
            "id": 23,
            "name": "Kogi"
        },
        {
            "id": 24,
            "name": "Kwara"
        },
        {
            "id": 25,
            "name": "Lagos"
        },
        {
            "id": 26,
            "name": "Nasarawa"
        },
        {
            "id": 27,
            "name": "Niger"
        },
        {
            "id": 28,
            "name": "Ogun"
        },
        {
            "id": 29,
            "name": "Ondo"
        },
        {
            "id": 30,
            "name": "Osun"
        },
        {
            "id": 31,
            "name": "Oyo"
        },
        {
            "id": 32,
            "name": "Plateau"
        },
        {
            "id": 33,
            "name": "Rivers"
        },
        {
            "id": 34,
            "name": "Sokoto"
        },
        {
            "id": 35,
            "name": "Taraba"
        },
        {
            "id": 36,
            "name": "Yobe"
        },
        {
            "id": 37,
            "name": "Zamfara"
        }
    ]
}
```

### HTTP Request
`GET api/v1/states`

`HEAD api/v1/states`


<!-- END_0000ac6e7f1b13ada4bac431c152854c -->

<!-- START_e3a8359c2a2db1c2299bb91a0569b086 -->
## Show States with LGAs
All States will be returned with their corresponding LGAs

> Example request:

```bash
curl -X GET "https://http://allnigeria-api.herokuapp.com/api/v1/states/lgas" \
-H "Accept: application/json"
```

```javascript
var settings = {
    "async": true,
    "crossDomain": true,
    "url": "https://http://allnigeria-api.herokuapp.com/api/v1/states/lgas",
    "method": "GET",
    "headers": {
        "accept": "application/json"
    }
}

$.ajax(settings).done(function (response) {
    console.log(response);
});
```

> Example response:

```json
{
    "success": true,
    "message": "All states with corresponding LGAs",
    "data": [
        {
            "id": 1,
            "name": "Abia",
            "lgas": [
                {
                    "id": 1,
                    "name": "Aba north",
                    "state_id": 1
                },
                {
                    "id": 2,
                    "name": "Aba south",
                    "state_id": 1
                },
                {
                    "id": 3,
                    "name": "Arochukwu",
                    "state_id": 1
                },
                {
                    "id": 4,
                    "name": "Bende",
                    "state_id": 1
                },
                {
                    "id": 5,
                    "name": "Ikwuano",
                    "state_id": 1
                },
                {
                    "id": 6,
                    "name": "Isiala ngwa north",
                    "state_id": 1
                },
                {
                    "id": 7,
                    "name": "Isiala ngwa south",
                    "state_id": 1
                },
                {
                    "id": 8,
                    "name": "Isuikwuato",
                    "state_id": 1
                },
                {
                    "id": 9,
                    "name": "Obingwa",
                    "state_id": 1
                },
                {
                    "id": 10,
                    "name": "Ohafia",
                    "state_id": 1
                },
                {
                    "id": 11,
                    "name": "Osisioma",
                    "state_id": 1
                },
                {
                    "id": 12,
                    "name": "Ugwunagbo",
                    "state_id": 1
                },
                {
                    "id": 13,
                    "name": "Ukwa  west",
                    "state_id": 1
                },
                {
                    "id": 14,
                    "name": "Ukwa east",
                    "state_id": 1
                },
                {
                    "id": 15,
                    "name": "Umu - nneochi",
                    "state_id": 1
                },
                {
                    "id": 16,
                    "name": "Umuahia  south",
                    "state_id": 1
                },
                {
                    "id": 17,
                    "name": "Umuahia north",
                    "state_id": 1
                }
            ]
        },
        {
            "id": 2,
            "name": "Adamawa",
            "lgas": [
                {
                    "id": 18,
                    "name": "Demsa",
                    "state_id": 2
                },
                {
                    "id": 19,
                    "name": "Fufore",
                    "state_id": 2
                },
                {
                    "id": 20,
                    "name": "Ganye",
                    "state_id": 2
                },
                {
                    "id": 21,
                    "name": "Gire 1",
                    "state_id": 2
                },
                {
                    "id": 22,
                    "name": "Gombi",
                    "state_id": 2
                },
                {
                    "id": 23,
                    "name": "Guyuk",
                    "state_id": 2
                },
                {
                    "id": 24,
                    "name": "Hong",
                    "state_id": 2
                },
                {
                    "id": 25,
                    "name": "Jada",
                    "state_id": 2
                },
                {
                    "id": 26,
                    "name": "Lamurde",
                    "state_id": 2
                },
                {
                    "id": 27,
                    "name": "Madagali",
                    "state_id": 2
                },
                {
                    "id": 28,
                    "name": "Maiha",
                    "state_id": 2
                },
                {
                    "id": 29,
                    "name": "Mayo - belwa",
                    "state_id": 2
                },
                {
                    "id": 30,
                    "name": "Michika",
                    "state_id": 2
                },
                {
                    "id": 31,
                    "name": "Mubi north",
                    "state_id": 2
                },
                {
                    "id": 32,
                    "name": "Mubi south",
                    "state_id": 2
                },
                {
                    "id": 33,
                    "name": "Numan",
                    "state_id": 2
                },
                {
                    "id": 34,
                    "name": "Shelleng",
                    "state_id": 2
                },
                {
                    "id": 35,
                    "name": "Song",
                    "state_id": 2
                },
                {
                    "id": 36,
                    "name": "Toungo",
                    "state_id": 2
                },
                {
                    "id": 37,
                    "name": "Yola north",
                    "state_id": 2
                },
                {
                    "id": 38,
                    "name": "Yola south",
                    "state_id": 2
                }
            ]
        },
        {
            "id": 3,
            "name": "Akwa ibom",
            "lgas": [
                {
                    "id": 39,
                    "name": "Abak",
                    "state_id": 3
                },
                {
                    "id": 40,
                    "name": "Eastern obolo",
                    "state_id": 3
                },
                {
                    "id": 41,
                    "name": "Eket",
                    "state_id": 3
                },
                {
                    "id": 42,
                    "name": "Esit eket (uquo)",
                    "state_id": 3
                },
                {
                    "id": 43,
                    "name": "Essien udim",
                    "state_id": 3
                },
                {
                    "id": 44,
                    "name": "Etim ekpo",
                    "state_id": 3
                },
                {
                    "id": 45,
                    "name": "Etinan",
                    "state_id": 3
                },
                {
                    "id": 46,
                    "name": "Ibeno",
                    "state_id": 3
                },
                {
                    "id": 47,
                    "name": "Ibesikpo asutan",
                    "state_id": 3
                },
                {
                    "id": 48,
                    "name": "Ibiono ibom",
                    "state_id": 3
                },
                {
                    "id": 49,
                    "name": "Ika",
                    "state_id": 3
                },
                {
                    "id": 50,
                    "name": "Ikono",
                    "state_id": 3
                },
                {
                    "id": 51,
                    "name": "Ikot abasi",
                    "state_id": 3
                },
                {
                    "id": 52,
                    "name": "Ikot ekpene",
                    "state_id": 3
                },
                {
                    "id": 53,
                    "name": "Ini",
                    "state_id": 3
                },
                {
                    "id": 54,
                    "name": "Itu",
                    "state_id": 3
                },
                {
                    "id": 55,
                    "name": "Mbo",
                    "state_id": 3
                },
                {
                    "id": 56,
                    "name": "Mkpat enin",
                    "state_id": 3
                },
                {
                    "id": 57,
                    "name": "Nsit atai",
                    "state_id": 3
                },
                {
                    "id": 58,
                    "name": "Nsit ibom",
                    "state_id": 3
                },
                {
                    "id": 59,
                    "name": "Nsit ubium",
                    "state_id": 3
                },
                {
                    "id": 60,
                    "name": "Obot akara",
                    "state_id": 3
                },
                {
                    "id": 61,
                    "name": "Okobo",
                    "state_id": 3
                },
                {
                    "id": 62,
                    "name": "Onna",
                    "state_id": 3
                },
                {
                    "id": 63,
                    "name": "Oron",
                    "state_id": 3
                },
                {
                    "id": 64,
                    "name": "Oruk anam",
                    "state_id": 3
                },
                {
                    "id": 65,
                    "name": "Udung uko",
                    "state_id": 3
                },
                {
                    "id": 66,
                    "name": "Ukanafun",
                    "state_id": 3
                },
                {
                    "id": 67,
                    "name": "Uruan",
                    "state_id": 3
                },
                {
                    "id": 68,
                    "name": "Urue offong oruko",
                    "state_id": 3
                },
                {
                    "id": 69,
                    "name": "Uyo",
                    "state_id": 3
                }
            ]
        },
        {
            "id": 4,
            "name": "Anambra",
            "lgas": [
                {
                    "id": 70,
                    "name": "Aguata",
                    "state_id": 4
                },
                {
                    "id": 71,
                    "name": "Anambra east",
                    "state_id": 4
                },
                {
                    "id": 72,
                    "name": "Anambra west",
                    "state_id": 4
                },
                {
                    "id": 73,
                    "name": "Anaocha",
                    "state_id": 4
                },
                {
                    "id": 74,
                    "name": "Awka north",
                    "state_id": 4
                },
                {
                    "id": 75,
                    "name": "Awka south",
                    "state_id": 4
                },
                {
                    "id": 76,
                    "name": "Ayamelum",
                    "state_id": 4
                },
                {
                    "id": 77,
                    "name": "Dunukofia",
                    "state_id": 4
                },
                {
                    "id": 78,
                    "name": "Ekwusigo",
                    "state_id": 4
                },
                {
                    "id": 79,
                    "name": "Idemili north",
                    "state_id": 4
                },
                {
                    "id": 80,
                    "name": "Idemili-south",
                    "state_id": 4
                },
                {
                    "id": 81,
                    "name": "Ihala",
                    "state_id": 4
                },
                {
                    "id": 82,
                    "name": "Njikoka",
                    "state_id": 4
                },
                {
                    "id": 83,
                    "name": "Nnewi north",
                    "state_id": 4
                },
                {
                    "id": 84,
                    "name": "Nnewi south",
                    "state_id": 4
                },
                {
                    "id": 85,
                    "name": "Ogbaru",
                    "state_id": 4
                },
                {
                    "id": 86,
                    "name": "Onitsha -south",
                    "state_id": 4
                },
                {
                    "id": 87,
                    "name": "Onitsha-north",
                    "state_id": 4
                },
                {
                    "id": 88,
                    "name": "Orumba  south",
                    "state_id": 4
                },
                {
                    "id": 89,
                    "name": "Orumba north",
                    "state_id": 4
                },
                {
                    "id": 90,
                    "name": "Oyi",
                    "state_id": 4
                }
            ]
        },
        {
            "id": 5,
            "name": "Bauchi",
            "lgas": [
                {
                    "id": 91,
                    "name": "Alkaleri",
                    "state_id": 5
                },
                {
                    "id": 92,
                    "name": "Bauchi",
                    "state_id": 5
                },
                {
                    "id": 93,
                    "name": "Bogoro",
                    "state_id": 5
                },
                {
                    "id": 94,
                    "name": "Dambam",
                    "state_id": 5
                },
                {
                    "id": 95,
                    "name": "Darazo",
                    "state_id": 5
                },
                {
                    "id": 96,
                    "name": "Dass",
                    "state_id": 5
                },
                {
                    "id": 97,
                    "name": "Gamawa",
                    "state_id": 5
                },
                {
                    "id": 98,
                    "name": "Ganjuwa",
                    "state_id": 5
                },
                {
                    "id": 99,
                    "name": "Giade",
                    "state_id": 5
                },
                {
                    "id": 100,
                    "name": "Itas\/gadau",
                    "state_id": 5
                },
                {
                    "id": 101,
                    "name": "Jama'are",
                    "state_id": 5
                },
                {
                    "id": 102,
                    "name": "Katagum",
                    "state_id": 5
                },
                {
                    "id": 103,
                    "name": "Kirfi",
                    "state_id": 5
                },
                {
                    "id": 104,
                    "name": "Misau",
                    "state_id": 5
                },
                {
                    "id": 105,
                    "name": "Ningi",
                    "state_id": 5
                },
                {
                    "id": 106,
                    "name": "Shira",
                    "state_id": 5
                },
                {
                    "id": 107,
                    "name": "Tafawa balewa",
                    "state_id": 5
                },
                {
                    "id": 108,
                    "name": "Toro",
                    "state_id": 5
                },
                {
                    "id": 109,
                    "name": "Warji",
                    "state_id": 5
                },
                {
                    "id": 110,
                    "name": "Zaki",
                    "state_id": 5
                }
            ]
        },
        {
            "id": 6,
            "name": "Bayelsa",
            "lgas": [
                {
                    "id": 111,
                    "name": "Brass",
                    "state_id": 6
                },
                {
                    "id": 112,
                    "name": "Ekeremor",
                    "state_id": 6
                },
                {
                    "id": 113,
                    "name": "Kolokuma\/opokuma",
                    "state_id": 6
                },
                {
                    "id": 114,
                    "name": "Nembe",
                    "state_id": 6
                },
                {
                    "id": 115,
                    "name": "Ogbia",
                    "state_id": 6
                },
                {
                    "id": 116,
                    "name": "Sagbama",
                    "state_id": 6
                },
                {
                    "id": 117,
                    "name": "Southern ijaw",
                    "state_id": 6
                },
                {
                    "id": 118,
                    "name": "Yenagoa",
                    "state_id": 6
                }
            ]
        },
        {
            "id": 7,
            "name": "Benue",
            "lgas": [
                {
                    "id": 119,
                    "name": "Ado",
                    "state_id": 7
                },
                {
                    "id": 120,
                    "name": "Agatu",
                    "state_id": 7
                },
                {
                    "id": 121,
                    "name": "Apa",
                    "state_id": 7
                },
                {
                    "id": 122,
                    "name": "Buruku",
                    "state_id": 7
                },
                {
                    "id": 123,
                    "name": "Gboko",
                    "state_id": 7
                },
                {
                    "id": 124,
                    "name": "Guma",
                    "state_id": 7
                },
                {
                    "id": 125,
                    "name": "Gwer east",
                    "state_id": 7
                },
                {
                    "id": 126,
                    "name": "Gwer west",
                    "state_id": 7
                },
                {
                    "id": 127,
                    "name": "Katsina-ala",
                    "state_id": 7
                },
                {
                    "id": 128,
                    "name": "Konshisha",
                    "state_id": 7
                },
                {
                    "id": 129,
                    "name": "Kwande",
                    "state_id": 7
                },
                {
                    "id": 130,
                    "name": "Logo",
                    "state_id": 7
                },
                {
                    "id": 131,
                    "name": "Makurdi",
                    "state_id": 7
                },
                {
                    "id": 132,
                    "name": "Obi",
                    "state_id": 7
                },
                {
                    "id": 133,
                    "name": "Ogbadibo",
                    "state_id": 7
                },
                {
                    "id": 134,
                    "name": "Ohimini",
                    "state_id": 7
                },
                {
                    "id": 135,
                    "name": "Oju",
                    "state_id": 7
                },
                {
                    "id": 136,
                    "name": "Okpokwu",
                    "state_id": 7
                },
                {
                    "id": 137,
                    "name": "Otukpo",
                    "state_id": 7
                },
                {
                    "id": 138,
                    "name": "Tarka",
                    "state_id": 7
                },
                {
                    "id": 139,
                    "name": "Ukum",
                    "state_id": 7
                },
                {
                    "id": 140,
                    "name": "Ushongo",
                    "state_id": 7
                },
                {
                    "id": 141,
                    "name": "Vandeikya",
                    "state_id": 7
                }
            ]
        },
        {
            "id": 8,
            "name": "Borno",
            "lgas": [
                {
                    "id": 142,
                    "name": "Abadam",
                    "state_id": 8
                },
                {
                    "id": 143,
                    "name": "Askira \/ uba",
                    "state_id": 8
                },
                {
                    "id": 144,
                    "name": "Bama",
                    "state_id": 8
                },
                {
                    "id": 145,
                    "name": "Bayo",
                    "state_id": 8
                },
                {
                    "id": 146,
                    "name": "Biu",
                    "state_id": 8
                },
                {
                    "id": 147,
                    "name": "Chibok",
                    "state_id": 8
                },
                {
                    "id": 148,
                    "name": "Damboa",
                    "state_id": 8
                },
                {
                    "id": 149,
                    "name": "Dikwa",
                    "state_id": 8
                },
                {
                    "id": 150,
                    "name": "Gubio",
                    "state_id": 8
                },
                {
                    "id": 151,
                    "name": "Guzamala",
                    "state_id": 8
                },
                {
                    "id": 152,
                    "name": "Gwoza",
                    "state_id": 8
                },
                {
                    "id": 153,
                    "name": "Hawul",
                    "state_id": 8
                },
                {
                    "id": 154,
                    "name": "Jere",
                    "state_id": 8
                },
                {
                    "id": 155,
                    "name": "Kaga",
                    "state_id": 8
                },
                {
                    "id": 156,
                    "name": "Kala balge",
                    "state_id": 8
                },
                {
                    "id": 157,
                    "name": "Konduga",
                    "state_id": 8
                },
                {
                    "id": 158,
                    "name": "Kukawa",
                    "state_id": 8
                },
                {
                    "id": 159,
                    "name": "Kwaya \/ kusar",
                    "state_id": 8
                },
                {
                    "id": 160,
                    "name": "Mafa",
                    "state_id": 8
                },
                {
                    "id": 161,
                    "name": "Magumeri",
                    "state_id": 8
                },
                {
                    "id": 162,
                    "name": "Maiduguri m. c.",
                    "state_id": 8
                },
                {
                    "id": 163,
                    "name": "Marte",
                    "state_id": 8
                },
                {
                    "id": 164,
                    "name": "Mobbar",
                    "state_id": 8
                },
                {
                    "id": 165,
                    "name": "Monguno",
                    "state_id": 8
                },
                {
                    "id": 166,
                    "name": "Ngala",
                    "state_id": 8
                },
                {
                    "id": 167,
                    "name": "Nganzai",
                    "state_id": 8
                },
                {
                    "id": 168,
                    "name": "Shani",
                    "state_id": 8
                }
            ]
        },
        {
            "id": 9,
            "name": "Cross river",
            "lgas": [
                {
                    "id": 169,
                    "name": "Abi",
                    "state_id": 9
                },
                {
                    "id": 170,
                    "name": "Akamkpa",
                    "state_id": 9
                },
                {
                    "id": 171,
                    "name": "Akpabuyo",
                    "state_id": 9
                },
                {
                    "id": 172,
                    "name": "Bakassi",
                    "state_id": 9
                },
                {
                    "id": 173,
                    "name": "Bekwarra",
                    "state_id": 9
                },
                {
                    "id": 174,
                    "name": "Biase",
                    "state_id": 9
                },
                {
                    "id": 175,
                    "name": "Boki",
                    "state_id": 9
                },
                {
                    "id": 176,
                    "name": "Calabar municipality",
                    "state_id": 9
                },
                {
                    "id": 177,
                    "name": "Calabar south",
                    "state_id": 9
                },
                {
                    "id": 178,
                    "name": "Etung",
                    "state_id": 9
                },
                {
                    "id": 179,
                    "name": "Ikom",
                    "state_id": 9
                },
                {
                    "id": 180,
                    "name": "Obanliku",
                    "state_id": 9
                },
                {
                    "id": 181,
                    "name": "Obubra",
                    "state_id": 9
                },
                {
                    "id": 182,
                    "name": "Obudu",
                    "state_id": 9
                },
                {
                    "id": 183,
                    "name": "Odukpani",
                    "state_id": 9
                },
                {
                    "id": 184,
                    "name": "Ogoja",
                    "state_id": 9
                },
                {
                    "id": 185,
                    "name": "Yakurr",
                    "state_id": 9
                },
                {
                    "id": 186,
                    "name": "Yala",
                    "state_id": 9
                }
            ]
        },
        {
            "id": 10,
            "name": "Delta",
            "lgas": [
                {
                    "id": 187,
                    "name": "Aniocha - south",
                    "state_id": 10
                },
                {
                    "id": 188,
                    "name": "Aniocha north",
                    "state_id": 10
                },
                {
                    "id": 189,
                    "name": "Bomadi",
                    "state_id": 10
                },
                {
                    "id": 190,
                    "name": "Burutu",
                    "state_id": 10
                },
                {
                    "id": 191,
                    "name": "Ethiope  east",
                    "state_id": 10
                },
                {
                    "id": 192,
                    "name": "Ethiope  west",
                    "state_id": 10
                },
                {
                    "id": 193,
                    "name": "Ika - south",
                    "state_id": 10
                },
                {
                    "id": 194,
                    "name": "Ika north- east",
                    "state_id": 10
                },
                {
                    "id": 195,
                    "name": "Isoko north",
                    "state_id": 10
                },
                {
                    "id": 196,
                    "name": "Isoko south",
                    "state_id": 10
                },
                {
                    "id": 197,
                    "name": "Ndokwa east",
                    "state_id": 10
                },
                {
                    "id": 198,
                    "name": "Ndokwa west",
                    "state_id": 10
                },
                {
                    "id": 199,
                    "name": "Okpe",
                    "state_id": 10
                },
                {
                    "id": 200,
                    "name": "Oshimili - north",
                    "state_id": 10
                },
                {
                    "id": 201,
                    "name": "Oshimili - south",
                    "state_id": 10
                },
                {
                    "id": 202,
                    "name": "Patani",
                    "state_id": 10
                },
                {
                    "id": 203,
                    "name": "Sapele",
                    "state_id": 10
                },
                {
                    "id": 204,
                    "name": "Udu",
                    "state_id": 10
                },
                {
                    "id": 205,
                    "name": "Ughelli north",
                    "state_id": 10
                },
                {
                    "id": 206,
                    "name": "Ughelli south",
                    "state_id": 10
                },
                {
                    "id": 207,
                    "name": "Ukwuani",
                    "state_id": 10
                },
                {
                    "id": 208,
                    "name": "Uvwie",
                    "state_id": 10
                },
                {
                    "id": 209,
                    "name": "Warri  north",
                    "state_id": 10
                },
                {
                    "id": 210,
                    "name": "Warri south",
                    "state_id": 10
                },
                {
                    "id": 211,
                    "name": "Warri south  west",
                    "state_id": 10
                }
            ]
        },
        {
            "id": 11,
            "name": "Ebonyi",
            "lgas": [
                {
                    "id": 212,
                    "name": "Abakaliki",
                    "state_id": 11
                },
                {
                    "id": 213,
                    "name": "Afikpo  south",
                    "state_id": 11
                },
                {
                    "id": 214,
                    "name": "Afikpo north",
                    "state_id": 11
                },
                {
                    "id": 215,
                    "name": "Ebonyi",
                    "state_id": 11
                },
                {
                    "id": 216,
                    "name": "Ezza north",
                    "state_id": 11
                },
                {
                    "id": 217,
                    "name": "Ezza south",
                    "state_id": 11
                },
                {
                    "id": 218,
                    "name": "Ikwo",
                    "state_id": 11
                },
                {
                    "id": 219,
                    "name": "Ishielu",
                    "state_id": 11
                },
                {
                    "id": 220,
                    "name": "Ivo",
                    "state_id": 11
                },
                {
                    "id": 221,
                    "name": "Izzi",
                    "state_id": 11
                },
                {
                    "id": 222,
                    "name": "Ohaozara",
                    "state_id": 11
                },
                {
                    "id": 223,
                    "name": "Ohaukwu",
                    "state_id": 11
                },
                {
                    "id": 224,
                    "name": "Onicha",
                    "state_id": 11
                }
            ]
        },
        {
            "id": 12,
            "name": "Edo",
            "lgas": [
                {
                    "id": 225,
                    "name": "Akoko edo",
                    "state_id": 12
                },
                {
                    "id": 226,
                    "name": "Egor",
                    "state_id": 12
                },
                {
                    "id": 227,
                    "name": "Esan central",
                    "state_id": 12
                },
                {
                    "id": 228,
                    "name": "Esan north east",
                    "state_id": 12
                },
                {
                    "id": 229,
                    "name": "Esan south east",
                    "state_id": 12
                },
                {
                    "id": 230,
                    "name": "Esan west",
                    "state_id": 12
                },
                {
                    "id": 231,
                    "name": "Etsako  west",
                    "state_id": 12
                },
                {
                    "id": 232,
                    "name": "Etsako central",
                    "state_id": 12
                },
                {
                    "id": 233,
                    "name": "Etsako east",
                    "state_id": 12
                },
                {
                    "id": 234,
                    "name": "Igueben",
                    "state_id": 12
                },
                {
                    "id": 235,
                    "name": "Ikpoba\/okha",
                    "state_id": 12
                },
                {
                    "id": 236,
                    "name": "Oredo",
                    "state_id": 12
                },
                {
                    "id": 237,
                    "name": "Orhionmwon",
                    "state_id": 12
                },
                {
                    "id": 238,
                    "name": "Ovia north east",
                    "state_id": 12
                },
                {
                    "id": 239,
                    "name": "Ovia south west",
                    "state_id": 12
                },
                {
                    "id": 240,
                    "name": "Owan east",
                    "state_id": 12
                },
                {
                    "id": 241,
                    "name": "Owan west",
                    "state_id": 12
                },
                {
                    "id": 242,
                    "name": "Uhunmwode",
                    "state_id": 12
                }
            ]
        },
        {
            "id": 13,
            "name": "Ekiti",
            "lgas": [
                {
                    "id": 243,
                    "name": "Ado ekiti",
                    "state_id": 13
                },
                {
                    "id": 244,
                    "name": "Efon",
                    "state_id": 13
                },
                {
                    "id": 245,
                    "name": "Ekiti east",
                    "state_id": 13
                },
                {
                    "id": 246,
                    "name": "Ekiti south west",
                    "state_id": 13
                },
                {
                    "id": 247,
                    "name": "Ekiti west",
                    "state_id": 13
                },
                {
                    "id": 248,
                    "name": "Emure",
                    "state_id": 13
                },
                {
                    "id": 249,
                    "name": "Gbonyin",
                    "state_id": 13
                },
                {
                    "id": 250,
                    "name": "Ido \/ osi",
                    "state_id": 13
                },
                {
                    "id": 251,
                    "name": "Ijero",
                    "state_id": 13
                },
                {
                    "id": 252,
                    "name": "Ikere",
                    "state_id": 13
                },
                {
                    "id": 253,
                    "name": "Ikole",
                    "state_id": 13
                },
                {
                    "id": 254,
                    "name": "Ilejemeje",
                    "state_id": 13
                },
                {
                    "id": 255,
                    "name": "Irepodun \/ ifelodun",
                    "state_id": 13
                },
                {
                    "id": 256,
                    "name": "Ise \/ orun",
                    "state_id": 13
                },
                {
                    "id": 257,
                    "name": "Moba",
                    "state_id": 13
                },
                {
                    "id": 258,
                    "name": "Oye",
                    "state_id": 13
                }
            ]
        },
        {
            "id": 14,
            "name": "Enugu",
            "lgas": [
                {
                    "id": 259,
                    "name": "Aninri",
                    "state_id": 14
                },
                {
                    "id": 260,
                    "name": "Awgu",
                    "state_id": 14
                },
                {
                    "id": 261,
                    "name": "Enugu east",
                    "state_id": 14
                },
                {
                    "id": 262,
                    "name": "Enugu north",
                    "state_id": 14
                },
                {
                    "id": 263,
                    "name": "Enugu south",
                    "state_id": 14
                },
                {
                    "id": 264,
                    "name": "Ezeagu",
                    "state_id": 14
                },
                {
                    "id": 265,
                    "name": "Igbo etiti",
                    "state_id": 14
                },
                {
                    "id": 266,
                    "name": "Igbo eze north",
                    "state_id": 14
                },
                {
                    "id": 267,
                    "name": "Igbo eze south",
                    "state_id": 14
                },
                {
                    "id": 268,
                    "name": "Isi uzo",
                    "state_id": 14
                },
                {
                    "id": 269,
                    "name": "Nkanu east",
                    "state_id": 14
                },
                {
                    "id": 270,
                    "name": "Nkanu west",
                    "state_id": 14
                },
                {
                    "id": 271,
                    "name": "Nsukka",
                    "state_id": 14
                },
                {
                    "id": 272,
                    "name": "Oji-river",
                    "state_id": 14
                },
                {
                    "id": 273,
                    "name": "Udenu",
                    "state_id": 14
                },
                {
                    "id": 274,
                    "name": "Udi",
                    "state_id": 14
                },
                {
                    "id": 275,
                    "name": "Uzo-uwani",
                    "state_id": 14
                }
            ]
        },
        {
            "id": 15,
            "name": "Fct",
            "lgas": [
                {
                    "id": 276,
                    "name": "Abaji",
                    "state_id": 15
                },
                {
                    "id": 277,
                    "name": "Bwari",
                    "state_id": 15
                },
                {
                    "id": 278,
                    "name": "Gwagwalada",
                    "state_id": 15
                },
                {
                    "id": 279,
                    "name": "Kuje",
                    "state_id": 15
                },
                {
                    "id": 280,
                    "name": "Kwali",
                    "state_id": 15
                },
                {
                    "id": 281,
                    "name": "Municipal",
                    "state_id": 15
                }
            ]
        },
        {
            "id": 16,
            "name": "Gombe",
            "lgas": [
                {
                    "id": 282,
                    "name": "Akko",
                    "state_id": 16
                },
                {
                    "id": 283,
                    "name": "Balanga",
                    "state_id": 16
                },
                {
                    "id": 284,
                    "name": "Billiri",
                    "state_id": 16
                },
                {
                    "id": 285,
                    "name": "Dukku",
                    "state_id": 16
                },
                {
                    "id": 286,
                    "name": "Funakaye",
                    "state_id": 16
                },
                {
                    "id": 287,
                    "name": "Gombe",
                    "state_id": 16
                },
                {
                    "id": 288,
                    "name": "Kaltungo",
                    "state_id": 16
                },
                {
                    "id": 289,
                    "name": "Kwami",
                    "state_id": 16
                },
                {
                    "id": 290,
                    "name": "Nafada",
                    "state_id": 16
                },
                {
                    "id": 291,
                    "name": "Shongom",
                    "state_id": 16
                },
                {
                    "id": 292,
                    "name": "Yalmaltu\/ deba",
                    "state_id": 16
                }
            ]
        },
        {
            "id": 17,
            "name": "Imo",
            "lgas": [
                {
                    "id": 293,
                    "name": "Aboh mbaise",
                    "state_id": 17
                },
                {
                    "id": 294,
                    "name": "Ahiazu mbaise",
                    "state_id": 17
                },
                {
                    "id": 295,
                    "name": "Ehime mbano",
                    "state_id": 17
                },
                {
                    "id": 296,
                    "name": "Ezinihitte mbaise",
                    "state_id": 17
                },
                {
                    "id": 297,
                    "name": "Ideato north",
                    "state_id": 17
                },
                {
                    "id": 298,
                    "name": "Ideato south",
                    "state_id": 17
                },
                {
                    "id": 299,
                    "name": "Ihitte\/uboma (isinweke)",
                    "state_id": 17
                },
                {
                    "id": 300,
                    "name": "Ikeduru (iho)",
                    "state_id": 17
                },
                {
                    "id": 301,
                    "name": "Isiala mbano (umuelemai)",
                    "state_id": 17
                },
                {
                    "id": 302,
                    "name": "Isu (umundugba)",
                    "state_id": 17
                },
                {
                    "id": 303,
                    "name": "Mbaitoli (nwaorieubi)",
                    "state_id": 17
                },
                {
                    "id": 304,
                    "name": "Ngor okpala (umuneke)",
                    "state_id": 17
                },
                {
                    "id": 305,
                    "name": "Njaba (nnenasa)",
                    "state_id": 17
                },
                {
                    "id": 306,
                    "name": "Nkwerre",
                    "state_id": 17
                },
                {
                    "id": 307,
                    "name": "Nwangele (onu-nwangele amaigbo)",
                    "state_id": 17
                },
                {
                    "id": 308,
                    "name": "Obowo (otoko)",
                    "state_id": 17
                },
                {
                    "id": 309,
                    "name": "Oguta (oguta)",
                    "state_id": 17
                },
                {
                    "id": 310,
                    "name": "Ohaji\/egbema (mmahu-egbema)",
                    "state_id": 17
                },
                {
                    "id": 311,
                    "name": "Okigwe  (okigwe)",
                    "state_id": 17
                },
                {
                    "id": 312,
                    "name": "Onuimo (okwe)",
                    "state_id": 17
                },
                {
                    "id": 313,
                    "name": "Orlu",
                    "state_id": 17
                },
                {
                    "id": 314,
                    "name": "Orsu (awo idemili)",
                    "state_id": 17
                },
                {
                    "id": 315,
                    "name": "Oru west (mgbidi)",
                    "state_id": 17
                },
                {
                    "id": 316,
                    "name": "Oru-east",
                    "state_id": 17
                },
                {
                    "id": 317,
                    "name": "Owerri north (orie uratta)",
                    "state_id": 17
                },
                {
                    "id": 318,
                    "name": "Owerri urban (owerri)",
                    "state_id": 17
                },
                {
                    "id": 319,
                    "name": "Owerri west (umuguma)",
                    "state_id": 17
                }
            ]
        },
        {
            "id": 18,
            "name": "Jigawa",
            "lgas": [
                {
                    "id": 320,
                    "name": "Auyo",
                    "state_id": 18
                },
                {
                    "id": 321,
                    "name": "Babura",
                    "state_id": 18
                },
                {
                    "id": 322,
                    "name": "Birnin kudu",
                    "state_id": 18
                },
                {
                    "id": 323,
                    "name": "Birniwa",
                    "state_id": 18
                },
                {
                    "id": 324,
                    "name": "Buji",
                    "state_id": 18
                },
                {
                    "id": 325,
                    "name": "Dutse",
                    "state_id": 18
                },
                {
                    "id": 326,
                    "name": "Gagarawa",
                    "state_id": 18
                },
                {
                    "id": 327,
                    "name": "Garki",
                    "state_id": 18
                },
                {
                    "id": 328,
                    "name": "Gumel",
                    "state_id": 18
                },
                {
                    "id": 329,
                    "name": "Guri",
                    "state_id": 18
                },
                {
                    "id": 330,
                    "name": "Gwaram",
                    "state_id": 18
                },
                {
                    "id": 331,
                    "name": "Gwiwa",
                    "state_id": 18
                },
                {
                    "id": 332,
                    "name": "Hadejia",
                    "state_id": 18
                },
                {
                    "id": 333,
                    "name": "Jahun",
                    "state_id": 18
                },
                {
                    "id": 334,
                    "name": "Kafin hausa",
                    "state_id": 18
                },
                {
                    "id": 335,
                    "name": "Kaugama",
                    "state_id": 18
                },
                {
                    "id": 336,
                    "name": "Kazaure",
                    "state_id": 18
                },
                {
                    "id": 337,
                    "name": "Kirika samma",
                    "state_id": 18
                },
                {
                    "id": 338,
                    "name": "Kiyawa",
                    "state_id": 18
                },
                {
                    "id": 339,
                    "name": "Maigatari",
                    "state_id": 18
                },
                {
                    "id": 340,
                    "name": "Malam madori",
                    "state_id": 18
                },
                {
                    "id": 341,
                    "name": "Miga",
                    "state_id": 18
                },
                {
                    "id": 342,
                    "name": "Ringim",
                    "state_id": 18
                },
                {
                    "id": 343,
                    "name": "Roni",
                    "state_id": 18
                },
                {
                    "id": 344,
                    "name": "Sule-tankarkar",
                    "state_id": 18
                },
                {
                    "id": 345,
                    "name": "Taura",
                    "state_id": 18
                },
                {
                    "id": 346,
                    "name": "Yankwashi",
                    "state_id": 18
                }
            ]
        },
        {
            "id": 19,
            "name": "Kaduna",
            "lgas": [
                {
                    "id": 347,
                    "name": "Birnin gwari",
                    "state_id": 19
                },
                {
                    "id": 348,
                    "name": "Chikun",
                    "state_id": 19
                },
                {
                    "id": 349,
                    "name": "Giwa",
                    "state_id": 19
                },
                {
                    "id": 350,
                    "name": "Igabi",
                    "state_id": 19
                },
                {
                    "id": 351,
                    "name": "Ikara",
                    "state_id": 19
                },
                {
                    "id": 352,
                    "name": "Jaba",
                    "state_id": 19
                },
                {
                    "id": 353,
                    "name": "Jema'a",
                    "state_id": 19
                },
                {
                    "id": 354,
                    "name": "Kachia",
                    "state_id": 19
                },
                {
                    "id": 355,
                    "name": "Kaduna north",
                    "state_id": 19
                },
                {
                    "id": 356,
                    "name": "Kaduna south",
                    "state_id": 19
                },
                {
                    "id": 357,
                    "name": "Kagarko",
                    "state_id": 19
                },
                {
                    "id": 358,
                    "name": "Kajuru",
                    "state_id": 19
                },
                {
                    "id": 359,
                    "name": "Kaura",
                    "state_id": 19
                },
                {
                    "id": 360,
                    "name": "Kauru",
                    "state_id": 19
                },
                {
                    "id": 361,
                    "name": "Kubau",
                    "state_id": 19
                },
                {
                    "id": 362,
                    "name": "Kudan",
                    "state_id": 19
                },
                {
                    "id": 363,
                    "name": "Lere",
                    "state_id": 19
                },
                {
                    "id": 364,
                    "name": "Makarfi",
                    "state_id": 19
                },
                {
                    "id": 365,
                    "name": "Sabon gari",
                    "state_id": 19
                },
                {
                    "id": 366,
                    "name": "Sanga",
                    "state_id": 19
                },
                {
                    "id": 367,
                    "name": "Soba",
                    "state_id": 19
                },
                {
                    "id": 368,
                    "name": "Zangon kataf",
                    "state_id": 19
                },
                {
                    "id": 369,
                    "name": "Zaria",
                    "state_id": 19
                }
            ]
        },
        {
            "id": 20,
            "name": "Kano",
            "lgas": [
                {
                    "id": 370,
                    "name": "Ajingi",
                    "state_id": 20
                },
                {
                    "id": 371,
                    "name": "Albasu",
                    "state_id": 20
                },
                {
                    "id": 372,
                    "name": "Bagwai",
                    "state_id": 20
                },
                {
                    "id": 373,
                    "name": "Bebeji",
                    "state_id": 20
                },
                {
                    "id": 374,
                    "name": "Bichi",
                    "state_id": 20
                },
                {
                    "id": 375,
                    "name": "Bunkure",
                    "state_id": 20
                },
                {
                    "id": 376,
                    "name": "Dala",
                    "state_id": 20
                },
                {
                    "id": 377,
                    "name": "Danbata",
                    "state_id": 20
                },
                {
                    "id": 378,
                    "name": "Dawaki kudu",
                    "state_id": 20
                },
                {
                    "id": 379,
                    "name": "Dawaki tofa",
                    "state_id": 20
                },
                {
                    "id": 380,
                    "name": "Doguwa",
                    "state_id": 20
                },
                {
                    "id": 381,
                    "name": "Fagge",
                    "state_id": 20
                },
                {
                    "id": 382,
                    "name": "Gabasawa",
                    "state_id": 20
                },
                {
                    "id": 383,
                    "name": "Garko",
                    "state_id": 20
                },
                {
                    "id": 384,
                    "name": "Garun malam",
                    "state_id": 20
                },
                {
                    "id": 385,
                    "name": "Gaya",
                    "state_id": 20
                },
                {
                    "id": 386,
                    "name": "Gezawa",
                    "state_id": 20
                },
                {
                    "id": 387,
                    "name": "Gwale",
                    "state_id": 20
                },
                {
                    "id": 388,
                    "name": "Gwarzo",
                    "state_id": 20
                },
                {
                    "id": 389,
                    "name": "Kabo",
                    "state_id": 20
                },
                {
                    "id": 390,
                    "name": "Kano municipal",
                    "state_id": 20
                },
                {
                    "id": 391,
                    "name": "Karaye",
                    "state_id": 20
                },
                {
                    "id": 392,
                    "name": "Kibiya",
                    "state_id": 20
                },
                {
                    "id": 393,
                    "name": "Kiru",
                    "state_id": 20
                },
                {
                    "id": 394,
                    "name": "Kumbotso",
                    "state_id": 20
                },
                {
                    "id": 395,
                    "name": "Kunchi",
                    "state_id": 20
                },
                {
                    "id": 396,
                    "name": "Kura",
                    "state_id": 20
                },
                {
                    "id": 397,
                    "name": "Madobi",
                    "state_id": 20
                },
                {
                    "id": 398,
                    "name": "Makoda",
                    "state_id": 20
                },
                {
                    "id": 399,
                    "name": "Minjibir",
                    "state_id": 20
                },
                {
                    "id": 400,
                    "name": "Nasarawa",
                    "state_id": 20
                },
                {
                    "id": 401,
                    "name": "Rano",
                    "state_id": 20
                },
                {
                    "id": 402,
                    "name": "Rimin gado",
                    "state_id": 20
                },
                {
                    "id": 403,
                    "name": "Rogo",
                    "state_id": 20
                },
                {
                    "id": 404,
                    "name": "Shanono",
                    "state_id": 20
                },
                {
                    "id": 405,
                    "name": "Sumaila",
                    "state_id": 20
                },
                {
                    "id": 406,
                    "name": "Takai",
                    "state_id": 20
                },
                {
                    "id": 407,
                    "name": "Tarauni",
                    "state_id": 20
                },
                {
                    "id": 408,
                    "name": "Tofa",
                    "state_id": 20
                },
                {
                    "id": 409,
                    "name": "Tsanyawa",
                    "state_id": 20
                },
                {
                    "id": 410,
                    "name": "Tudun wada",
                    "state_id": 20
                },
                {
                    "id": 411,
                    "name": "Ungogo",
                    "state_id": 20
                },
                {
                    "id": 412,
                    "name": "Warawa",
                    "state_id": 20
                },
                {
                    "id": 413,
                    "name": "Wudil",
                    "state_id": 20
                }
            ]
        },
        {
            "id": 21,
            "name": "Katsina",
            "lgas": [
                {
                    "id": 414,
                    "name": "Bakori",
                    "state_id": 21
                },
                {
                    "id": 415,
                    "name": "Batagarawa",
                    "state_id": 21
                },
                {
                    "id": 416,
                    "name": "Batsari",
                    "state_id": 21
                },
                {
                    "id": 417,
                    "name": "Baure",
                    "state_id": 21
                },
                {
                    "id": 418,
                    "name": "Bindawa",
                    "state_id": 21
                },
                {
                    "id": 419,
                    "name": "Charanchi",
                    "state_id": 21
                },
                {
                    "id": 420,
                    "name": "Dan musa",
                    "state_id": 21
                },
                {
                    "id": 421,
                    "name": "Dandume",
                    "state_id": 21
                },
                {
                    "id": 422,
                    "name": "Danja",
                    "state_id": 21
                },
                {
                    "id": 423,
                    "name": "Daura",
                    "state_id": 21
                },
                {
                    "id": 424,
                    "name": "Dutsi",
                    "state_id": 21
                },
                {
                    "id": 425,
                    "name": "Dutsin-ma",
                    "state_id": 21
                },
                {
                    "id": 426,
                    "name": "Faskari",
                    "state_id": 21
                },
                {
                    "id": 427,
                    "name": "Funtua",
                    "state_id": 21
                },
                {
                    "id": 428,
                    "name": "Ingawa",
                    "state_id": 21
                },
                {
                    "id": 429,
                    "name": "Jibia",
                    "state_id": 21
                },
                {
                    "id": 430,
                    "name": "Kafur",
                    "state_id": 21
                },
                {
                    "id": 431,
                    "name": "Kaita",
                    "state_id": 21
                },
                {
                    "id": 432,
                    "name": "Kankara",
                    "state_id": 21
                },
                {
                    "id": 433,
                    "name": "Kankia",
                    "state_id": 21
                },
                {
                    "id": 434,
                    "name": "Katsina",
                    "state_id": 21
                },
                {
                    "id": 435,
                    "name": "Kurfi",
                    "state_id": 21
                },
                {
                    "id": 436,
                    "name": "Kusada",
                    "state_id": 21
                },
                {
                    "id": 437,
                    "name": "Mai'adua",
                    "state_id": 21
                },
                {
                    "id": 438,
                    "name": "Malufashi",
                    "state_id": 21
                },
                {
                    "id": 439,
                    "name": "Mani",
                    "state_id": 21
                },
                {
                    "id": 440,
                    "name": "Mashi",
                    "state_id": 21
                },
                {
                    "id": 441,
                    "name": "Matazu",
                    "state_id": 21
                },
                {
                    "id": 442,
                    "name": "Musawa",
                    "state_id": 21
                },
                {
                    "id": 443,
                    "name": "Rimi",
                    "state_id": 21
                },
                {
                    "id": 444,
                    "name": "Sabuwa",
                    "state_id": 21
                },
                {
                    "id": 445,
                    "name": "Safana",
                    "state_id": 21
                },
                {
                    "id": 446,
                    "name": "Sandamu",
                    "state_id": 21
                },
                {
                    "id": 447,
                    "name": "Zango",
                    "state_id": 21
                }
            ]
        },
        {
            "id": 22,
            "name": "Kebbi",
            "lgas": [
                {
                    "id": 448,
                    "name": "Aliero",
                    "state_id": 22
                },
                {
                    "id": 449,
                    "name": "Arewa",
                    "state_id": 22
                },
                {
                    "id": 450,
                    "name": "Argungu",
                    "state_id": 22
                },
                {
                    "id": 451,
                    "name": "Augie",
                    "state_id": 22
                },
                {
                    "id": 452,
                    "name": "Bagudo",
                    "state_id": 22
                },
                {
                    "id": 453,
                    "name": "Birnin kebbi",
                    "state_id": 22
                },
                {
                    "id": 454,
                    "name": "Bunza",
                    "state_id": 22
                },
                {
                    "id": 455,
                    "name": "Dandi",
                    "state_id": 22
                },
                {
                    "id": 456,
                    "name": "Fakai",
                    "state_id": 22
                },
                {
                    "id": 457,
                    "name": "Gwandu",
                    "state_id": 22
                },
                {
                    "id": 458,
                    "name": "Jega",
                    "state_id": 22
                },
                {
                    "id": 459,
                    "name": "Kalgo",
                    "state_id": 22
                },
                {
                    "id": 460,
                    "name": "Koko\/besse",
                    "state_id": 22
                },
                {
                    "id": 461,
                    "name": "Maiyama",
                    "state_id": 22
                },
                {
                    "id": 462,
                    "name": "Ngaski",
                    "state_id": 22
                },
                {
                    "id": 463,
                    "name": "Sakaba",
                    "state_id": 22
                },
                {
                    "id": 464,
                    "name": "Shanga",
                    "state_id": 22
                },
                {
                    "id": 465,
                    "name": "Suru",
                    "state_id": 22
                },
                {
                    "id": 466,
                    "name": "Wasagu\/danko",
                    "state_id": 22
                },
                {
                    "id": 467,
                    "name": "Yauri",
                    "state_id": 22
                },
                {
                    "id": 468,
                    "name": "Zuru",
                    "state_id": 22
                }
            ]
        },
        {
            "id": 23,
            "name": "Kogi",
            "lgas": [
                {
                    "id": 469,
                    "name": "Adavi",
                    "state_id": 23
                },
                {
                    "id": 470,
                    "name": "Ajaokuta",
                    "state_id": 23
                },
                {
                    "id": 471,
                    "name": "Ankpa",
                    "state_id": 23
                },
                {
                    "id": 472,
                    "name": "Bassa",
                    "state_id": 23
                },
                {
                    "id": 473,
                    "name": "Dekina",
                    "state_id": 23
                },
                {
                    "id": 474,
                    "name": "Ibaji",
                    "state_id": 23
                },
                {
                    "id": 475,
                    "name": "Idah",
                    "state_id": 23
                },
                {
                    "id": 476,
                    "name": "Igalamela\/odolu",
                    "state_id": 23
                },
                {
                    "id": 477,
                    "name": "Ijumu",
                    "state_id": 23
                },
                {
                    "id": 478,
                    "name": "Kabba\/bunu",
                    "state_id": 23
                },
                {
                    "id": 479,
                    "name": "Kogi . k. k.",
                    "state_id": 23
                },
                {
                    "id": 480,
                    "name": "Lokoja",
                    "state_id": 23
                },
                {
                    "id": 481,
                    "name": "Mopa moro",
                    "state_id": 23
                },
                {
                    "id": 482,
                    "name": "Ofu",
                    "state_id": 23
                },
                {
                    "id": 483,
                    "name": "Ogori mangogo",
                    "state_id": 23
                },
                {
                    "id": 484,
                    "name": "Okehi",
                    "state_id": 23
                },
                {
                    "id": 485,
                    "name": "Okene",
                    "state_id": 23
                },
                {
                    "id": 486,
                    "name": "Olamaboro",
                    "state_id": 23
                },
                {
                    "id": 487,
                    "name": "Omala",
                    "state_id": 23
                },
                {
                    "id": 488,
                    "name": "Yagba east",
                    "state_id": 23
                },
                {
                    "id": 489,
                    "name": "Yagba west",
                    "state_id": 23
                }
            ]
        },
        {
            "id": 24,
            "name": "Kwara",
            "lgas": [
                {
                    "id": 490,
                    "name": "Asa",
                    "state_id": 24
                },
                {
                    "id": 491,
                    "name": "Baruten",
                    "state_id": 24
                },
                {
                    "id": 492,
                    "name": "Edu",
                    "state_id": 24
                },
                {
                    "id": 493,
                    "name": "Ekiti",
                    "state_id": 24
                },
                {
                    "id": 494,
                    "name": "Ifelodun",
                    "state_id": 24
                },
                {
                    "id": 495,
                    "name": "Ilorin east",
                    "state_id": 24
                },
                {
                    "id": 496,
                    "name": "Ilorin-south",
                    "state_id": 24
                },
                {
                    "id": 497,
                    "name": "Ilorin-west",
                    "state_id": 24
                },
                {
                    "id": 498,
                    "name": "Irepodun",
                    "state_id": 24
                },
                {
                    "id": 499,
                    "name": "Isin",
                    "state_id": 24
                },
                {
                    "id": 500,
                    "name": "Kaiama",
                    "state_id": 24
                },
                {
                    "id": 501,
                    "name": "Moro",
                    "state_id": 24
                },
                {
                    "id": 502,
                    "name": "Offa",
                    "state_id": 24
                },
                {
                    "id": 503,
                    "name": "Oke - ero",
                    "state_id": 24
                },
                {
                    "id": 504,
                    "name": "Oyun",
                    "state_id": 24
                },
                {
                    "id": 505,
                    "name": "Patigi",
                    "state_id": 24
                }
            ]
        },
        {
            "id": 25,
            "name": "Lagos",
            "lgas": [
                {
                    "id": 506,
                    "name": "Agege",
                    "state_id": 25
                },
                {
                    "id": 507,
                    "name": "Ajeromi\/ifelodun",
                    "state_id": 25
                },
                {
                    "id": 508,
                    "name": "Alimosho",
                    "state_id": 25
                },
                {
                    "id": 509,
                    "name": "Amuwo-odofin",
                    "state_id": 25
                },
                {
                    "id": 510,
                    "name": "Apapa",
                    "state_id": 25
                },
                {
                    "id": 511,
                    "name": "Badagry",
                    "state_id": 25
                },
                {
                    "id": 512,
                    "name": "Epe",
                    "state_id": 25
                },
                {
                    "id": 513,
                    "name": "Eti-osa",
                    "state_id": 25
                },
                {
                    "id": 514,
                    "name": "Ibeju\/lekki",
                    "state_id": 25
                },
                {
                    "id": 515,
                    "name": "Ifako-ijaye",
                    "state_id": 25
                },
                {
                    "id": 516,
                    "name": "Ikeja",
                    "state_id": 25
                },
                {
                    "id": 517,
                    "name": "Ikorodu",
                    "state_id": 25
                },
                {
                    "id": 518,
                    "name": "Kosofe",
                    "state_id": 25
                },
                {
                    "id": 519,
                    "name": "Lagos island",
                    "state_id": 25
                },
                {
                    "id": 520,
                    "name": "Lagos mainland",
                    "state_id": 25
                },
                {
                    "id": 521,
                    "name": "Mushin",
                    "state_id": 25
                },
                {
                    "id": 522,
                    "name": "Ojo",
                    "state_id": 25
                },
                {
                    "id": 523,
                    "name": "Oshodi\/isolo",
                    "state_id": 25
                },
                {
                    "id": 524,
                    "name": "Somolu",
                    "state_id": 25
                },
                {
                    "id": 525,
                    "name": "Surulere",
                    "state_id": 25
                }
            ]
        },
        {
            "id": 26,
            "name": "Nasarawa",
            "lgas": [
                {
                    "id": 526,
                    "name": "Akwanga",
                    "state_id": 26
                },
                {
                    "id": 527,
                    "name": "Awe",
                    "state_id": 26
                },
                {
                    "id": 528,
                    "name": "Doma",
                    "state_id": 26
                },
                {
                    "id": 529,
                    "name": "Karu",
                    "state_id": 26
                },
                {
                    "id": 530,
                    "name": "Keana",
                    "state_id": 26
                },
                {
                    "id": 531,
                    "name": "Keffi",
                    "state_id": 26
                },
                {
                    "id": 532,
                    "name": "Kokona",
                    "state_id": 26
                },
                {
                    "id": 533,
                    "name": "Lafia",
                    "state_id": 26
                },
                {
                    "id": 534,
                    "name": "Nasarawa",
                    "state_id": 26
                },
                {
                    "id": 535,
                    "name": "Nasarawa eggon",
                    "state_id": 26
                },
                {
                    "id": 536,
                    "name": "Obi",
                    "state_id": 26
                },
                {
                    "id": 537,
                    "name": "Toto",
                    "state_id": 26
                },
                {
                    "id": 538,
                    "name": "Wamba",
                    "state_id": 26
                }
            ]
        },
        {
            "id": 27,
            "name": "Niger",
            "lgas": [
                {
                    "id": 539,
                    "name": "Agaie",
                    "state_id": 27
                },
                {
                    "id": 540,
                    "name": "Agwara",
                    "state_id": 27
                },
                {
                    "id": 541,
                    "name": "Bida",
                    "state_id": 27
                },
                {
                    "id": 542,
                    "name": "Borgu",
                    "state_id": 27
                },
                {
                    "id": 543,
                    "name": "Bosso",
                    "state_id": 27
                },
                {
                    "id": 544,
                    "name": "Chanchaga",
                    "state_id": 27
                },
                {
                    "id": 545,
                    "name": "Edatti",
                    "state_id": 27
                },
                {
                    "id": 546,
                    "name": "Gbako",
                    "state_id": 27
                },
                {
                    "id": 547,
                    "name": "Gurara",
                    "state_id": 27
                },
                {
                    "id": 548,
                    "name": "Katcha",
                    "state_id": 27
                },
                {
                    "id": 549,
                    "name": "Kontagora",
                    "state_id": 27
                },
                {
                    "id": 550,
                    "name": "Lapai",
                    "state_id": 27
                },
                {
                    "id": 551,
                    "name": "Lavun",
                    "state_id": 27
                },
                {
                    "id": 552,
                    "name": "Magama",
                    "state_id": 27
                },
                {
                    "id": 553,
                    "name": "Mariga",
                    "state_id": 27
                },
                {
                    "id": 554,
                    "name": "Mashegu",
                    "state_id": 27
                },
                {
                    "id": 555,
                    "name": "Mokwa",
                    "state_id": 27
                },
                {
                    "id": 556,
                    "name": "Munya",
                    "state_id": 27
                },
                {
                    "id": 557,
                    "name": "Paikoro",
                    "state_id": 27
                },
                {
                    "id": 558,
                    "name": "Rafi",
                    "state_id": 27
                },
                {
                    "id": 559,
                    "name": "Rijau",
                    "state_id": 27
                },
                {
                    "id": 560,
                    "name": "Shiroro",
                    "state_id": 27
                },
                {
                    "id": 561,
                    "name": "Suleja",
                    "state_id": 27
                },
                {
                    "id": 562,
                    "name": "Tafa",
                    "state_id": 27
                },
                {
                    "id": 563,
                    "name": "Wushishi",
                    "state_id": 27
                }
            ]
        },
        {
            "id": 28,
            "name": "Ogun",
            "lgas": [
                {
                    "id": 564,
                    "name": "Abeokuta north",
                    "state_id": 28
                },
                {
                    "id": 565,
                    "name": "Abeokuta south",
                    "state_id": 28
                },
                {
                    "id": 566,
                    "name": "Ado odo-ota",
                    "state_id": 28
                },
                {
                    "id": 567,
                    "name": "Egbado north",
                    "state_id": 28
                },
                {
                    "id": 568,
                    "name": "Egbado south",
                    "state_id": 28
                },
                {
                    "id": 569,
                    "name": "Ewekoro",
                    "state_id": 28
                },
                {
                    "id": 570,
                    "name": "Ifo",
                    "state_id": 28
                },
                {
                    "id": 571,
                    "name": "Ijebu east",
                    "state_id": 28
                },
                {
                    "id": 572,
                    "name": "Ijebu north",
                    "state_id": 28
                },
                {
                    "id": 573,
                    "name": "Ijebu north east",
                    "state_id": 28
                },
                {
                    "id": 574,
                    "name": "Ijebu ode",
                    "state_id": 28
                },
                {
                    "id": 575,
                    "name": "Ikenne",
                    "state_id": 28
                },
                {
                    "id": 576,
                    "name": "Imeko\/afon",
                    "state_id": 28
                },
                {
                    "id": 577,
                    "name": "Ipokia",
                    "state_id": 28
                },
                {
                    "id": 578,
                    "name": "Obafemi\/owode",
                    "state_id": 28
                },
                {
                    "id": 579,
                    "name": "Odeda",
                    "state_id": 28
                },
                {
                    "id": 580,
                    "name": "Odogbolu",
                    "state_id": 28
                },
                {
                    "id": 581,
                    "name": "Ogun water side",
                    "state_id": 28
                },
                {
                    "id": 582,
                    "name": "Remo north",
                    "state_id": 28
                },
                {
                    "id": 583,
                    "name": "Sagamu",
                    "state_id": 28
                }
            ]
        },
        {
            "id": 29,
            "name": "Ondo",
            "lgas": [
                {
                    "id": 584,
                    "name": "Akoko north east",
                    "state_id": 29
                },
                {
                    "id": 585,
                    "name": "Akoko north west",
                    "state_id": 29
                },
                {
                    "id": 586,
                    "name": "Akoko south east",
                    "state_id": 29
                },
                {
                    "id": 587,
                    "name": "Akoko south west",
                    "state_id": 29
                },
                {
                    "id": 588,
                    "name": "Akure north",
                    "state_id": 29
                },
                {
                    "id": 589,
                    "name": "Akure south",
                    "state_id": 29
                },
                {
                    "id": 590,
                    "name": "Ese-odo",
                    "state_id": 29
                },
                {
                    "id": 591,
                    "name": "Idanre",
                    "state_id": 29
                },
                {
                    "id": 592,
                    "name": "Ifedore",
                    "state_id": 29
                },
                {
                    "id": 593,
                    "name": "Ilaje",
                    "state_id": 29
                },
                {
                    "id": 594,
                    "name": "Ileoluji\/okeigbo",
                    "state_id": 29
                },
                {
                    "id": 595,
                    "name": "Irele",
                    "state_id": 29
                },
                {
                    "id": 596,
                    "name": "Odigbo",
                    "state_id": 29
                },
                {
                    "id": 597,
                    "name": "Okitipupa",
                    "state_id": 29
                },
                {
                    "id": 598,
                    "name": "Ondo east",
                    "state_id": 29
                },
                {
                    "id": 599,
                    "name": "Ondo west",
                    "state_id": 29
                },
                {
                    "id": 600,
                    "name": "Ose",
                    "state_id": 29
                },
                {
                    "id": 601,
                    "name": "Owo",
                    "state_id": 29
                }
            ]
        },
        {
            "id": 30,
            "name": "Osun",
            "lgas": [
                {
                    "id": 602,
                    "name": "Atakumosa east",
                    "state_id": 30
                },
                {
                    "id": 603,
                    "name": "Atakumosa west",
                    "state_id": 30
                },
                {
                    "id": 604,
                    "name": "Ayedaade",
                    "state_id": 30
                },
                {
                    "id": 605,
                    "name": "Ayedire",
                    "state_id": 30
                },
                {
                    "id": 606,
                    "name": "Boluwaduro",
                    "state_id": 30
                },
                {
                    "id": 607,
                    "name": "Boripe",
                    "state_id": 30
                },
                {
                    "id": 608,
                    "name": "Ede north",
                    "state_id": 30
                },
                {
                    "id": 609,
                    "name": "Ede south",
                    "state_id": 30
                },
                {
                    "id": 610,
                    "name": "Egbedore",
                    "state_id": 30
                },
                {
                    "id": 611,
                    "name": "Ejigbo",
                    "state_id": 30
                },
                {
                    "id": 612,
                    "name": "Ife central",
                    "state_id": 30
                },
                {
                    "id": 613,
                    "name": "Ife east",
                    "state_id": 30
                },
                {
                    "id": 614,
                    "name": "Ife north",
                    "state_id": 30
                },
                {
                    "id": 615,
                    "name": "Ife south",
                    "state_id": 30
                },
                {
                    "id": 616,
                    "name": "Ifedayo",
                    "state_id": 30
                },
                {
                    "id": 617,
                    "name": "Ifelodun",
                    "state_id": 30
                },
                {
                    "id": 618,
                    "name": "Ila",
                    "state_id": 30
                },
                {
                    "id": 619,
                    "name": "Ilesa east",
                    "state_id": 30
                },
                {
                    "id": 620,
                    "name": "Ilesa west",
                    "state_id": 30
                },
                {
                    "id": 621,
                    "name": "Irepodun",
                    "state_id": 30
                },
                {
                    "id": 622,
                    "name": "Irewole",
                    "state_id": 30
                },
                {
                    "id": 623,
                    "name": "Isokan",
                    "state_id": 30
                },
                {
                    "id": 624,
                    "name": "Iwo",
                    "state_id": 30
                },
                {
                    "id": 625,
                    "name": "Obokun",
                    "state_id": 30
                },
                {
                    "id": 626,
                    "name": "Odo-otin",
                    "state_id": 30
                },
                {
                    "id": 627,
                    "name": "Ola-oluwa",
                    "state_id": 30
                },
                {
                    "id": 628,
                    "name": "Olorunda",
                    "state_id": 30
                },
                {
                    "id": 629,
                    "name": "Oriade",
                    "state_id": 30
                },
                {
                    "id": 630,
                    "name": "Orolu",
                    "state_id": 30
                },
                {
                    "id": 631,
                    "name": "Osogbo",
                    "state_id": 30
                }
            ]
        },
        {
            "id": 31,
            "name": "Oyo",
            "lgas": [
                {
                    "id": 632,
                    "name": "Afijio",
                    "state_id": 31
                },
                {
                    "id": 633,
                    "name": "Akinyele",
                    "state_id": 31
                },
                {
                    "id": 634,
                    "name": "Atiba",
                    "state_id": 31
                },
                {
                    "id": 635,
                    "name": "Atisbo",
                    "state_id": 31
                },
                {
                    "id": 636,
                    "name": "Egbeda",
                    "state_id": 31
                },
                {
                    "id": 637,
                    "name": "Ibadan north",
                    "state_id": 31
                },
                {
                    "id": 638,
                    "name": "Ibadan north east",
                    "state_id": 31
                },
                {
                    "id": 639,
                    "name": "Ibadan north west",
                    "state_id": 31
                },
                {
                    "id": 640,
                    "name": "Ibadan south west",
                    "state_id": 31
                },
                {
                    "id": 641,
                    "name": "Ibadan south-east",
                    "state_id": 31
                },
                {
                    "id": 642,
                    "name": "Ibarapa central",
                    "state_id": 31
                },
                {
                    "id": 643,
                    "name": "Ibarapa east",
                    "state_id": 31
                },
                {
                    "id": 644,
                    "name": "Ibarapa north",
                    "state_id": 31
                },
                {
                    "id": 645,
                    "name": "Ido",
                    "state_id": 31
                },
                {
                    "id": 646,
                    "name": "Irepo",
                    "state_id": 31
                },
                {
                    "id": 647,
                    "name": "Iseyin",
                    "state_id": 31
                },
                {
                    "id": 648,
                    "name": "Itesiwaju",
                    "state_id": 31
                },
                {
                    "id": 649,
                    "name": "Iwajowa",
                    "state_id": 31
                },
                {
                    "id": 650,
                    "name": "Kajola",
                    "state_id": 31
                },
                {
                    "id": 651,
                    "name": "Lagelu",
                    "state_id": 31
                },
                {
                    "id": 652,
                    "name": "Ogbomoso north",
                    "state_id": 31
                },
                {
                    "id": 653,
                    "name": "Ogbomoso south",
                    "state_id": 31
                },
                {
                    "id": 654,
                    "name": "Ogo-oluwa",
                    "state_id": 31
                },
                {
                    "id": 655,
                    "name": "Olorunsogo",
                    "state_id": 31
                },
                {
                    "id": 656,
                    "name": "Oluyole",
                    "state_id": 31
                },
                {
                    "id": 657,
                    "name": "Ona-ara",
                    "state_id": 31
                },
                {
                    "id": 658,
                    "name": "Oorelope",
                    "state_id": 31
                },
                {
                    "id": 659,
                    "name": "Ori ire",
                    "state_id": 31
                },
                {
                    "id": 660,
                    "name": "Oyo east",
                    "state_id": 31
                },
                {
                    "id": 661,
                    "name": "Oyo west",
                    "state_id": 31
                },
                {
                    "id": 662,
                    "name": "Saki east",
                    "state_id": 31
                },
                {
                    "id": 663,
                    "name": "Saki west",
                    "state_id": 31
                },
                {
                    "id": 664,
                    "name": "Surulere",
                    "state_id": 31
                }
            ]
        },
        {
            "id": 32,
            "name": "Plateau",
            "lgas": [
                {
                    "id": 665,
                    "name": "Barikin ladi",
                    "state_id": 32
                },
                {
                    "id": 666,
                    "name": "Bassa",
                    "state_id": 32
                },
                {
                    "id": 667,
                    "name": "Bokkos",
                    "state_id": 32
                },
                {
                    "id": 668,
                    "name": "Jos east",
                    "state_id": 32
                },
                {
                    "id": 669,
                    "name": "Jos north",
                    "state_id": 32
                },
                {
                    "id": 670,
                    "name": "Jos south",
                    "state_id": 32
                },
                {
                    "id": 671,
                    "name": "Kanam",
                    "state_id": 32
                },
                {
                    "id": 672,
                    "name": "Kanke",
                    "state_id": 32
                },
                {
                    "id": 673,
                    "name": "Langtang north",
                    "state_id": 32
                },
                {
                    "id": 674,
                    "name": "Langtang south",
                    "state_id": 32
                },
                {
                    "id": 675,
                    "name": "Mangu",
                    "state_id": 32
                },
                {
                    "id": 676,
                    "name": "Mikang",
                    "state_id": 32
                },
                {
                    "id": 677,
                    "name": "Pankshin",
                    "state_id": 32
                },
                {
                    "id": 678,
                    "name": "Qua'an pan",
                    "state_id": 32
                },
                {
                    "id": 679,
                    "name": "Riyom",
                    "state_id": 32
                },
                {
                    "id": 680,
                    "name": "Shendam",
                    "state_id": 32
                },
                {
                    "id": 681,
                    "name": "Wase",
                    "state_id": 32
                }
            ]
        },
        {
            "id": 33,
            "name": "Rivers",
            "lgas": [
                {
                    "id": 682,
                    "name": "Abua-odual",
                    "state_id": 33
                },
                {
                    "id": 683,
                    "name": "Ahoada east",
                    "state_id": 33
                },
                {
                    "id": 684,
                    "name": "Ahoada west",
                    "state_id": 33
                },
                {
                    "id": 685,
                    "name": "Akuku toru",
                    "state_id": 33
                },
                {
                    "id": 686,
                    "name": "Andoni",
                    "state_id": 33
                },
                {
                    "id": 687,
                    "name": "Asari-toru",
                    "state_id": 33
                },
                {
                    "id": 688,
                    "name": "Bonny",
                    "state_id": 33
                },
                {
                    "id": 689,
                    "name": "Degema",
                    "state_id": 33
                },
                {
                    "id": 690,
                    "name": "Eleme",
                    "state_id": 33
                },
                {
                    "id": 691,
                    "name": "Emohua",
                    "state_id": 33
                },
                {
                    "id": 692,
                    "name": "Etche",
                    "state_id": 33
                },
                {
                    "id": 693,
                    "name": "Gokana",
                    "state_id": 33
                },
                {
                    "id": 694,
                    "name": "Ikwerre",
                    "state_id": 33
                },
                {
                    "id": 695,
                    "name": "Khana",
                    "state_id": 33
                },
                {
                    "id": 696,
                    "name": "Obio\/akpor",
                    "state_id": 33
                },
                {
                    "id": 697,
                    "name": "Ogba\/egbema\/ndoni",
                    "state_id": 33
                },
                {
                    "id": 698,
                    "name": "Ogu\/bolo",
                    "state_id": 33
                },
                {
                    "id": 699,
                    "name": "Okrika",
                    "state_id": 33
                },
                {
                    "id": 700,
                    "name": "Omuma",
                    "state_id": 33
                },
                {
                    "id": 701,
                    "name": "Opobo\/nekoro",
                    "state_id": 33
                },
                {
                    "id": 702,
                    "name": "Oyigbo",
                    "state_id": 33
                },
                {
                    "id": 703,
                    "name": "Port harcourt",
                    "state_id": 33
                },
                {
                    "id": 704,
                    "name": "Tai",
                    "state_id": 33
                }
            ]
        },
        {
            "id": 34,
            "name": "Sokoto",
            "lgas": [
                {
                    "id": 705,
                    "name": "Binji",
                    "state_id": 34
                },
                {
                    "id": 706,
                    "name": "Bodinga",
                    "state_id": 34
                },
                {
                    "id": 707,
                    "name": "Dange\/shuni",
                    "state_id": 34
                },
                {
                    "id": 708,
                    "name": "Gada",
                    "state_id": 34
                },
                {
                    "id": 709,
                    "name": "Goronyo",
                    "state_id": 34
                },
                {
                    "id": 710,
                    "name": "Gudu",
                    "state_id": 34
                },
                {
                    "id": 711,
                    "name": "Gwadabawa",
                    "state_id": 34
                },
                {
                    "id": 712,
                    "name": "Illela",
                    "state_id": 34
                },
                {
                    "id": 713,
                    "name": "Isa",
                    "state_id": 34
                },
                {
                    "id": 714,
                    "name": "Kebbe",
                    "state_id": 34
                },
                {
                    "id": 715,
                    "name": "Kware",
                    "state_id": 34
                },
                {
                    "id": 716,
                    "name": "Rabah",
                    "state_id": 34
                },
                {
                    "id": 717,
                    "name": "S\/birni",
                    "state_id": 34
                },
                {
                    "id": 718,
                    "name": "Shagari",
                    "state_id": 34
                },
                {
                    "id": 719,
                    "name": "Silame",
                    "state_id": 34
                },
                {
                    "id": 720,
                    "name": "Sokoto north",
                    "state_id": 34
                },
                {
                    "id": 721,
                    "name": "Sokoto south",
                    "state_id": 34
                },
                {
                    "id": 722,
                    "name": "Tambuwal",
                    "state_id": 34
                },
                {
                    "id": 723,
                    "name": "Tangaza",
                    "state_id": 34
                },
                {
                    "id": 724,
                    "name": "Tureta",
                    "state_id": 34
                },
                {
                    "id": 725,
                    "name": "Wamakko",
                    "state_id": 34
                },
                {
                    "id": 726,
                    "name": "Wurno",
                    "state_id": 34
                },
                {
                    "id": 727,
                    "name": "Yabo",
                    "state_id": 34
                }
            ]
        },
        {
            "id": 35,
            "name": "Taraba",
            "lgas": [
                {
                    "id": 728,
                    "name": "Ardo - kola",
                    "state_id": 35
                },
                {
                    "id": 729,
                    "name": "Bali",
                    "state_id": 35
                },
                {
                    "id": 730,
                    "name": "Donga",
                    "state_id": 35
                },
                {
                    "id": 731,
                    "name": "Gashaka",
                    "state_id": 35
                },
                {
                    "id": 732,
                    "name": "Gassol",
                    "state_id": 35
                },
                {
                    "id": 733,
                    "name": "Ibi",
                    "state_id": 35
                },
                {
                    "id": 734,
                    "name": "Jalingo",
                    "state_id": 35
                },
                {
                    "id": 735,
                    "name": "Karim-lamido",
                    "state_id": 35
                },
                {
                    "id": 736,
                    "name": "Kurmi",
                    "state_id": 35
                },
                {
                    "id": 737,
                    "name": "Lau",
                    "state_id": 35
                },
                {
                    "id": 738,
                    "name": "Sardauna",
                    "state_id": 35
                },
                {
                    "id": 739,
                    "name": "Takum",
                    "state_id": 35
                },
                {
                    "id": 740,
                    "name": "Ussa",
                    "state_id": 35
                },
                {
                    "id": 741,
                    "name": "Wukari",
                    "state_id": 35
                },
                {
                    "id": 742,
                    "name": "Yorro",
                    "state_id": 35
                },
                {
                    "id": 743,
                    "name": "Zing",
                    "state_id": 35
                }
            ]
        },
        {
            "id": 36,
            "name": "Yobe",
            "lgas": [
                {
                    "id": 744,
                    "name": "Bade",
                    "state_id": 36
                },
                {
                    "id": 745,
                    "name": "Bursari",
                    "state_id": 36
                },
                {
                    "id": 746,
                    "name": "Damaturu",
                    "state_id": 36
                },
                {
                    "id": 747,
                    "name": "Fika",
                    "state_id": 36
                },
                {
                    "id": 748,
                    "name": "Fune",
                    "state_id": 36
                },
                {
                    "id": 749,
                    "name": "Geidam",
                    "state_id": 36
                },
                {
                    "id": 750,
                    "name": "Gujba",
                    "state_id": 36
                },
                {
                    "id": 751,
                    "name": "Gulani",
                    "state_id": 36
                },
                {
                    "id": 752,
                    "name": "Jakusko",
                    "state_id": 36
                },
                {
                    "id": 753,
                    "name": "Karasawa",
                    "state_id": 36
                },
                {
                    "id": 754,
                    "name": "Machina",
                    "state_id": 36
                },
                {
                    "id": 755,
                    "name": "Nangere",
                    "state_id": 36
                },
                {
                    "id": 756,
                    "name": "Nguru",
                    "state_id": 36
                },
                {
                    "id": 757,
                    "name": "Potiskum",
                    "state_id": 36
                },
                {
                    "id": 758,
                    "name": "Tarmuwa",
                    "state_id": 36
                },
                {
                    "id": 759,
                    "name": "Yunusari",
                    "state_id": 36
                },
                {
                    "id": 760,
                    "name": "Yusufari",
                    "state_id": 36
                }
            ]
        },
        {
            "id": 37,
            "name": "Zamfara",
            "lgas": [
                {
                    "id": 761,
                    "name": "Anka",
                    "state_id": 37
                },
                {
                    "id": 762,
                    "name": "Bakura",
                    "state_id": 37
                },
                {
                    "id": 763,
                    "name": "Birnin magaji",
                    "state_id": 37
                },
                {
                    "id": 764,
                    "name": "Bukkuyum",
                    "state_id": 37
                },
                {
                    "id": 765,
                    "name": "Bungudu",
                    "state_id": 37
                },
                {
                    "id": 766,
                    "name": "Gummi",
                    "state_id": 37
                },
                {
                    "id": 767,
                    "name": "Gusau",
                    "state_id": 37
                },
                {
                    "id": 768,
                    "name": "Kaura namoda",
                    "state_id": 37
                },
                {
                    "id": 769,
                    "name": "Maradun",
                    "state_id": 37
                },
                {
                    "id": 770,
                    "name": "Maru",
                    "state_id": 37
                },
                {
                    "id": 771,
                    "name": "Shinkafi",
                    "state_id": 37
                },
                {
                    "id": 772,
                    "name": "Talata mafara",
                    "state_id": 37
                },
                {
                    "id": 773,
                    "name": "Tsafe",
                    "state_id": 37
                },
                {
                    "id": 774,
                    "name": "Zurmi",
                    "state_id": 37
                }
            ]
        }
    ]
}
```

### HTTP Request
`GET api/v1/states/lgas`

`HEAD api/v1/states/lgas`


<!-- END_e3a8359c2a2db1c2299bb91a0569b086 -->

<!-- START_997381b725042e68219808d260629b4b -->
## Show LGAs
All LGAs belonging to the specified State will be returned. Pass state id.

> Example request:

```bash
curl -X GET "https://http://allnigeria-api.herokuapp.com/api/v1/state/lgas/{state}" \
-H "Accept: application/json"
```

```javascript
var settings = {
    "async": true,
    "crossDomain": true,
    "url": "https://http://allnigeria-api.herokuapp.com/api/v1/state/lgas/{state}",
    "method": "GET",
    "headers": {
        "accept": "application/json"
    }
}

$.ajax(settings).done(function (response) {
    console.log(response);
});
```

> Example response:

```json
{
    "success": true,
    "message": "LGAs for Abia were found",
    "data": [
        {
            "id": 1,
            "name": "Aba north",
            "state_id": 1
        },
        {
            "id": 2,
            "name": "Aba south",
            "state_id": 1
        },
        {
            "id": 3,
            "name": "Arochukwu",
            "state_id": 1
        },
        {
            "id": 4,
            "name": "Bende",
            "state_id": 1
        },
        {
            "id": 5,
            "name": "Ikwuano",
            "state_id": 1
        },
        {
            "id": 6,
            "name": "Isiala ngwa north",
            "state_id": 1
        },
        {
            "id": 7,
            "name": "Isiala ngwa south",
            "state_id": 1
        },
        {
            "id": 8,
            "name": "Isuikwuato",
            "state_id": 1
        },
        {
            "id": 9,
            "name": "Obingwa",
            "state_id": 1
        },
        {
            "id": 10,
            "name": "Ohafia",
            "state_id": 1
        },
        {
            "id": 11,
            "name": "Osisioma",
            "state_id": 1
        },
        {
            "id": 12,
            "name": "Ugwunagbo",
            "state_id": 1
        },
        {
            "id": 13,
            "name": "Ukwa  west",
            "state_id": 1
        },
        {
            "id": 14,
            "name": "Ukwa east",
            "state_id": 1
        },
        {
            "id": 15,
            "name": "Umu - nneochi",
            "state_id": 1
        },
        {
            "id": 16,
            "name": "Umuahia  south",
            "state_id": 1
        },
        {
            "id": 17,
            "name": "Umuahia north",
            "state_id": 1
        }
    ]
}
```

### HTTP Request
`GET api/v1/state/lgas/{state}`

`HEAD api/v1/state/lgas/{state}`


<!-- END_997381b725042e68219808d260629b4b -->

<!-- START_af332325931a5890987ee5fb0f8d5a1f -->
## Show Wards
All Wards belonging to the specified LGA will be returned. Pass LGA id.

> Example request:

```bash
curl -X GET "https://http://allnigeria-api.herokuapp.com/api/v1/lga/wards/{lga}" \
-H "Accept: application/json"
```

```javascript
var settings = {
    "async": true,
    "crossDomain": true,
    "url": "https://http://allnigeria-api.herokuapp.com/api/v1/lga/wards/{lga}",
    "method": "GET",
    "headers": {
        "accept": "application/json"
    }
}

$.ajax(settings).done(function (response) {
    console.log(response);
});
```

> Example response:

```json
{
    "success": true,
    "message": "Wards for Aba north were found",
    "data": [
        {
            "id": 1,
            "name": "Ariaria market",
            "lga_id": 1
        },
        {
            "id": 2,
            "name": "Eziama",
            "lga_id": 1
        },
        {
            "id": 3,
            "name": "Industrial area",
            "lga_id": 1
        },
        {
            "id": 4,
            "name": "Ogbor i",
            "lga_id": 1
        },
        {
            "id": 5,
            "name": "Ogbor ii",
            "lga_id": 1
        },
        {
            "id": 6,
            "name": "Old aba gra",
            "lga_id": 1
        },
        {
            "id": 7,
            "name": "Osusu i",
            "lga_id": 1
        },
        {
            "id": 8,
            "name": "Osusu ii",
            "lga_id": 1
        },
        {
            "id": 9,
            "name": "St.eugenes by okigwe rd.",
            "lga_id": 1
        },
        {
            "id": 10,
            "name": "Umuogor",
            "lga_id": 1
        },
        {
            "id": 11,
            "name": "Umuola",
            "lga_id": 1
        },
        {
            "id": 12,
            "name": "Uratta",
            "lga_id": 1
        }
    ]
}
```

### HTTP Request
`GET api/v1/lga/wards/{lga}`

`HEAD api/v1/lga/wards/{lga}`


<!-- END_af332325931a5890987ee5fb0f8d5a1f -->

<!-- START_45740b9744eb036c0aedee2d4d26615d -->
## Show Units
All Polling Units belonging to the specified Ward will be returned. Pass Ward id.

> Example request:

```bash
curl -X GET "https://http://allnigeria-api.herokuapp.com/api/v1/ward/units/{ward}" \
-H "Accept: application/json"
```

```javascript
var settings = {
    "async": true,
    "crossDomain": true,
    "url": "https://http://allnigeria-api.herokuapp.com/api/v1/ward/units/{ward}",
    "method": "GET",
    "headers": {
        "accept": "application/json"
    }
}

$.ajax(settings).done(function (response) {
    console.log(response);
});
```

> Example response:

```json
{
    "success": true,
    "message": "Units for Ariaria market were found",
    "data": [
        {
            "id": 1,
            "name": "(48 Polling Booths )B.t.c-school premises i (PU: 01\/01\/09\/007)",
            "ward_id": 1
        },
        {
            "id": 2,
            "name": "B.t.c-school premises ii (PU: 01\/01\/09\/008)",
            "ward_id": 1
        },
        {
            "id": 3,
            "name": "B.t.c-school premises iii (PU: 01\/01\/09\/009)",
            "ward_id": 1
        },
        {
            "id": 4,
            "name": "B.t.c-school premises iv (PU: 01\/01\/09\/010)",
            "ward_id": 1
        },
        {
            "id": 5,
            "name": "B.t.c-school premises v (PU: 01\/01\/09\/011)",
            "ward_id": 1
        },
        {
            "id": 6,
            "name": "B.t.c-school premises vi (PU: 01\/01\/09\/012)",
            "ward_id": 1
        },
        {
            "id": 7,
            "name": "B.t.c-school premises vii (PU: 01\/01\/09\/013)",
            "ward_id": 1
        },
        {
            "id": 8,
            "name": "Eziobu prim school  - school premises iv (PU: 01\/01\/09\/029)",
            "ward_id": 1
        },
        {
            "id": 9,
            "name": "Eziobu prim school  - school premises v (PU: 01\/01\/09\/030)",
            "ward_id": 1
        },
        {
            "id": 10,
            "name": "Eziobu prim school  - school premises vi (PU: 01\/01\/09\/031)",
            "ward_id": 1
        },
        {
            "id": 11,
            "name": "Eziobu prim school  - school premises vii (PU: 01\/01\/09\/032)",
            "ward_id": 1
        },
        {
            "id": 12,
            "name": "Eziobu prim school - school  premises ii (PU: 01\/01\/09\/027)",
            "ward_id": 1
        },
        {
            "id": 13,
            "name": "Eziobu prim school - school premises iii (PU: 01\/01\/09\/028)",
            "ward_id": 1
        },
        {
            "id": 14,
            "name": "Eziobu prim school premises i (PU: 01\/01\/09\/026)",
            "ward_id": 1
        },
        {
            "id": 15,
            "name": "Fire service station premises i (PU: 01\/01\/09\/024)",
            "ward_id": 1
        },
        {
            "id": 16,
            "name": "Fire service station premises ii (PU: 01\/01\/09\/025)",
            "ward_id": 1
        },
        {
            "id": 17,
            "name": "Holy ghost comm.school  - school premises i (PU: 01\/01\/09\/039)",
            "ward_id": 1
        },
        {
            "id": 18,
            "name": "Holy ghost comm.school  - school premises ii (PU: 01\/01\/09\/040)",
            "ward_id": 1
        },
        {
            "id": 19,
            "name": "Holy ghost comm.school  - school premises iii (PU: 01\/01\/09\/041)",
            "ward_id": 1
        },
        {
            "id": 20,
            "name": "Holy ghost comm.school  - school premises iv (PU: 01\/01\/09\/042)",
            "ward_id": 1
        },
        {
            "id": 21,
            "name": "Holy ghost comm.school  - school premises v (PU: 01\/01\/09\/043)",
            "ward_id": 1
        },
        {
            "id": 22,
            "name": "Old internal revenue-premises i (PU: 01\/01\/09\/014)",
            "ward_id": 1
        },
        {
            "id": 23,
            "name": "Old internal revenue-premises ii (PU: 01\/01\/09\/015)",
            "ward_id": 1
        },
        {
            "id": 24,
            "name": "Old internal revenue-premises iii (PU: 01\/01\/09\/016)",
            "ward_id": 1
        },
        {
            "id": 25,
            "name": "Old internal revenue-premises iv (PU: 01\/01\/09\/017)",
            "ward_id": 1
        },
        {
            "id": 26,
            "name": "Old internal revenue-premises v (PU: 01\/01\/09\/018)",
            "ward_id": 1
        },
        {
            "id": 27,
            "name": "Old internal revenue-premises vi (PU: 01\/01\/09\/019)",
            "ward_id": 1
        },
        {
            "id": 28,
            "name": "Old internal revenue-premises vii (PU: 01\/01\/09\/020)",
            "ward_id": 1
        },
        {
            "id": 29,
            "name": "Osusu rd.prim.school-premises i (PU: 01\/01\/09\/001)",
            "ward_id": 1
        },
        {
            "id": 30,
            "name": "Osusu rd.prim.school-premises ii (PU: 01\/01\/09\/002)",
            "ward_id": 1
        },
        {
            "id": 31,
            "name": "Osusu rd.prim.school-premises iii (PU: 01\/01\/09\/003)",
            "ward_id": 1
        },
        {
            "id": 32,
            "name": "Osusu rd.prim.school-premises iv (PU: 01\/01\/09\/004)",
            "ward_id": 1
        },
        {
            "id": 33,
            "name": "Osusu rd.prim.school-premises v (PU: 01\/01\/09\/005)",
            "ward_id": 1
        },
        {
            "id": 34,
            "name": "Osusu rd.prim.school-premises vi (PU: 01\/01\/09\/006)",
            "ward_id": 1
        },
        {
            "id": 35,
            "name": "Osusu village hall - council hall i (PU: 01\/01\/09\/033)",
            "ward_id": 1
        },
        {
            "id": 36,
            "name": "Osusu village hall - council hall ii (PU: 01\/01\/09\/034)",
            "ward_id": 1
        },
        {
            "id": 37,
            "name": "Osusu village hall - council hall iii (PU: 01\/01\/09\/035)",
            "ward_id": 1
        },
        {
            "id": 38,
            "name": "Osusu village hall - council hall iv (PU: 01\/01\/09\/036)",
            "ward_id": 1
        },
        {
            "id": 39,
            "name": "Osusu village hall - council hall vi (PU: 01\/01\/09\/038)",
            "ward_id": 1
        },
        {
            "id": 40,
            "name": "Osusu village hall - council v (PU: 01\/01\/09\/037)",
            "ward_id": 1
        },
        {
            "id": 41,
            "name": "Rock family prim.\/nurs.school  - school premises i (PU: 01\/01\/09\/021)",
            "ward_id": 1
        },
        {
            "id": 42,
            "name": "Rock family prim.\/nurs.school  - school premises ii (PU: 01\/01\/09\/022)",
            "ward_id": 1
        },
        {
            "id": 43,
            "name": "Rock family prim.\/nurs.school  - school premises iii (PU: 01\/01\/09\/023)",
            "ward_id": 1
        },
        {
            "id": 44,
            "name": "Sacred heart college-school premises i (PU: 01\/01\/09\/044)",
            "ward_id": 1
        },
        {
            "id": 45,
            "name": "Sacred heart college-school premises ii (PU: 01\/01\/09\/045)",
            "ward_id": 1
        },
        {
            "id": 46,
            "name": "Sacred heart college-school premises iii (PU: 01\/01\/09\/046)",
            "ward_id": 1
        },
        {
            "id": 47,
            "name": "Sacred heart college-school premises iv (PU: 01\/01\/09\/047)",
            "ward_id": 1
        },
        {
            "id": 48,
            "name": "Sacred heart college-school premises v (PU: 01\/01\/09\/048)",
            "ward_id": 1
        }
    ]
}
```

### HTTP Request
`GET api/v1/ward/units/{ward}`

`HEAD api/v1/ward/units/{ward}`


<!-- END_45740b9744eb036c0aedee2d4d26615d -->

