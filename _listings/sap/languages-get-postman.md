{
  "info": {
    "name": "SAP Translation Hub Languages that SAP Translation Hub supports.",
    "_postman_id": "1e8ccd16-9281-49fe-973b-f5b7f23a2639",
    "description": "Returns a list of the languages that SAP Translation Hub supports. You can also check whether a particualr language is available in SAP Translation Hub.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "SAP",
      "item": [
        {
          "id": "4a29be85-b2d3-4502-b051-63a142c33ec4",
          "name": "sap-product-terminology-is-organized-by-domains-domains-are-used-in-the-translation-process-to-deter",
          "request": {
            "url": "http://sandbox.api.sap.com/translationhub/api/v1/domains?onlyGroups=%7B%7D&search=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Content-Type",
                "value": "{}",
                "description": "Specifies the nature of the data in the body so that the receiving agent can process the data accordingly",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "SAP product terminology is organized by domains. Domains are used in the translation process to determine the correct terminology for a given application. <br> This resource returns a list of the domains and domain groups that are available in SAP Translation Hub.<br> You can combine the domain resource with the translation resource to more accurately reflect the subject area of your texts."
          },
          "response": [
            {
              "status": "Successful response",
              "code": 200,
              "name": "Response_200",
              "id": "66ab822a-658e-418d-971c-a2a558d95695"
            }
          ]
        }
      ]
    },
    {
      "name": "Languages",
      "item": [
        {
          "id": "881c9b30-8692-48c4-b43a-ce99e9e20b42",
          "name": "returns-a-list-of-the-languages-that-sap-translation-hub-supports-you-can-also-check-whether-a-parti",
          "request": {
            "url": "http://sandbox.api.sap.com/translationhub/api/v1/languages?search=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Content-Type",
                "value": "{}",
                "description": "Specifies the nature of the data in the body so that the receiving agent can process the data accordingly",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of the languages that SAP Translation Hub supports. You can also check whether a particualr language is available in SAP Translation Hub."
          },
          "response": [
            {
              "status": "Successful response",
              "code": 200,
              "name": "Response_200",
              "id": "279059ce-ce4c-4487-b732-23dfc0b1832a"
            }
          ]
        }
      ]
    }
  ]
}