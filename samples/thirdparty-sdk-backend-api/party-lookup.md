POST /thirdpartyTransaction/partyLookup

Request
```
{
    "transactionRequestId": "b51ec534-ee48-4575-b6a9-ead2955b8069",
    "payee": {
      "partyIdType": "MSISDN",
      "partyIdentifier": "9876543210"
    }
}
```

Response
```
{
    "party": {
      "partyIdInfo": {
        "partyIdType": "MSISDN",
        "partyIdentifier": "9876543210",
        "fspId": "pispA"
      },
      "merchantClassificationCode": "4321",
      "name": "Justin Trudeau",
      "personalInfo": {
        "complexName": {
          "firstName": "Justin",
          "middleName": "Pierre",
          "lastName": "Trudeau"
        },
        "dateOfBirth": "1980-01-01"
      }
    },
    "currentState": "partyLookupSuccess"
}
```

{
  "status": 200,
  "statusText": "OK",
  "body": {
    "party": {
      "partyIdInfo": {
        "partyIdType": "MSISDN",
        "partyIdentifier": "9876543210",
        "fspId": "pispA"
      },
      "merchantClassificationCode": "4321",
      "name": "Justin Trudeau",
      "personalInfo": {
        "complexName": {
          "firstName": "Justin",
          "middleName": "Pierre",
          "lastName": "Trudeau"
        },
        "dateOfBirth": "1980-01-01"
      }
    },
    "currentState": "partyLookupSuccess"
  },
  "headers": {
    "content-type": "application/json; charset=utf-8",
    "cache-control": "no-cache",
    "content-length": "317",
    "date": "Fri, 23 Sep 2022 05:12:48 GMT",
    "connection": "keep-alive",
    "keep-alive": "timeout=5"
  }
}