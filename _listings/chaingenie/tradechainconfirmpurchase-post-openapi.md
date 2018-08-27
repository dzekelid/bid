---
swagger: "2.0"
x-collection-name: ChainGenie
x-complete: 0
info:
  title: ChainGenie Bid / buy listed item (by Buyer)
  description: "Bid / buy the item listed on the marketplace: <br/>\r\n- Buyer confirms
    interest in buying<br/>\r\n- Escrow from buyer added to value of contract<br/>\r\n-
    Invoice document is created with all details using invoice template<br/>\r\n-
    Invoice is added IPFS and invoice hash into blockchain<br/>\r\n- End transaction
    state = Trade is actively locked between the seller and buyer<br/>"
  version: "1.0"
host: api.chaingenie.com
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /tradechain/ConfirmPurchase:
    post:
      summary: Bid / buy listed item (by Buyer)
      description: "Bid / buy the item listed on the marketplace: <br/>\r\n- Buyer
        confirms interest in buying<br/>\r\n- Escrow from buyer added to value of
        contract<br/>\r\n- Invoice document is created with all details using invoice
        template<br/>\r\n- Invoice is added IPFS and invoice hash into blockchain<br/>\r\n-
        End transaction state = Trade is actively locked between the seller and buyer<br/>"
      operationId: TradechainConfirmPurchasePost
      x-api-path-slug: tradechainconfirmpurchase-post
      parameters:
      - in: header
        name: ApiKey
      - in: formData
        name: itemBuyerName
      - in: formData
        name: itemContractId
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Bid
      - ""
      - ""
      - Buy
      - Listed
      - Item
      - (by
      - Buyer)
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---