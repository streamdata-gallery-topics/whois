---
swagger: "2.0"
x-collection-name: OpenDNS
x-complete: 0
info:
  title: OpenDNS Whois
  version: 1.0.0
  description: This API method returns the WHOIS information for the specified email
    address(es), nameserver(s) and domains. You can also search by multiple email
    addresses or multiple nameservers.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /whois/emails/:
    get:
      summary: Whois
      description: This API method returns the WHOIS information for the specified
        email address(es), nameserver(s) and domains. You can also search by multiple
        email addresses or multiple nameservers.
      operationId: whois
      x-api-path-slug: whoisemails-get
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