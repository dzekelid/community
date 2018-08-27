---
swagger: "2.0"
x-collection-name: Meetup
x-complete: 0
info:
  title: Meetup Report Group
  description: Submits a new abuse report for a target group. Abuse reports will be
    followed up on by our Community Support team.
  version: 1.0.0
host: api.meetup.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /:urlname/abuse_reports:
    post:
      summary: Report Group
      description: Submits a new abuse report for a target group. Abuse reports will
        be followed up on by our Community Support team.
      operationId: abuse
      x-api-path-slug: urlnameabuse-reports-post
      parameters:
      - in: query
        name: type
        description: A required identifier for type of abuse you are reporting
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
      - Groups
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