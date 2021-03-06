---
swagger: "2.0"
x-collection-name: GIG & CROWD
x-complete: 0
info:
  title: GIGANDCROWD Delete Art Rer
  version: 1.0.0
  description: Delete art rer.
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
  /api/v1/art/{unique}/details:
    get:
      summary: Get Art Unique Details
      description: Get art unique details.
      operationId: getApiV1ArtUniqueDetails
      x-api-path-slug: apiv1artuniquedetails-get
      parameters:
      - in: path
        name: unique
      responses:
        200:
          description: OK
      tags:
      - Art
      - Unique
      - Details
  /api/v1/art/{id}/videos:
    get:
      summary: Get Art Veos
      description: Get art veos.
      operationId: getApiV1ArtVeos
      x-api-path-slug: apiv1artidvideos-get
      parameters:
      - in: path
        name: id
        description: Id
      responses:
        200:
          description: OK
      tags:
      - Art
      - Veos
  /api/v1/art/{id}/events/past:
    get:
      summary: Get Art Events Past
      description: Get art events past.
      operationId: getApiV1ArtEventsPast
      x-api-path-slug: apiv1artideventspast-get
      parameters:
      - in: path
        name: id
        description: Id
      responses:
        200:
          description: OK
      tags:
      - Art
      - Events
      - Past
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
  /api/v1/art/search/{page}:
    post:
      summary: Post Art Search Page
      description: Post art search page.
      operationId: postApiV1ArtSearchPage
      x-api-path-slug: apiv1artsearchpage-post
      parameters:
      - in: path
        name: page
      - in: body
        name: request
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Art
      - Search
      - Page
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
  /api/v1/art/riderinfo:
    post:
      summary: Post Art Rerinfo
      description: Post art rerinfo.
      operationId: postApiV1ArtRerinfo
      x-api-path-slug: apiv1artriderinfo-post
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
      - Rerinfo
  /api/v1/art/rider:
    get:
      summary: Get Art Rer
      description: Get art rer.
      operationId: getApiV1ArtRer
      x-api-path-slug: apiv1artrider-get
      parameters:
      - in: header
        name: Authorization
      responses:
        200:
          description: OK
      tags:
      - Art
      - Rer
    post:
      summary: Post Art Rer
      description: Post art rer.
      operationId: postApiV1ArtRer
      x-api-path-slug: apiv1artrider-post
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
      - Rer
    delete:
      summary: Delete Art Rer
      description: Delete art rer.
      operationId: deleteApiV1ArtRer
      x-api-path-slug: apiv1artrider-delete
      parameters:
      - in: header
        name: Authorization
      responses:
        200:
          description: OK
      tags:
      - Art
      - Rer
  /api/v1/art/rider/home:
    get:
      summary: Get Art Rer Home
      description: Get art rer home.
      operationId: getApiV1ArtRerHome
      x-api-path-slug: apiv1artriderhome-get
      parameters:
      - in: header
        name: Authorization
      responses:
        200:
          description: OK
      tags:
      - Art
      - Rer
      - Home
    post:
      summary: Post Art Rer Home
      description: Post art rer home.
      operationId: postApiV1ArtRerHome
      x-api-path-slug: apiv1artriderhome-post
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
      - Rer
      - Home
    delete:
      summary: Delete Art Rer Home
      description: Delete art rer home.
      operationId: deleteApiV1ArtRerHome
      x-api-path-slug: apiv1artriderhome-delete
      parameters:
      - in: header
        name: Authorization
      responses:
        200:
          description: OK
      tags:
      - Art
      - Rer
      - Home
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
  /api/v1/art/video:
    post:
      summary: Post Art Veo
      description: Post art veo.
      operationId: postApiV1ArtVeo
      x-api-path-slug: apiv1artvideo-post
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
      - Veo
  /api/v1/art/video/{id}:
    delete:
      summary: Delete Art Veo
      description: Delete art veo.
      operationId: deleteApiV1ArtVeo
      x-api-path-slug: apiv1artvideoid-delete
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
      - Veo
  /api/v1/art/video/{id}/main:
    post:
      summary: Post Art Veo Main
      description: Post art veo main.
      operationId: postApiV1ArtVeoMain
      x-api-path-slug: apiv1artvideoidmain-post
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
      - Veo
      - Main
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
  /api/v1/request/art/invite:
    post:
      summary: Post Request Art Invite
      description: Post request art invite.
      operationId: postApiV1RequestArtInvite
      x-api-path-slug: apiv1requestartinvite-post
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
      - Request
      - Art
      - Invite
  /api/v1/request/art/in:
    get:
      summary: Get Request Art In
      description: Get request art in.
      operationId: getApiV1RequestArtIn
      x-api-path-slug: apiv1requestartin-get
      parameters:
      - in: header
        name: Authorization
      responses:
        200:
          description: OK
      tags:
      - Request
      - Art
      - In
  /api/v1/request/art/calendar:
    get:
      summary: Get Request Art Calendar
      description: Get request art calendar.
      operationId: getApiV1RequestArtCalendar
      x-api-path-slug: apiv1requestartcalendar-get
      parameters:
      - in: header
        name: Authorization
      - in: query
        name: request.from
      - in: query
        name: request.to
      responses:
        200:
          description: OK
      tags:
      - Request
      - Art
      - Calendar
  /api/v1/request/art/archive:
    get:
      summary: Get Request Art Archive
      description: Get request art archive.
      operationId: getApiV1RequestArtArchive
      x-api-path-slug: apiv1requestartarchive-get
      parameters:
      - in: header
        name: Authorization
      responses:
        200:
          description: OK
      tags:
      - Request
      - Art
      - Archive
  /api/v1/request/art/reject:
    post:
      summary: Post Request Art Reject
      description: Post request art reject.
      operationId: postApiV1RequestArtReject
      x-api-path-slug: apiv1requestartreject-post
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
      - Request
      - Art
      - Reject
  /api/v1/request/art/accept:
    post:
      summary: Post Request Art Accept
      description: Post request art accept.
      operationId: postApiV1RequestArtAccept
      x-api-path-slug: apiv1requestartaccept-post
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
      - Request
      - Art
      - Accept
  /api/v1/request/art/accept/performanceDate:
    post:
      summary: Post Request Art Accept Performancedate
      description: Post request art accept performancedate.
      operationId: postApiV1RequestArtAcceptPerformancedate
      x-api-path-slug: apiv1requestartacceptperformancedate-post
      parameters:
      - in: header
        name: Authorization
      - in: body
        name: request
        description: /
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Request
      - Art
      - Accept
      - Performancedate
  /api/v1/request/art/reject/performanceDate:
    post:
      summary: Post Request Art Reject Performancedate
      description: Post request art reject performancedate.
      operationId: postApiV1RequestArtRejectPerformancedate
      x-api-path-slug: apiv1requestartrejectperformancedate-post
      parameters:
      - in: header
        name: Authorization
      - in: body
        name: request
        description: /
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Request
      - Art
      - Reject
      - Performancedate
  /api/v1/request/{requestId}/art/{artistId}/rider:
    get:
      summary: Get Request Requestid Art Artistid Rer
      description: Get request requestid art artistid rer.
      operationId: getApiV1RequestRequestArtArtistRer
      x-api-path-slug: apiv1requestrequestidartartistidrider-get
      parameters:
      - in: path
        name: artistId
      - in: header
        name: Authorization
      - in: path
        name: requestId
        description: /
      responses:
        200:
          description: OK
      tags:
      - Request
      - Requestid
      - Art
      - Artistid
      - Rer
  /api/v1/request/{requestId}/art/{artistId}/rider/home:
    get:
      summary: Get Request Requestid Art Artistid Rer Home
      description: Get request requestid art artistid rer home.
      operationId: getApiV1RequestRequestArtArtistRerHome
      x-api-path-slug: apiv1requestrequestidartartistidriderhome-get
      parameters:
      - in: path
        name: artistId
      - in: header
        name: Authorization
      - in: path
        name: requestId
        description: /
      responses:
        200:
          description: OK
      tags:
      - Request
      - Requestid
      - Art
      - Artistid
      - Rer
      - Home
  /api/v1/request/{requestId}/art/{artistId}/presskit/{photoId}:
    get:
      summary: Get Request Requestid Art Artistid Presskit Photoid
      description: Get request requestid art artistid presskit photoid.
      operationId: getApiV1RequestRequestArtArtistPresskitPhoto
      x-api-path-slug: apiv1requestrequestidartartistidpresskitphotoid-get
      parameters:
      - in: path
        name: artistId
      - in: header
        name: Authorization
      - in: path
        name: photoId
      - in: path
        name: requestId
      responses:
        200:
          description: OK
      tags:
      - Request
      - Requestid
      - Art
      - Artistid
      - Presskit
      - Photoid
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