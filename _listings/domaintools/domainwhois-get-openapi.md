---
swagger: "2.0"
x-collection-name: DomainTools
x-complete: 0
info:
  title: Whois Lookup API Whois Lookup
  version: 1.0.0
  description: The Whois Lookup API provides the ownership record for a domain name
    or IP address with basic registration details.
host: api.domaintools.com
basePath: /v1/domaintools.com/
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
  /{domain}/whois:
    get:
      summary: Whois Lookup
      description: The Whois Lookup API provides the ownership record for a domain
        name or IP address with basic registration details.
      operationId: whoisLookup
      x-api-path-slug: domainwhois-get
      parameters:
      - in: path
        name: domain
        description: The domain to lookup
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