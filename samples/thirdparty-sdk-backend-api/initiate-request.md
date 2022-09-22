POST /thirdpartyTransaction/${transactionRequestId}/initiate

Request
```
{
    "payee": {
      "partyIdInfo": {
        "partyIdType": "MSISDN",
        "partyIdentifier": "9876543210",
        "fspId": "dfspb"
      }
    },
    "payer": {
      "partyIdType": "THIRD_PARTY_LINK",
      "partyIdentifier": "1234567890",
      "fspId": "dfspa"
    },
    "amountType": "SEND",
    "amount": {
      "amount": "100",
      "currency": "USD"
    },
    "transactionType": {
      "scenario": "TRANSFER",
      "initiator": "PAYER",
      "initiatorType": "CONSUMER"
    },
    "expiration": "2020-07-15T22:17:28.985-01:00"
}
```

Response
```
{
    "authorization": {
      "authorizationRequestId": "5f8ee7f9-290f-4e03-ae1c-1e81ecf398df",
      "transactionRequestId": "b51ec534-ee48-4575-b6a9-ead2955b8069",
      "challenge": "<base64 encoded binary - the encoded challenge>",
      "transferAmount": {
        "amount": "10",
        "currency": "EUR"
      },
      "payeeReceiveAmount": {
        "amount": "10",
        "currency": "EUR"
      },
      "fees": {
        "amount": "0",
        "currency": "EUR"
      },
      "payee": {
        "partyIdInfo": {
          "partyIdType": "MSISDN",
          "partyIdentifier": "9876543210",
          "fspId": "dfspb"
        }
      },
      "payer": {
        "partyIdType": "THIRD_PARTY_LINK",
        "partyIdentifier": "qwerty-123456",
        "fspId": "dfspa"
      },
      "transactionType": {
        "scenario": "TRANSFER",
        "initiator": "PAYER",
        "initiatorType": "CONSUMER"
      },
      "expiration": "2020-06-15T12:00:00.000Z"
    },
    "currentState": "authorizationReceived"
}
```