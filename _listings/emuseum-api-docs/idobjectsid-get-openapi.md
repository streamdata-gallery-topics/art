---
swagger: "2.0"
x-collection-name: eMuseum API docs
x-complete: 0
info:
  title: eMuseum API Art
  description: Get Art
  version: 1.0.0
host: gsafinearts.pbs.gsa.gov
basePath: /emuseum/api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /id/objects/{id}:
    get:
      summary: Art
      description: Get Art
      operationId: getArt
      x-api-path-slug: idobjectsid-get
      responses:
        200:
          description: OK
      tags:
      - Art
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