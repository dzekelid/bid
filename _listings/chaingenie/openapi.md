swagger: "2.0"
x-collection-name: ChainGenie
x-complete: 1
info:
  title: ChainGenie = DLT + Blockchain + Magic
  description: chaingenie-is-here-to-help-companies-enjoy-the-benefits-of-blockchain-technology-distributed-tamper-proof-record-keeping-consensus-between-distrusting-nodes-when-you-do-not-have-the-expensive-blockchain-resources-chaingenie-offers-a-hook-to-connect-your-existing-it-applications-to-popular-blockchain-networks-like-ethereum-bitcoin-blockchain-etc-with-great-ease---want-to-know-how-chaingenie-works-under-the-hood-download-our-flyer--httpchaingenie-comchaingenieflyer-pdfthe-following-is-only-teaser-documentation--for-full-information-email--a-hrefmailtomagicchaingenie-commagicchaingenie-comahrupdate-09262016-brullibanking-micro-services-addedliliapikey-is-required-for-invoking-any-micro-serviceliulemail-a-hrefmailtomagicchaingenie-commagicchaingenie-coma-for-your-sandbox-apikey-hrcoming-soon-brmagic-canvas--drag-and-drop-microservices-to-create-a-blockchain-application---iblockchain-made-easyihrwant-to-connect-with-me-on-linkedin-send-me-an-invite--a-hrefhttplinkedin-cominupriya-target-blankhttplinkedin-cominupriyaahrscript----function-i-s-o-g-r-a-m---------igoogleanalyticsobject--r-ir--ir--function--------------ir-q--ir-q---pusharguments---------ir-l--1--new-date-a--s-createelemento--m--s-getelementsbytagnameo0-a-async--1-a-src--g-m-parentnode-insertbeforea-m----window-document-script-httpswww-googleanalytics-comanalytics-js-ga----gacreate-ua825523031-auto----gasend-pageviewscript
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