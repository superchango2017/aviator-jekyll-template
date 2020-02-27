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
        access_token": haf2SDl07E9N7RluNQ4kJ1TkGgso
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