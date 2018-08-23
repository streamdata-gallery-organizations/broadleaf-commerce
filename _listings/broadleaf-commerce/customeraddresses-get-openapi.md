---
swagger: "2.0"
x-collection-name: Broadleaf Commerce
x-complete: 0
info:
  title: Broadleaf Commerce API Get Customer Addresses
  description: Get customer addresses.
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
  /auditevents:
    get:
      summary: Get Auditevents
      description: Get auditevents.
      operationId: getAuditevents
      x-api-path-slug: auditevents-get
      parameters:
      - in: query
        name: after
        description: after
      - in: query
        name: principal
        description: principal
      - in: query
        name: type
        description: type
      responses:
        200:
          description: OK
      tags:
      - Auditevents
  /auditevents.json:
    get:
      summary: Get Auditevents
      description: Get auditevents.
      operationId: getAuditevents.json
      x-api-path-slug: auditevents-json-get
      parameters:
      - in: query
        name: after
        description: after
      - in: query
        name: principal
        description: principal
      - in: query
        name: type
        description: type
      responses:
        200:
          description: OK
      tags:
      - Auditevents
  /autoconfig:
    get:
      summary: Get Autoconfig
      description: Get autoconfig.
      operationId: getAutoconfig
      x-api-path-slug: autoconfig-get
      responses:
        200:
          description: OK
      tags:
      - Autoconfig
  /autoconfig.json:
    get:
      summary: Get Autoconfig
      description: Get autoconfig.
      operationId: getAutoconfig.json
      x-api-path-slug: autoconfig-json-get
      responses:
        200:
          description: OK
      tags:
      - Autoconfig
  /beans:
    get:
      summary: Get Beans
      description: Get beans.
      operationId: getBeans
      x-api-path-slug: beans-get
      responses:
        200:
          description: OK
      tags:
      - Beans
  /beans.json:
    get:
      summary: Get Beans
      description: Get beans.
      operationId: getBeans.json
      x-api-path-slug: beans-json-get
      responses:
        200:
          description: OK
      tags:
      - Beans
  /cart:
    get:
      summary: Get Cart
      description: Get cart.
      operationId: getCart
      x-api-path-slug: cart-get
      parameters:
      - in: query
        name: customerId
      responses:
        200:
          description: OK
      tags:
      - Cart
    post:
      summary: Post Cart
      description: Post cart.
      operationId: postCart
      x-api-path-slug: cart-post
      parameters:
      - in: query
        name: customerId
      responses:
        200:
          description: OK
      tags:
      - Cart
  /cart/checkout:
    post:
      summary: Post Cart Checkout
      description: Post cart checkout.
      operationId: postCartCheckout
      x-api-path-slug: cartcheckout-post
      parameters:
      - in: query
        name: cartId
        description: cartId
      responses:
        200:
          description: OK
      tags:
      - Cart
      - Checkout
  /cart/checkout/payment:
    post:
      summary: Post Cart Checkout Payment
      description: Post cart checkout payment.
      operationId: postCartCheckoutPayment
      x-api-path-slug: cartcheckoutpayment-post
      parameters:
      - in: query
        name: cartId
        description: cartId
      - in: body
        name: wrapper
        description: wrapper
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Cart
      - Checkout
      - Payment
  /cart/checkout/payment/{customerPaymentId}:
    post:
      summary: Post Cart Checkout Payment Customerpaymentid
      description: Post cart checkout payment customerpaymentid.
      operationId: postCartCheckoutPaymentCustomerpayment
      x-api-path-slug: cartcheckoutpaymentcustomerpaymentid-post
      parameters:
      - in: query
        name: amount
        description: amount
      - in: query
        name: cartId
        description: cartId
      - in: query
        name: currency
        description: currency
      - in: path
        name: customerPaymentId
        description: customerPaymentId
      responses:
        200:
          description: OK
      tags:
      - Cart
      - Checkout
      - Payment
      - Customerpaymentid
  /cart/checkout/payment/{paymentId}:
    delete:
      summary: Delete Cart Checkout Payment Paymentid
      description: Delete cart checkout payment paymentid.
      operationId: deleteCartCheckoutPaymentPayment
      x-api-path-slug: cartcheckoutpaymentpaymentid-delete
      parameters:
      - in: query
        name: cartId
        description: cartId
      - in: path
        name: paymentId
        description: paymentId
      responses:
        200:
          description: OK
      tags:
      - Cart
      - Checkout
      - Payment
      - Paymentid
  /cart/checkout/payment/{paymentId}/transaction:
    put:
      summary: Put Cart Checkout Payment Paymentid Transaction
      description: Put cart checkout payment paymentid transaction.
      operationId: putCartCheckoutPaymentPaymentTransaction
      x-api-path-slug: cartcheckoutpaymentpaymentidtransaction-put
      parameters:
      - in: query
        name: cartId
        description: cartId
      - in: path
        name: paymentId
        description: paymentId
      - in: body
        name: wrapper
        description: wrapper
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Cart
      - Checkout
      - Payment
      - Paymentid
      - Transaction
  /cart/checkout/payments:
    get:
      summary: Get Cart Checkout Payments
      description: Get cart checkout payments.
      operationId: getCartCheckoutPayments
      x-api-path-slug: cartcheckoutpayments-get
      parameters:
      - in: query
        name: cartId
        description: cartId
      responses:
        200:
          description: OK
      tags:
      - Cart
      - Checkout
      - Payments
  /cart/{cartId}:
    get:
      summary: Get Cart
      description: Get cart.
      operationId: getCartCart
      x-api-path-slug: cartcartid-get
      parameters:
      - in: path
        name: cartId
        description: cartId
      - in: query
        name: customerId
      responses:
        200:
          description: OK
      tags:
      - Cart
  /cart/{cartId}/attributes:
    put:
      summary: Put Cart Attributes
      description: Put cart attributes.
      operationId: putCartCartAttributes
      x-api-path-slug: cartcartidattributes-put
      parameters:
      - in: path
        name: cartId
        description: cartId
      - in: query
        name: customerId
      - in: query
        name: priceOrder
        description: priceOrder
      - in: body
        name: requestParams
        description: requestParams
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Cart
      - Attributes
    delete:
      summary: Delete Cart Attributes
      description: Delete cart attributes.
      operationId: deleteCartCartAttributes
      x-api-path-slug: cartcartidattributes-delete
      parameters:
      - in: path
        name: cartId
        description: cartId
      - in: query
        name: customerId
      - in: query
        name: priceOrder
        description: priceOrder
      - in: body
        name: requestParams
        description: requestParams
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Cart
      - Attributes
  /cart/{cartId}/item:
    post:
      summary: Post Cart Item
      description: Post cart item.
      operationId: postCartCartItem
      x-api-path-slug: cartcartiditem-post
      parameters:
      - in: path
        name: cartId
        description: cartId
      - in: query
        name: customerId
      - in: body
        name: orderItemWrapper
        description: orderItemWrapper
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: priceOrder
        description: priceOrder
      responses:
        200:
          description: OK
      tags:
      - Cart
      - Item
  /cart/{cartId}/item/{itemId}/attributes:
    put:
      summary: Put Cart Item Attributes
      description: Put cart item attributes.
      operationId: putCartCartItemItemAttributes
      x-api-path-slug: cartcartiditemitemidattributes-put
      parameters:
      - in: path
        name: cartId
        description: cartId
      - in: query
        name: customerId
      - in: path
        name: itemId
        description: itemId
      - in: query
        name: priceOrder
        description: priceOrder
      - in: body
        name: requestParams
        description: requestParams
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Cart
      - Item
      - Attributes
    delete:
      summary: Delete Cart Item Attributes
      description: Delete cart item attributes.
      operationId: deleteCartCartItemItemAttributes
      x-api-path-slug: cartcartiditemitemidattributes-delete
      parameters:
      - in: path
        name: cartId
        description: cartId
      - in: query
        name: customerId
      - in: path
        name: itemId
        description: itemId
      - in: query
        name: priceOrder
        description: priceOrder
      - in: body
        name: requestParams
        description: requestParams
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Cart
      - Item
      - Attributes
  /cart/{cartId}/items/{itemId}:
    put:
      summary: Put Cart Items
      description: Put cart items.
      operationId: putCartCartItemsItem
      x-api-path-slug: cartcartiditemsitemid-put
      parameters:
      - in: path
        name: cartId
        description: cartId
      - in: query
        name: customerId
      - in: path
        name: itemId
        description: itemId
      - in: query
        name: priceOrder
        description: priceOrder
      - in: query
        name: quantity
        description: quantity
      responses:
        200:
          description: OK
      tags:
      - Cart
      - Items
    delete:
      summary: Delete Cart Items
      description: Delete cart items.
      operationId: deleteCartCartItemsItem
      x-api-path-slug: cartcartiditemsitemid-delete
      parameters:
      - in: path
        name: cartId
        description: cartId
      - in: query
        name: customerId
      - in: path
        name: itemId
        description: itemId
      - in: query
        name: priceOrder
        description: priceOrder
      responses:
        200:
          description: OK
      tags:
      - Cart
      - Items
  /cart/{cartId}/offer/{promoCode}:
    post:
      summary: Post Cart Offer Promocode
      description: Post cart offer promocode.
      operationId: postCartCartOfferPromocode
      x-api-path-slug: cartcartidofferpromocode-post
      parameters:
      - in: path
        name: cartId
        description: cartId
      - in: query
        name: customerId
      - in: query
        name: priceOrder
        description: priceOrder
      - in: path
        name: promoCode
        description: promoCode
      responses:
        200:
          description: OK
      tags:
      - Cart
      - Offer
      - Promocode
    delete:
      summary: Delete Cart Offer Promocode
      description: Delete cart offer promocode.
      operationId: deleteCartCartOfferPromocode
      x-api-path-slug: cartcartidofferpromocode-delete
      parameters:
      - in: path
        name: cartId
        description: cartId
      - in: query
        name: customerId
      - in: query
        name: priceOrder
        description: priceOrder
      - in: path
        name: promoCode
        description: promoCode
      responses:
        200:
          description: OK
      tags:
      - Cart
      - Offer
      - Promocode
  /cart/{cartId}/offers:
    delete:
      summary: Delete Cart Offers
      description: Delete cart offers.
      operationId: deleteCartCartOffers
      x-api-path-slug: cartcartidoffers-delete
      parameters:
      - in: path
        name: cartId
        description: cartId
      - in: query
        name: customerId
      - in: query
        name: priceOrder
        description: priceOrder
      responses:
        200:
          description: OK
      tags:
      - Cart
      - Offers
  /catalog/categories:
    get:
      summary: Get Catalog Categories
      description: Get catalog categories.
      operationId: getCatalogCategories
      x-api-path-slug: catalogcategories-get
      parameters:
      - in: query
        name: limit
        description: limit
      - in: query
        name: name
        description: name
      - in: query
        name: offset
        description: offset
      responses:
        200:
          description: OK
      tags:
      - Catalog
      - Categories
  /catalog/category:
    get:
      summary: Get Catalog Category
      description: Get catalog category.
      operationId: getCatalogCategory
      x-api-path-slug: catalogcategory-get
      parameters:
      - in: query
        name: productLimit
        description: productLimit
      - in: query
        name: productOffset
        description: productOffset
      - in: query
        name: searchParameter
        description: searchParameter
      - in: query
        name: subcategoryLimit
        description: subcategoryLimit
      - in: query
        name: subcategoryOffset
        description: subcategoryOffset
      responses:
        200:
          description: OK
      tags:
      - Catalog
      - Category
  /catalog/category/{categoryId}:
    get:
      summary: Get Catalog Category
      description: Get catalog category.
      operationId: getCatalogCategoryCategory
      x-api-path-slug: catalogcategorycategoryid-get
      parameters:
      - in: path
        name: categoryId
        description: categoryId
      - in: query
        name: productLimit
        description: productLimit
      - in: query
        name: productOffset
        description: productOffset
      - in: query
        name: subcategoryLimit
        description: subcategoryLimit
      - in: query
        name: subcategoryOffset
        description: subcategoryOffset
      responses:
        200:
          description: OK
      tags:
      - Catalog
      - Category
  /catalog/category/{categoryId}/activeSubcategories:
    get:
      summary: Get Catalog Category Active Subcategories
      description: Get catalog category active subcategories.
      operationId: getCatalogCategoryCategoryActivesubcategories
      x-api-path-slug: catalogcategorycategoryidactivesubcategories-get
      parameters:
      - in: path
        name: categoryId
        description: categoryId
      - in: query
        name: limit
        description: limit
      - in: query
        name: offset
        description: offset
      responses:
        200:
          description: OK
      tags:
      - Catalog
      - Category
      - Active
      - Subcategories
  /catalog/category/{categoryId}/attributes:
    get:
      summary: Get Catalog Category Attributes
      description: Get catalog category attributes.
      operationId: getCatalogCategoryCategoryAttributes
      x-api-path-slug: catalogcategorycategoryidattributes-get
      parameters:
      - in: path
        name: categoryId
        description: categoryId
      responses:
        200:
          description: OK
      tags:
      - Catalog
      - Category
      - Attributes
  /catalog/category/{categoryId}/categories:
    get:
      summary: Get Catalog Category Categories
      description: Get catalog category categories.
      operationId: getCatalogCategoryCategoryCategories
      x-api-path-slug: catalogcategorycategoryidcategories-get
      parameters:
      - in: query
        name: active
        description: active
      - in: path
        name: categoryId
        description: categoryId
      - in: query
        name: limit
        description: limit
      - in: query
        name: offset
        description: offset
      responses:
        200:
          description: OK
      tags:
      - Catalog
      - Category
      - Categories
  /catalog/category/{id}/media:
    get:
      summary: Get Catalog Category Media
      description: Get catalog category media.
      operationId: getCatalogCategoryMedia
      x-api-path-slug: catalogcategoryidmedia-get
      parameters:
      - in: path
        name: id
        description: id
      responses:
        200:
          description: OK
      tags:
      - Catalog
      - Category
      - Media
  /catalog/product/{id}:
    get:
      summary: Get Catalog Product
      description: Get catalog product.
      operationId: getCatalogProduct
      x-api-path-slug: catalogproductid-get
      parameters:
      - in: path
        name: id
        description: id
      - in: query
        name: includePriceData
        description: includePriceData
      - in: query
        name: includePromotionMessages
        description: includePromotionMessages
      responses:
        200:
          description: OK
      tags:
      - Catalog
      - Product
  /catalog/product/{productId}/attributes:
    get:
      summary: Get Catalog Product Attributes
      description: Get catalog product attributes.
      operationId: getCatalogProductProductAttributes
      x-api-path-slug: catalogproductproductidattributes-get
      parameters:
      - in: path
        name: productId
        description: productId
      responses:
        200:
          description: OK
      tags:
      - Catalog
      - Product
      - Attributes
  /catalog/product/{productId}/categories:
    get:
      summary: Get Catalog Product Categories
      description: Get catalog product categories.
      operationId: getCatalogProductProductCategories
      x-api-path-slug: catalogproductproductidcategories-get
      parameters:
      - in: path
        name: productId
        description: productId
      responses:
        200:
          description: OK
      tags:
      - Catalog
      - Product
      - Categories
  /catalog/product/{productId}/crosssale:
    get:
      summary: Get Catalog Product Crosssale
      description: Get catalog product crosssale.
      operationId: getCatalogProductProductCrosssale
      x-api-path-slug: catalogproductproductidcrosssale-get
      parameters:
      - in: query
        name: limit
        description: limit
      - in: query
        name: offset
        description: offset
      - in: path
        name: productId
        description: productId
      responses:
        200:
          description: OK
      tags:
      - Catalog
      - Product
      - Crosssale
  /catalog/product/{productId}/defaultSku:
    get:
      summary: Get Catalog Product Default sku
      description: Get catalog product default sku.
      operationId: getCatalogProductProductDefaultsku
      x-api-path-slug: catalogproductproductiddefaultsku-get
      parameters:
      - in: path
        name: productId
        description: productId
      responses:
        200:
          description: OK
      tags:
      - Catalog
      - Product
      - Default
      - Sku
  /catalog/product/{productId}/media:
    get:
      summary: Get Catalog Product Media
      description: Get catalog product media.
      operationId: getCatalogProductProductMedia
      x-api-path-slug: catalogproductproductidmedia-get
      parameters:
      - in: path
        name: productId
        description: productId
      responses:
        200:
          description: OK
      tags:
      - Catalog
      - Product
      - Media
  /catalog/product/{productId}/skus:
    get:
      summary: Get Catalog Product Skus
      description: Get catalog product skus.
      operationId: getCatalogProductProductSkus
      x-api-path-slug: catalogproductproductidskus-get
      parameters:
      - in: path
        name: productId
        description: productId
      responses:
        200:
          description: OK
      tags:
      - Catalog
      - Product
      - Skus
  /catalog/product/{productId}/upsale:
    get:
      summary: Get Catalog Product Upsale
      description: Get catalog product upsale.
      operationId: getCatalogProductProductUpsale
      x-api-path-slug: catalogproductproductidupsale-get
      parameters:
      - in: query
        name: limit
        description: limit
      - in: query
        name: offset
        description: offset
      - in: path
        name: productId
        description: productId
      responses:
        200:
          description: OK
      tags:
      - Catalog
      - Product
      - Upsale
  /catalog/search:
    get:
      summary: Get Catalog Search
      description: Get catalog search.
      operationId: getCatalogSearch
      x-api-path-slug: catalogsearch-get
      parameters:
      - in: query
        name: includePriceData
        description: includePriceData
      - in: query
        name: includePromotionMessages
        description: includePromotionMessages
      - in: query
        name: page
        description: page
      - in: query
        name: pageSize
        description: pageSize
      - in: query
        name: q
        description: q
      responses:
        200:
          description: OK
      tags:
      - Catalog
      - Search
  /catalog/search/category/{categoryId}:
    get:
      summary: Get Catalog Search Category
      description: Get catalog search category.
      operationId: getCatalogSearchCategoryCategory
      x-api-path-slug: catalogsearchcategorycategoryid-get
      parameters:
      - in: path
        name: categoryId
        description: categoryId
      - in: query
        name: includePriceData
        description: includePriceData
      - in: query
        name: includePromotionMessages
        description: includePromotionMessages
      - in: query
        name: page
        description: page
      - in: query
        name: pageSize
        description: pageSize
      - in: query
        name: q
        description: q
      responses:
        200:
          description: OK
      tags:
      - Catalog
      - Search
      - Category
  /catalog/sku/inventory:
    get:
      summary: Get Catalog Sku Inventory
      description: Get catalog sku inventory.
      operationId: getCatalogSkuInventory
      x-api-path-slug: catalogskuinventory-get
      parameters:
      - in: query
        name: id
        description: id
      responses:
        200:
          description: OK
      tags:
      - Catalog
      - Sku
      - Inventory
  /catalog/sku/{skuId}:
    get:
      summary: Get Catalog Sku Skuid
      description: Get catalog sku skuid.
      operationId: getCatalogSkuSku
      x-api-path-slug: catalogskuskuid-get
      parameters:
      - in: path
        name: skuId
        description: skuId
      responses:
        200:
          description: OK
      tags:
      - Catalog
      - Sku
      - Skuid
  /catalog/sku/{skuId}/attributes:
    get:
      summary: Get Catalog Sku Skuid Attributes
      description: Get catalog sku skuid attributes.
      operationId: getCatalogSkuSkuAttributes
      x-api-path-slug: catalogskuskuidattributes-get
      parameters:
      - in: path
        name: skuId
        description: skuId
      responses:
        200:
          description: OK
      tags:
      - Catalog
      - Sku
      - Skuid
      - Attributes
  /catalog/sku/{skuId}/media:
    get:
      summary: Get Catalog Sku Skuid Media
      description: Get catalog sku skuid media.
      operationId: getCatalogSkuSkuMedia
      x-api-path-slug: catalogskuskuidmedia-get
      parameters:
      - in: path
        name: skuId
        description: skuId
      responses:
        200:
          description: OK
      tags:
      - Catalog
      - Sku
      - Skuid
      - Media
  /configprops:
    get:
      summary: Get Configprops
      description: Get configprops.
      operationId: getConfigprops
      x-api-path-slug: configprops-get
      responses:
        200:
          description: OK
      tags:
      - Configprops
  /configprops.json:
    get:
      summary: Get Configprops
      description: Get configprops.
      operationId: getConfigprops.json
      x-api-path-slug: configprops-json-get
      responses:
        200:
          description: OK
      tags:
      - Configprops
  /customer:
    get:
      summary: Get Customer
      description: Get customer.
      operationId: getCustomer
      x-api-path-slug: customer-get
      parameters:
      - in: query
        name: email
        description: email
      responses:
        200:
          description: OK
      tags:
      - Customer
    post:
      summary: Post Customer
      description: Post customer.
      operationId: postCustomer
      x-api-path-slug: customer-post
      parameters:
      - in: body
        name: wrapper
        description: wrapper
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Customer
    put:
      summary: Put Customer
      description: Put customer.
      operationId: putCustomer
      x-api-path-slug: customer-put
      parameters:
      - in: query
        name: customerId
      - in: body
        name: wrapper
        description: wrapper
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Customer
  /customer/address:
    get:
      summary: Get Customer Address
      description: Get customer address.
      operationId: getCustomerAddress
      x-api-path-slug: customeraddress-get
      parameters:
      - in: query
        name: addressName
        description: addressName
      - in: query
        name: customerId
      responses:
        200:
          description: OK
      tags:
      - Customer
      - Ress
    put:
      summary: Put Customer Address
      description: Put customer address.
      operationId: putCustomerAddress
      x-api-path-slug: customeraddress-put
      parameters:
      - in: query
        name: customerId
      - in: body
        name: wrapper
        description: wrapper
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Customer
      - Ress
  /customer/address/{addressId}:
    put:
      summary: Put Customer Address Addressid
      description: Put customer address addressid.
      operationId: putCustomerAddressAddress
      x-api-path-slug: customeraddressaddressid-put
      parameters:
      - in: path
        name: addressId
        description: addressId
      - in: query
        name: customerId
      - in: body
        name: wrapper
        description: wrapper
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Customer
      - Ress
      - Ressid
  /customer/address/{addressName}:
    delete:
      summary: Delete Customer Address Addressname
      description: Delete customer address addressname.
      operationId: deleteCustomerAddressAddressname
      x-api-path-slug: customeraddressaddressname-delete
      parameters:
      - in: path
        name: addressName
        description: addressName
      - in: query
        name: customerId
      responses:
        200:
          description: OK
      tags:
      - Customer
      - Ress
      - Ressname
  /customer/addresses:
    get:
      summary: Get Customer Addresses
      description: Get customer addresses.
      operationId: getCustomerAddresses
      x-api-path-slug: customeraddresses-get
      parameters:
      - in: query
        name: customerId
      responses:
        200:
          description: OK
      tags:
      - Customer
      - Resses
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