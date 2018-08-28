---
swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 0
info:
  title: Plentymarkets Update multiple property relation value
  description: Updates multiple property relation value
  contact:
    name: plentymarkets
    url: https://forum.plentymarkets.com/c/rest-api
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
  /rest/feedbacks/delete_feedbacks/{feedbackIds}:
    delete:
      summary: Delete multiple feedbacks
      description: Deletes multiple feedbacks. A list with IDs of feedbacks must be
        specified.
      operationId: deleteRestFeedbacksDeleteFeedbacksFeedbacks
      x-api-path-slug: restfeedbacksdelete-feedbacksfeedbackids-delete
      parameters:
      - in: path
        name: feedbackIds
      responses:
        200:
          description: OK
      tags:
      - Multiple
      - Feedbacks
  /rest/feedbacks/feedbacks_visibility:
    put:
      summary: Update the visibility of multiple feedbacks
      description: Updates the visibility of multiple feedbacks. A list with IDs of
        feedbacks must be specified.
      operationId: putRestFeedbacksFeedbacksVisibility
      x-api-path-slug: restfeedbacksfeedbacks-visibility-put
      parameters:
      - in: query
        name: feedbackIds
        description: The list of feedback IDs, separated by commas
      - in: query
        name: isVisible
        description: The visibility value
      responses:
        200:
          description: OK
      tags:
      - Visibility
      - Of
      - Multiple
      - Feedbacks
  /rest/markets/settings/correlations/bulk:
    post:
      summary: Create multiple correlations
      description: Creates multiple correlations. The type, market settings ID and
        the correlation ID for each param combination must be specified.
      operationId: postRestMarketsSettingsCorrelationsBulk
      x-api-path-slug: restmarketssettingscorrelationsbulk-post
      responses:
        200:
          description: OK
      tags:
      - Multiple
      - Correlations
  /rest/plugin_sets/{pluginSetId}/languages/{languageCode}:
    delete:
      summary: Delete multiple translation
      description: Deletes multiple translation. The pluginSetId and languageCode
        must be specified.
      operationId: deleteRestPluginSetsPluginsetLanguagesLanguagecode
      x-api-path-slug: restplugin-setspluginsetidlanguageslanguagecode-delete
      parameters:
      - in: query
        name: $languageCode
        description: The code of the language
      - in: query
        name: $pluginSetId
        description: The ID of the plugin set
      - in: path
        name: languageCode
      - in: path
        name: pluginSetId
      responses:
        200:
          description: OK
      tags:
      - Multiple
      - Translation
  /rest/properties/relations/values:
    put:
      summary: Update multiple property relation value
      description: Updates multiple property relation value
      operationId: putRestPropertiesRelationsValues
      x-api-path-slug: restpropertiesrelationsvalues-put
      responses:
        200:
          description: OK
      tags:
      - Multiple
      - Property
      - Relation
      - Value
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