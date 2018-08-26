---
swagger: "2.0"
x-collection-name: DomainTools
x-complete: 1
info:
  title: Whois Lookup API
  version: 1.0.0
host: api.domaintools.com
basePath: /v1/domaintools.com/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
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
---