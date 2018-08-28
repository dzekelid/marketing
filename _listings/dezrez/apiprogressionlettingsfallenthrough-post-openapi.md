---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: Dezrez Set Marketing Role as Fallen Through
  version: 1.0.0
  description: Set marketing role as fallen through.
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/documentgeneration/instruction:
    post:
      summary: Generates a Instruction letter correspondence to the vendor of a particular
        marketing role
      description: Generates a instruction letter correspondence to the vendor of
        a particular marketing role.
      operationId: DocumentGeneration_GenerateInstructionLetterPackBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationinstruction-post
      parameters:
      - in: body
        name: generatePackDetails
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Instruction
      - Letter
      - Correspondence
      - To
      - Vendor
      - Of
      - Particular
      - Marketing
      - Role
  /api/documentgeneration/withdrawninstruction:
    post:
      summary: Generates a Withdrawn Instruction letter correspondence to the vendor
        of a particular marketing role
      description: Generates a withdrawn instruction letter correspondence to the
        vendor of a particular marketing role.
      operationId: DocumentGeneration_GenerateWithdrawnInstructionLetterPackBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationwithdrawninstruction-post
      parameters:
      - in: body
        name: generatePackDetails
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Withdrawn
      - Instruction
      - Letter
      - Correspondence
      - To
      - Vendor
      - Of
      - Particular
      - Marketing
      - Role
  /api/documentgeneration/valuationlost:
    post:
      summary: Generates a Valuation Lost letter correspondence to the vendor of a
        particular marketing role
      description: Generates a valuation lost letter correspondence to the vendor
        of a particular marketing role.
      operationId: DocumentGeneration_GenerateValuationLostLetterPackBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationvaluationlost-post
      parameters:
      - in: body
        name: generatePackDetails
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Valuation
      - Lost
      - Letter
      - Correspondence
      - To
      - Vendor
      - Of
      - Particular
      - Marketing
      - Role
  /api/progression/lettings/fallenthrough:
    post:
      summary: Set Marketing Role as Fallen Through
      description: Set marketing role as fallen through.
      operationId: LettingsProgression_FallenThroughByfallenThroughDataContract
      x-api-path-slug: apiprogressionlettingsfallenthrough-post
      parameters:
      - in: body
        name: fallenThroughDataContract
        description: Details of the fallen though
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Set
      - Marketing
      - Role
      - As
      - Fallen
      - Through
  /api/list/property/propertyidsfiltered:
    post:
      summary: Get list of RoleIds for property marketing roles
      description: Get list of roleids for property marketing roles.
      operationId: List_GetPropertyListFilteredByfilter
      x-api-path-slug: apilistpropertypropertyidsfiltered-post
      parameters:
      - in: body
        name: filter
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - List
      - Of
      - RoleIdsproperty
      - Marketing
      - Roles
  /api/admin/portal/getportaluploadsforrole:
    get:
      summary: Get all the live portal uploads associated with a property marketing
        role
      description: Get all the live portal uploads associated with a property marketing
        role.
      operationId: Portal_GetLivePortalInformationRecordsForRoleByroleId
      x-api-path-slug: apiadminportalgetportaluploadsforrole-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: roleId
      responses:
        200:
          description: OK
      tags:
      - Live
      - Portal
      - Uploads
      - Associated
      - Property
      - Marketing
      - Role
  /api/role/{id}/valuation:
    get:
      summary: Gets the valuation for a property marketing role
      description: Gets the valuation for a property marketing role.
      operationId: Role_GetValuationByid
      x-api-path-slug: apiroleidvaluation-get
      parameters:
      - in: path
        name: id
        description: The id of the property marketing role to find a valuation for
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - S
      - Valuationa
      - Property
      - Marketing
      - Role
  /api/role/{id}/valued:
    get:
      summary: Gets the valuation for a property marketing role
      description: Gets the valuation for a property marketing role.
      operationId: Role_GetValuedByid
      x-api-path-slug: apiroleidvalued-get
      parameters:
      - in: path
        name: id
        description: The id of the property marketing role to find a valuation for
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - S
      - Valuationa
      - Property
      - Marketing
      - Role
  /api/role/{id}/offers:
    get:
      summary: Get all of the offers associated to the current property marketing
        role.
      description: Get all of the offers associated to the current property marketing
        role..
      operationId: Role_OffersByidBypageSizeBypageNumberByexcludeDrafts
      x-api-path-slug: apiroleidoffers-get
      parameters:
      - in: query
        name: excludeDrafts
      - in: path
        name: id
        description: The id of the role to get the offers for
      - in: query
        name: pageNumber
        description: Page number to return
      - in: query
        name: pageSize
        description: Page size to return
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Of
      - Offers
      - Associated
      - To
      - Current
      - Property
      - Marketing
      - Role
  /api/role/{id}/offersbasic:
    get:
      summary: Get a basic list of offers associated to the current property marketing
        role.
      description: Get a basic list of offers associated to the current property marketing
        role..
      operationId: Role_OffersBasicByid
      x-api-path-slug: apiroleidoffersbasic-get
      parameters:
      - in: path
        name: id
        description: The id of the marketing role to get the offers for
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Basic
      - List
      - Of
      - Offers
      - Associated
      - To
      - Current
      - Property
      - Marketing
      - Role
  /api/role/{roleId}/viewingsbasic:
    get:
      summary: Get a basic list of all viewings for a particular marketing role.
      description: Get a basic list of all viewings for a particular marketing role..
      operationId: Role_BasicViewingsByroleId
      x-api-path-slug: apiroleroleidviewingsbasic-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: path
        name: roleId
        description: The id of the marketing role to get the viewings for
      responses:
        200:
          description: OK
      tags:
      - Basic
      - List
      - Of
      - ""
      - Viewingsa
      - Particular
      - Marketing
      - Role
  /api/role/{id}/viewings:
    get:
      summary: Get all of the viewings associated to the current property marketing
        role.
      description: Get all of the viewings associated to the current property marketing
        role..
      operationId: Role_ViewingsByidBypageSizeBypageNumberByexcludeDrafts
      x-api-path-slug: apiroleidviewings-get
      parameters:
      - in: query
        name: excludeDrafts
      - in: path
        name: id
        description: The id of the role to get the offers for
      - in: query
        name: pageNumber
        description: Page number to return
      - in: query
        name: pageSize
        description: Page size to return
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Of
      - Viewings
      - Associated
      - To
      - Current
      - Property
      - Marketing
      - Role
  /api/role/{id}/setdefaultimage:
    put:
      summary: Sets the default image of a property marketing role
      description: Sets the default image of a property marketing role.
      operationId: Role_SetDefaultImageByidBydocumentId
      x-api-path-slug: apiroleidsetdefaultimage-put
      parameters:
      - in: query
        name: documentId
        description: The id of the document to set as the default image
      - in: path
        name: id
        description: The id of the role
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Sets
      - Default
      - Image
      - Of
      - Property
      - Marketing
      - Role
  /api/role/{id}/confirmcompliancechecks:
    put:
      summary: Confirms the compliance checks have been carried out on a marketing
        role
      description: Confirms the compliance checks have been carried out on a marketing
        role.
      operationId: Role_ConfirmComplianceChecksByidBynegotiatorId
      x-api-path-slug: apiroleidconfirmcompliancechecks-put
      parameters:
      - in: path
        name: id
        description: The id of the role
      - in: query
        name: negotiatorId
        description: The negotiator id who confirmed the checks
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Confirms
      - Compliance
      - Checks
      - Have
      - Been
      - Carried
      - Out
      - "On"
      - Marketing
      - Role
  /api/role/{id}/setflag:
    put:
      summary: Sets a flag on a property marketing role
      description: Sets a flag on a property marketing role.
      operationId: Role_SetFlagByidBysetMarketingFlagDataContract
      x-api-path-slug: apiroleidsetflag-put
      parameters:
      - in: path
        name: id
        description: The id of the role
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: body
        name: setMarketingFlagDataContract
        description: The flag detail
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Sets
      - Flag
      - "On"
      - Property
      - Marketing
      - Role
  /api/role/{id}/setcompliancechecks:
    put:
      summary: Set the compliance checks on a property marketing role i.e. Valid Epc,
        Proof of ID or Proof of Ownership.
      description: Set the compliance checks on a property marketing role i.e. valid
        epc, proof of id or proof of ownership..
      operationId: Role_SetComplianceChecksByidBysetComplianceChecksDataContract
      x-api-path-slug: apiroleidsetcompliancechecks-put
      parameters:
      - in: path
        name: id
        description: The id of the role
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: body
        name: setComplianceChecksDataContract
        description: The flag detail
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Set
      - Compliance
      - Checks
      - "On"
      - Property
      - Marketing
      - Role
      - I
      - E
      - ""
      - Valid
      - Epc
      - ""
      - Proof
      - Of
      - ID
      - Proof
      - Of
      - Ownership
  /api/role/suggest:
    get:
      summary: Search for property marketing roles that match the specified search
        criteria
      description: Search for property marketing roles that match the specified search
        criteria.
      operationId: Role_SuggestBydataContract.isOnMarketBydataContract.pageNumberBydataContract.pageSizeBydataContract.
      x-api-path-slug: apirolesuggest-get
      parameters:
      - in: query
        name: dataContract.isOnMarket
      - in: query
        name: dataContract.pageNumber
      - in: query
        name: dataContract.pageSize
      - in: query
        name: dataContract.query
      - in: query
        name: dataContract.roleType
      - in: query
        name: dataContract.suggestType
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Searchproperty
      - Marketing
      - Roles
      - That
      - Match
      - Specified
      - Search
      - Criteria
  /api/role/{id}/copy:
    post:
      summary: Clones a property marketing role
      description: Clones a property marketing role.
      operationId: Role_CopySalesMarketingRoleByid
      x-api-path-slug: apiroleidcopy-post
      parameters:
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Clones
      - Property
      - Marketing
      - Role
  /api/progression/sales/fallenthrough:
    post:
      summary: Set Marketing Role as Fallen Through
      description: Set marketing role as fallen through.
      operationId: SalesProgression_FallenThroughByfallenThroughDataContract
      x-api-path-slug: apiprogressionsalesfallenthrough-post
      parameters:
      - in: body
        name: fallenThroughDataContract
        description: Details of the fallen though
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Set
      - Marketing
      - Role
      - As
      - Fallen
      - Through
  /api/admin/system/sendliveportalupdatemessage:
    post:
      summary: "Sends a message to the LivePortalJobHandler that says \r\nthe specified
        property marketing role has changed"
      description: "Sends a message to the liveportaljobhandler that says \r\nthe
        specified property marketing role has changed."
      operationId: System_SendLivePortalUpdateMessageBypropertyMarketingRoleId
      x-api-path-slug: apiadminsystemsendliveportalupdatemessage-post
      parameters:
      - in: query
        name: propertyMarketingRoleId
        description: The property marketing role ID
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Sends
      - Message
      - To
      - LivePortalJobHandler
      - That
      - Says
      - The
      - Specified
      - Property
      - Marketing
      - Role
      - Has
      - Changed
  /api/role/{id}/addfee:
    put:
      summary: Add a fee for a given PropertyMarketingRole.
      description: Add a fee for a given propertymarketingrole..
      operationId: Role_AddFeeByidByfeeDataContract
      x-api-path-slug: apiroleidaddfee-put
      parameters:
      - in: body
        name: feeDataContract
        description: The fee to add to the role
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: the id of the role
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Feea
      - Given
      - PropertyMarketingRole
  /api/role/{id}/removefee:
    put:
      summary: Remove a fee from a given PropertyMarketingRole.
      description: Remove a fee from a given propertymarketingrole..
      operationId: Role_RemoveFeeByidByfeeId
      x-api-path-slug: apiroleidremovefee-put
      parameters:
      - in: query
        name: feeId
        description: The Id of the fee to remove
      - in: path
        name: id
        description: the id of the role
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Fee
      - From
      - Given
      - PropertyMarketingRole
  /api/role/{id}/updatefees:
    put:
      summary: Update the fee for a given PropertyMarketingRole.
      description: Update the fee for a given propertymarketingrole..
      operationId: Role_UpdateFeesByidByfeeDataContracts
      x-api-path-slug: apiroleidupdatefees-put
      parameters:
      - in: body
        name: feeDataContracts
        description: The fees to apply to the role
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: the id of the role
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Feea
      - Given
      - PropertyMarketingRole
  /api/roomdescription/{id}/attachtorole:
    put:
      summary: Attach a RoomDescription to a PropertyMarketingRole
      description: Attach a roomdescription to a propertymarketingrole.
      operationId: RoomDescription_AttachToRoleByidByroleId
      x-api-path-slug: apiroomdescriptionidattachtorole-put
      parameters:
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: roleId
      responses:
        200:
          description: OK
      tags:
      - Attach
      - RoomDescription
      - To
      - PropertyMarketingRole
  /api/enum/marketingrolestatus:
    get:
      summary: Get an enum by its type and system name
      description: Get an enum by its type and system name.
      operationId: Enum_GetMarketingRoleStatusBytransactionType
      x-api-path-slug: apienummarketingrolestatus-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: transactionType
        description: The typeo of marketingrole to get
      responses:
        200:
          description: OK
      tags:
      - Enum
      - By
      - Its
      - Type
      - System
      - Name
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