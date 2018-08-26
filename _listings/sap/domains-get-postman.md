{
  "info": {
    "name": "SAP Translation Hub SAP product domains",
    "_postman_id": "596ce3cb-d829-4843-b019-f4b9806a08cf",
    "description": "SAP product terminology is organized by domains. Domains are used in the translation process to determine the correct terminology for a given application. <br> This resource returns a list of the domains and domain groups that are available in SAP Translation Hub.<br> You can combine the domain resource with the translation resource to more accurately reflect the subject area of your texts.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "SAP",
      "item": [
        {
          "id": "72b19e0c-af4f-4ab3-bce4-c510ca721a3b",
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
              "id": "bf2c833b-d563-461a-9b95-682f1b31386c"
            }
          ]
        }
      ]
    }
  ]
}