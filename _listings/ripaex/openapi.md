swagger: "2.0"
x-collection-name: RipaEx
x-complete: 1
info:
  title: RIPA Node Documentation
  description: this-is-a-documentation-for-ripanodehttpsgithub-comripaexripanode-built-with-swagger-ui-to-make-testing-a-breeze--if-you-find-any-issues-come-over-to-ripaexripanodetestapihttpsgithub-comripaexripanodetestapi-to-open-an-issue-or-even-better-send-a-pr-that-fixes-the-issue-the-community-ssl-public-api-used-as-test-host-is-provided-from-ripaex-iohttpswww-ripaex-io-
  version: 1.0.0
host: api.ripaex.io
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /peer/blocks/common:
    get:
      summary: Peer Blocks Common
      description: Get a list of blocks by ids.
      operationId: transport.commonBlock
      x-api-path-slug: peerblockscommon-get
      parameters:
      - in: query
        name: ids
        description: A list of block IDs
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Peer
      - Blocks
      - Common