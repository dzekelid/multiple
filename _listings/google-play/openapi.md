---
swagger: "2.0"
x-collection-name: Google Play
x-complete: 1
info:
  title: Google Play
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /achievements/updateMultiple:
    post:
      summary: Update Multiple Achievements
      description: Updates multiple achievements for the currently authenticated player.
      operationId: games.achievements.updateMultiple
      x-api-path-slug: achievementsupdatemultiple-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: consistencyToken
        description: The last-seen mutation timestamp
      responses:
        200:
          description: OK
      tags:
      - Achievement
---