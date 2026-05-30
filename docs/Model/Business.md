# # Business

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **string** | The unique business ID |
**title** | **string** | Title or name of the business |
**description** | **string** | A description explaining what the business does | [optional]
**whop_id** | **string** | The Whop Company ID |
**merchant_id** | **string** | The merchant owner ID |
**verified** | **bool** | Whether the business has been KYC-verified on Whop |
**send_customer_emails** | **bool** | Whether auto-emails are enabled for customers |
**member_count** | **float** | Total members/customers under this business |
**route** | **string** | Whop friendly URL path route | [optional]
**default_currency** | **string** | The default currency of the business |
**published_reviews_count** | **float** | Number of published user reviews on Whop |
**metadata** | **object** | Custom key-value metadata | [optional]
**target_audience** | **string** | The target audience description | [optional]
**social_links** | **object** | Social links setup | [optional]
**affiliate_instructions** | **string** | Markdown instructions for affiliates | [optional]
**whop_created_at** | **\DateTime** | Whop account creation timestamp | [optional]
**whop_updated_at** | **\DateTime** | Whop account last updated timestamp | [optional]
**created_at** | **\DateTime** | Timestamp when the business record was created |
**updated_at** | **\DateTime** | Timestamp when the business record was last updated |
**logo_url** | **string** | Brand logo image URL resolved from primary brand | [optional]

[[Back to Model list]](../../README.md#models) [[Back to API list]](../../README.md#endpoints) [[Back to README]](../../README.md)
