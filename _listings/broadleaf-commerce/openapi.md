---
swagger: "2.0"
x-collection-name: Broadleaf Commerce
x-complete: 1
info:
  title: Broadleaf Commerce API
  description: the-default-broadleaf-commerce-apis
  version: 1.0.0
host: demo.broadleafcommerce.org
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /wishlist/items/{itemId}/move:
    post:
      summary: Post Wishlist Items Move
      description: Post wishlist items move.
      operationId: postWishlistItemsItemMove
      x-api-path-slug: wishlistitemsitemidmove-post
      parameters:
      - in: path
        name: itemId
        description: itemId
      - in: query
        name: wishlistName
        description: wishlistName
      responses:
        200:
          description: OK
      tags:
      - Wishlist
      - Items
      - Move
---