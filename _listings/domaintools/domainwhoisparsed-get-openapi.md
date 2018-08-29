---
swagger: "2.0"
x-collection-name: DomainTools
x-complete: 0
info:
  title: Parsed Whois API Parsed Whois
  description: The Parsed Whois API provides parsed information extracted from the
    raw Whois recor
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
  /{domain}/whois/parsed:
    get:
      summary: Parsed Whois
      description: The Parsed Whois API provides parsed information extracted from
        the raw Whois recor
      operationId: parsedWhois
      x-api-path-slug: domainwhoisparsed-get
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