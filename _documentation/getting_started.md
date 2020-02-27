---
title: Getting Started
position_number: 1
parameters:
  - name:
    content:
content_markdown: |-
  Welcome to the CertiMint API 

The CertiMint API accepts data in three ways.

* Seal a hash.
The most secure way is to send a hash (SHA3-512) of your data to the API since it does not expose any of the data. 

* Send data as a string.

* Send a file.
The platform hashes the data for you and stores the data for later retrieval.

The `hash` and `string` endpoints accept arrays of data, allowing you to batch the data to be anchored together and decrease the performance overhead of high throughput anchor operations.

For each data item, the endpoint returns a unique identifier. This identifier is the key you need to request the crypto seal. The platform is creating the crypto seal in the background.

The files endpoint works a bit different, it takes a regular form upload (for example, from your website) over a JSON payload. 
  
  ### API workflow

![Conceptual model](/sites/default/files/SettleMint_CertiMint_API_workflow.png)

  You'll succeed if you do this.
  {: .success }

  Here's some useful information.
  {: .info }

  Something may not happen if you try and do this.
  {: .warning }

  Something bad will happen if you do this.
  {: .error }
left_code_blocks:
  - code_block:
    title:
    language:
right_code_blocks:
  - code_block:
    title:
    language:
---