---
swagger: "2.0"
x-collection-name: DomainTools
x-complete: 0
info:
  title: Whois History API Whois History
  description: Historical Whois records
  version: 1.0.0
host: api.domaintools.com
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{domain}/whois/history/:
    get:
      summary: Whois History
      description: Historical Whois records
      operationId: whoisHistory
      x-api-path-slug: domainwhoishistory-get
      parameters:
      - in: path
        name: domain
        description: The domain being requested
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Whois
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