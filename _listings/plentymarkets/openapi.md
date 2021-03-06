swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 1
info:
  title: plentymarkets REST-API
  description: the-plentymarkets-rest-api-expands-the-functionality-of-the-plentymarkets-cms-and-allows-access-to-resources-i-e--data-records-via-unique-uri-paths
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
  /rest/warehouses/locations:
    delete:
      summary: Delete multiple warehouse locations
      description: Deletes multiple warehouse locations
      operationId: deleteRestWarehousesLocations
      x-api-path-slug: restwarehouseslocations-delete
      responses:
        200:
          description: OK
      tags:
      - Multiple
      - Warehouse
      - Locations
  /rest/warehouses/locations/multiple_dimensions:
    post:
      summary: Create multiple warehouse location dimensions
      description: Creates multiple warehouse location dimension.
      operationId: postRestWarehousesLocationsMultipleDimensions
      x-api-path-slug: restwarehouseslocationsmultiple-dimensions-post
      responses:
        200:
          description: OK
      tags:
      - Multiple
      - Warehouse
      - Location
      - Dimensions