---
swagger: "2.0"
x-collection-name: Quovo
x-complete: 0
info:
  title: Quovo Get an account's transactions
  description: Provides information on an account's historical transactions.
  version: 1.0.0
host: example.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /accounts/{account_id}:
    get:
      summary: Get a single account
      description: Provides information on a single account.
      operationId: AccountsByAccountIdGet
      x-api-path-slug: accountsaccount-id-get
      parameters:
      - in: path
        name: account_id
      responses:
        200:
          description: OK
      tags:
      - Single
      - Account
  /accounts/{account_id}/transactions:
    get:
      summary: Get an account's transactions
      description: Provides information on an account's historical transactions.
      operationId: AccountsTransactionsByAccountIdGet
      x-api-path-slug: accountsaccount-idtransactions-get
      parameters:
      - in: path
        name: account_id
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Transactions
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