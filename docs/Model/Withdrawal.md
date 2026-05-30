# # Withdrawal

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **string** | The local withdrawal ID |
**whop_id** | **string** | The Whop withdrawal ID |
**amount** | **float** | The amount withdrawn in cents |
**currency** | **string** | Three-letter ISO currency code |
**status** | **string** | The status of the withdrawal request |
**fee_amount** | **float** | Fee amount charged for the withdrawal in cents | [optional]
**fee_type** | **string** | The fee structure type (inclusive or exclusive) | [optional]
**markup_fee** | **float** | Markup fee applied in cents | [optional]
**speed** | **string** | Speed of withdrawal (standard, instant) | [optional]
**trace_code** | **string** | Bank trace or reference code for tracking the payout | [optional]
**payer_name** | **string** | The name of the entity or account paying out | [optional]
**error_message** | **string** | Error message if the withdrawal failed | [optional]
**business_id** | **string** | The business ID associated with this withdrawal |
**created_at** | **\DateTime** | Timestamp when the withdrawal was requested |
**updated_at** | **\DateTime** | Timestamp when the withdrawal status was updated |

[[Back to Model list]](../../README.md#models) [[Back to API list]](../../README.md#endpoints) [[Back to README]](../../README.md)
