---
title: Authentication
position_number: 2
parameters:
  - name:
    content:
content_markdown: |-
  Authentication is the process of proving your identity to the system. The KPN API Store uses the OAuth 2.0 Client Credentials Grant type. Client IDs and Client secrets are provided when you create an app in the My apps dashboard of the KPN API Store. 

  Send your Client ID and Client secret with an API request to KPN API Store. You will receive an access token in the JSON message body of the response. 
  
  For example: `access_token`: `haf2SDl07E9N7RluNQ4kJ1TkGgso`

left_code_blocks:
  - code_block: |-
    {
    "refresh_token_expires_in": "0",
    "api_product_list": "[xxxxxxx]",
    "api_product_list_json": [
        " xxxxxxx"
    ],
    "organization_name": "kpn",
    "developer_email": "demo123@kpn.com",
    "token_type": "Bearer",
    "issued_at": "1521039195424",
    "client_id": "APP_CLIENT_ID",
    "access_token": "haf2SDl07E9N7RluNQ4kJ1TkGgso",
    "application_name": "6e38edxxxxxxxxxxxxxxxx4065d79c",
    "scope": "",
    "expires_in": "3599",
    "refresh_count": "0",
    "status": "approved"
    }
    title: Response
    language: json
right_code_blocks:
  - code_block: |2-
       $.get("http://api.myapp.com/books/", { "token": "YOUR_APP_KEY"}, function(data) {
         alert(data);
       });
    title: JQuery
    language: javascript
  - code_block: |2-
       curl http://api.myapp.com/books?token=YOUR_APP_KEY
    title: Curl
    language: bash
---