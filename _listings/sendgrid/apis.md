---
name: SendGrid
x-slug: sendgrid
description: Delivering your transactional and marketing emails through the worlds
  largest cloud-based email delivery platform. Send with confidence.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
x-kinRank: "9"
x-alexaRank: "10000"
tags: Recipients
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/recipients/master/_listings/sendgrid/apis.md
specificationVersion: "0.14"
apis:
- name: SendGrid Get Contactdb Lists List  Recipients
  x-api-slug: sendgrid
  description: "**This endpoint allows you to retrieve all recipients on the list
    with the given ID.** \n\nThe Contacts API helps you manage your [Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html)
    recipients."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//contactdb/lists/{list_id}/recipients
  tags: Email,Contactdb, Lists, List, , Recipients
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/recipients/master/_listings/sendgrid/contactdblistslist-idrecipients-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/recipients/master/_listings/sendgrid/contactdblistslist-idrecipients-get-openapi.md
- name: SendGrid Add Contactdb Lists List  Recipients
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to add multiple recipients to a list.**

    Adds existing recipients to a list, passing in the recipient IDs to add. Recipient IDs should be passed exactly as they are returned from recipient endpoints.

    The Contacts API helps you manage your [Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html) recipients.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//contactdb/lists/{list_id}/recipients
  tags: Email,Contactdb, Lists, List, , Recipients
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/recipients/master/_listings/sendgrid/contactdblistslist-idrecipients-post-openapi.md
- name: SendGrid Delete Contactdb Lists List  Recipients Recipient
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to delete a single recipient from a list.**

    The Contacts API helps you manage your [Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html) recipients.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//contactdb/lists/{list_id}/recipients/{recipient_id}
  tags: Email,Contactdb, Lists, List, , Recipients, Recipient
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/recipients/master/_listings/sendgrid/contactdblistslist-idrecipientsrecipient-id-delete-openapi.md
- name: SendGrid Add Contactdb Lists List  Recipients Recipient
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to add a single recipient to a list.**

    The Contacts API helps you manage your [Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html) recipients.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//contactdb/lists/{list_id}/recipients/{recipient_id}
  tags: Email,Contactdb, Lists, List, , Recipients, Recipient
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/recipients/master/_listings/sendgrid/contactdblistslist-idrecipientsrecipient-id-post-openapi.md
- name: SendGrid Delete Contactdb Recipients
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to deletes one or more recipients.**

    The body of an API call to this endpoint must include an array of recipient IDs of the recipients you want to delete.

    The contactdb is a database of your contacts for [SendGrid Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//contactdb/recipients
  tags: Email,Contactdb, Recipients
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/recipients/master/_listings/sendgrid/contactdbrecipients-delete-openapi.md
- name: SendGrid Get Contactdb Recipients
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to retrieve all of your Marketing Campaigns recipients.**

    Batch deletion of a page makes it possible to receive an empty page of recipients before reaching the end of
    the list of recipients. To avoid this issue; iterate over pages until a 404 is retrieved.

    The Contacts API helps you manage your [Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html) recipients.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//contactdb/recipients
  tags: Email,Contactdb, Recipients
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/recipients/master/_listings/sendgrid/contactdbrecipients-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/recipients/master/_listings/sendgrid/contactdbrecipients-get-openapi.md
- name: SendGrid Patch Contactdb Recipients
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to update one or more recipients.**

    The body of an API call to this endpoint must include an array of one or more recipient objects.

    It is of note that you can add custom field data as parameters on recipient objects. We have provided an example using some of the default custom fields SendGrid provides.

    The contactdb is a database of your contacts for [SendGrid Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//contactdb/recipients
  tags: Email,Contactdb, Recipients
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/recipients/master/_listings/sendgrid/contactdbrecipients-patch-openapi.md
- name: SendGrid Add Contactdb Recipients
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to add a Marketing Campaigns recipient.**

    You can add custom field data as a parameter on this endpoint. We have provided an example using some of the default custom fields SendGrid provides.

    The Contacts API helps you manage your [Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html) recipients.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//contactdb/recipients
  tags: Email,Contactdb, Recipients
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/recipients/master/_listings/sendgrid/contactdbrecipients-post-openapi.md
- name: SendGrid Get Contactdb Recipients Billable Count
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to retrieve the number of Marketing Campaigns recipients that you will be billed for.**

    You are billed for marketing campaigns based on the highest number of recipients you have had in your account at one time. This endpoint will allow you to know the current billable count value.

    The Contacts API helps you manage your [Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html) recipients.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//contactdb/recipients/billable_count
  tags: Email,Contactdb, Recipients, Billable, Count
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/recipients/master/_listings/sendgrid/contactdbrecipientsbillable-count-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/recipients/master/_listings/sendgrid/contactdbrecipientsbillable-count-get-openapi.md
- name: SendGrid Get Contactdb Recipients Count
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to retrieve the total number of Marketing Campaigns recipients.**

    The contactdb is a database of your contacts for [SendGrid Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//contactdb/recipients/count
  tags: Email,Contactdb, Recipients, Count
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/recipients/master/_listings/sendgrid/contactdbrecipientscount-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/recipients/master/_listings/sendgrid/contactdbrecipientscount-get-openapi.md
- name: SendGrid Get Contactdb Recipients Search
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to perform a search on all of your Marketing Campaigns recipients.**

    field_name:

    * is a variable that is substituted for your actual custom field name from your recipient.
    * Text fields must be url-encoded. Date fields are searchable only by unix timestamp (e.g. 2/2/2015 becomes 1422835200)
    * If field_name is a 'reserved' date field, such as created_at or updated_at, the system will internally convert
    your epoch time to a date range encompassing the entire day. For example, an epoch time of 1422835600 converts to
    Mon, 02 Feb 2015 00:06:40 GMT, but internally the system will search from Mon, 02 Feb 2015 00:00:00 GMT through
    Mon, 02 Feb 2015 23:59:59 GMT.

    The contactdb is a database of your contacts for [SendGrid Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//contactdb/recipients/search
  tags: Email,Contactdb, Recipients, Search
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/recipients/master/_listings/sendgrid/contactdbrecipientssearch-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/recipients/master/_listings/sendgrid/contactdbrecipientssearch-get-openapi.md
- name: SendGrid Delete Contactdb Recipients Recipient
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to delete a single recipient with the given ID from your contact database.**

    The Contacts API helps you manage your [Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html) recipients.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//contactdb/recipients/{recipient_id}
  tags: Email,Contactdb, Recipients, Recipient
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/recipients/master/_listings/sendgrid/contactdbrecipientsrecipient-id-delete-openapi.md
- name: SendGrid Get Contactdb Recipients Recipient
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to retrieve a single recipient by ID from your contact database.**

    The Contacts API helps you manage your [Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html) recipients.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//contactdb/recipients/{recipient_id}
  tags: Email,Contactdb, Recipients, Recipient
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/recipients/master/_listings/sendgrid/contactdbrecipientsrecipient-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/recipients/master/_listings/sendgrid/contactdbrecipientsrecipient-id-get-openapi.md
- name: SendGrid Get Contactdb Recipients Recipient  Lists
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to retrieve the lists that a given recipient belongs to.**

    Each recipient can be on many lists. This endpoint gives you all of the lists that any one recipient has been added to.

    The Contacts API helps you manage your [Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html) recipients.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//contactdb/recipients/{recipient_id}/lists
  tags: Email,Contactdb, Recipients, Recipient, , Lists
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/recipients/master/_listings/sendgrid/contactdbrecipientsrecipient-idlists-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/recipients/master/_listings/sendgrid/contactdbrecipientsrecipient-idlists-get-openapi.md
- name: SendGrid Get Contactdb Segments Segment  Recipients
  x-api-slug: sendgrid
  description: |-
    **This endpoint allows you to retrieve all of the recipients in a segment with the given ID.**

    The Contacts API helps you manage your [Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html) recipients.

    For more information about segments in Marketing Campaigns, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/lists.html#-Create-a-Segment).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3//contactdb/segments/{segment_id}/recipients
  tags: Email,Contactdb, Segments, Segment, , Recipients
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/recipients/master/_listings/sendgrid/contactdbsegmentssegment-idrecipients-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/recipients/master/_listings/sendgrid/contactdbsegmentssegment-idrecipients-get-openapi.md
- name: SendGrid
  x-api-slug: sendgrid
  description: SendGrids cloud-based email infrastructure relieves businesses of the
    cost and complexity of maintaining custom email systems. SendGrid provides reliable
    delivery, scalability and real-time analytics along with flexible APIs that make
    custom integration a breeze.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3
  tags: Recipients
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/recipients/master/_listings/sendgrid/openapi.md
x-common:
- type: x--net-library
  url: https://sendgrid.com/docs/Code_Examples/csharp.html
- type: x-base
  url: https://api.sendgrid.com
- type: x-blog
  url: http://blog.sendgrid.com/
- type: x-blog-rss
  url: http://feeds.feedburner.com/sendgrid/CDXr
- type: x-contact-form
  url: https://sendgrid.com/contact
- type: x-crunchbase
  url: http://www.crunchbase.com/company/sendgrid
- type: x-crunchbase
  url: https://crunchbase.com/organization/sendgrid
- type: x-developer
  url: https://sendgrid.com/developers
- type: x-documentation
  url: https://sendgrid.com/docs/index.html
- type: x-email
  url: privacy@sendgrid.com
- type: x-email
  url: legal@sendgrid.com
- type: x-email
  url: dpo@sendgrid.com
- type: x-forum
  url: http://support.sendgrid.com/forums
- type: x-github
  url: https://github.com/sendgrid
- type: x-go-library
  url: https://sendgrid.com/docs/Code_Examples/go.html
- type: x-ios-library
  url: https://sendgrid.com/docs/Code_Examples/ios.html
- type: x-java-library
  url: https://sendgrid.com/docs/Code_Examples/java.html
- type: x-labs
  url: http://labs.sendgrid.com/
- type: x-linkedin
  url: https://www.linkedin.com/company/sendgrid
- type: x-node-js-library
  url: https://sendgrid.com/docs/Code_Examples/nodejs.html
- type: x-partners
  url: https://sendgrid.com/partners
- type: x-perl-library
  url: https://sendgrid.com/docs/Code_Examples/perl.html
- type: x-php-library
  url: https://sendgrid.com/docs/Code_Examples/php.html
- type: x-pricing
  url: https://sendgrid.com/transactional-email/pricing
- type: x-privacy
  url: https://sendgrid.com/privacy
- type: x-python-library
  url: https://sendgrid.com/docs/Code_Examples/python.html
- type: x-ruby-library
  url: https://sendgrid.com/docs/Code_Examples/ruby.html
- type: x-security
  url: https://sendgrid.com/security
- type: x-selfservice-registration
  url: https://sendgrid.com/user/signup
- type: x-terms-of-service
  url: https://sendgrid.com/tos
- type: x-twitter
  url: https://twitter.com/SendGrid
- type: x-website
  url: http://sendgrid.com
- type: x-website
  url: https://sendgrid.com/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---