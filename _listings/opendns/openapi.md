swagger: "2.0"
x-collection-name: OpenDNS
x-complete: 1
info:
  title: OpenDNS
  version: 1.0.0
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