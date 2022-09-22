POST /thirdpartyTransaction/${transactionRequestId}/approve

Request
```
{
    "authorizationResponse": {
      "responseType": "ACCEPTED",
      "signedPayload": {
        "signedPayloadType": "FIDO",
        "fidoSignedPayload": {
          "id": "45c-TkfkjQovQeAWmOy-RLBHEJ_e4jYzQYgD8VdbkePgM5d98BaAadadNYrknxgH0jQEON8zBydLgh1EqoC9DA",
          "rawId": "45c+TkfkjQovQeAWmOy+RLBHEJ/e4jYzQYgD8VdbkePgM5d98BaAadadNYrknxgH0jQEON8zBydLgh1EqoC9DA==",
          "response": {
            "authenticatorData": "SZYN5YgOjGh0NBcPZHZgW4/krrmihjLHmVzzuoMdl2MBAAAACA==",
            "clientDataJSON": "eyJ0eXBlIjoid2ViYXV0aG4uZ2V0IiwiY2hhbGxlbmdlIjoiQUFBQUFBQUFBQUFBQUFBQUFBRUNBdyIsIm9yaWdpbiI6Imh0dHA6Ly9sb2NhbGhvc3Q6NDIxODEiLCJjcm9zc09yaWdpbiI6ZmFsc2UsIm90aGVyX2tleXNfY2FuX2JlX2FkZGVkX2hlcmUiOiJkbyBub3QgY29tcGFyZSBjbGllbnREYXRhSlNPTiBhZ2FpbnN0IGEgdGVtcGxhdGUuIFNlZSBodHRwczovL2dvby5nbC95YWJQZXgifQ==",
            "signature": "MEUCIDcJRBu5aOLJVc/sPyECmYi23w8xF35n3RNhyUNVwQ2nAiEA+Lnd8dBn06OKkEgAq00BVbmH87ybQHfXlf1Y4RJqwQ8="
          },
          "type": "public-key"
        }
      }
    }
}
```

Response
```
{
    "transactionStatus": {
      "transactionId": "c51ec534-ee48-4575-b6a9-ead2955b8069",
      "transactionRequestState": "ACCEPTED",
      "transactionState": "COMPLETED"
    },
    "currentState": "transactionStatusReceived"
}
```