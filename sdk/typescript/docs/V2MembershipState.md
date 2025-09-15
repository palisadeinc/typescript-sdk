# V2MembershipState

- MEMBERSHIP_STATE_CREATED: Freshly created, but no push notification sent   - MEMBERSHIP_STATE_PENDING: Push notification to member device sent, but not received public key yet  - MEMBERSHIP_STATE_CONFIRMED: Device has confirmed with a public key  - MEMBERSHIP_STATE_REJECTED: Device has rejected membership  - MEMBERSHIP_STATE_FAILED: Generic error state  - MEMBERSHIP_STATE_SUPER: FSM USE ONLY: Super state  - MEMBERSHIP_STATE_INITIAL: FSM USE ONLY: Initial state

## Enum

* `MembershipStateCreated` (value: `'MEMBERSHIP_STATE_CREATED'`)

* `MembershipStatePending` (value: `'MEMBERSHIP_STATE_PENDING'`)

* `MembershipStateConfirmed` (value: `'MEMBERSHIP_STATE_CONFIRMED'`)

* `MembershipStateRejected` (value: `'MEMBERSHIP_STATE_REJECTED'`)

* `MembershipStateFailed` (value: `'MEMBERSHIP_STATE_FAILED'`)

* `MembershipStateSuper` (value: `'MEMBERSHIP_STATE_SUPER'`)

* `MembershipStateInitial` (value: `'MEMBERSHIP_STATE_INITIAL'`)

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
