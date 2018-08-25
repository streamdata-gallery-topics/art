---
swagger: "2.0"
x-collection-name: GIG & CROWD
x-complete: 0
info:
  title: GIGANDCROWD Post Art Photo Type
  version: 1.0.0
  description: Post art photo type.
host: gigandcrowd.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v1/account/register/art:
    post:
      summary: Post Account Register Art
      description: Post account register art.
      operationId: postApiV1AccountRegisterArt
      x-api-path-slug: apiv1accountregisterart-post
      parameters:
      - in: body
        name: request
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Account
      - Register
      - Art
  /api/v1/Art:
    get:
      summary: Get Art
      description: Get art.
      operationId: getApiV1Art
      x-api-path-slug: apiv1art-get
      parameters:
      - in: header
        name: Authorization
      responses:
        200:
          description: OK
      tags:
      - Art
  /api/v1/art/background:
    post:
      summary: Post Art Background
      description: Post art background.
      operationId: postApiV1ArtBackground
      x-api-path-slug: apiv1artbackground-post
      parameters:
      - in: header
        name: Authorization
      - in: query
        name: file
      responses:
        200:
          description: OK
      tags:
      - Art
      - Background
  /api/v1/art/info:
    post:
      summary: Post Art Info
      description: Post art info.
      operationId: postApiV1ArtInfo
      x-api-path-slug: apiv1artinfo-post
      parameters:
      - in: header
        name: Authorization
      - in: body
        name: request
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Art
      - Info
  /api/v1/art/invited/{artistId}/{eventId}:
    get:
      summary: Get Art Invited Artistid Eventid
      description: Get art invited artistid eventid.
      operationId: getApiV1ArtInvitedArtistEvent
      x-api-path-slug: apiv1artinvitedartistideventid-get
      parameters:
      - in: path
        name: artistId
      - in: path
        name: eventId
      responses:
        200:
          description: OK
      tags:
      - Art
      - Invited
      - Artistid
      - Eventid
  /api/v1/art/link:
    post:
      summary: Post Art Link
      description: Post art link.
      operationId: postApiV1ArtLink
      x-api-path-slug: apiv1artlink-post
      parameters:
      - in: header
        name: Authorization
      - in: body
        name: model
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Art
      - Link
  /api/v1/art/link/{id}:
    delete:
      summary: Delete Art Link
      description: Delete art link.
      operationId: deleteApiV1ArtLink
      x-api-path-slug: apiv1artlinkid-delete
      parameters:
      - in: header
        name: Authorization
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Art
      - Link
  /api/v1/art/photo/{id}:
    delete:
      summary: Delete Art Photo
      description: Delete art photo.
      operationId: deleteApiV1ArtPhoto
      x-api-path-slug: apiv1artphotoid-delete
      parameters:
      - in: header
        name: Authorization
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Art
      - Photo
  /api/v1/art/photo/{photoId}:
    get:
      summary: Get Art Photo Photoid
      description: Get art photo photoid.
      operationId: getApiV1ArtPhotoPhoto
      x-api-path-slug: apiv1artphotophotoid-get
      parameters:
      - in: header
        name: Authorization
      - in: path
        name: photoId
      responses:
        200:
          description: OK
      tags:
      - Art
      - Photo
      - Photoid
  /api/v1/art/photo/{photoId}/thumb:
    get:
      summary: Get Art Photo Photoid Thumb
      description: Get art photo photoid thumb.
      operationId: getApiV1ArtPhotoPhotoThumb
      x-api-path-slug: apiv1artphotophotoidthumb-get
      parameters:
      - in: header
        name: Authorization
      - in: path
        name: photoId
      responses:
        200:
          description: OK
      tags:
      - Art
      - Photo
      - Photoid
      - Thumb
  /api/v1/art/photo/{type}:
    post:
      summary: Post Art Photo Type
      description: Post art photo type.
      operationId: postApiV1ArtPhotoType
      x-api-path-slug: apiv1artphototype-post
      parameters:
      - in: header
        name: Authorization
      - in: query
        name: file
      responses:
        200:
          description: OK
      tags:
      - Art
      - Photo
      - Type
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