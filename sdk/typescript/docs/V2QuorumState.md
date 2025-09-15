# V2QuorumState

- QUORUM_STATE_CREATED: Freshly created, but no push notifications sent   - QUORUM_STATE_PENDING: Push notifications to member devices sent, but not all confirmed  - QUORUM_STATE_CONFIRMED: All devices have accepted membership  - QUORUM_STATE_REJECTED: 1+ Devices have rejected membership  - QUORUM_STATE_FAILED: Generic error state  - QUORUM_STATE_SUPER: FSM USE ONLY: Super state  - QUORUM_STATE_INITIAL: FSM USE ONLY: Initial state  - QUORUM_STATE_MODIFY_MEMBERSHIP: Register new quorum members here  - QUORUM_STATE_MODIFY_SHARDS: Key shards are being modified  - QUORUM_STATE_FINALIZE_MODIFICATION: Members finalize the quorum modification, ensuring old shards are deleted etc.

## Enum

* `QuorumStateCreated` (value: `'QUORUM_STATE_CREATED'`)

* `QuorumStatePending` (value: `'QUORUM_STATE_PENDING'`)

* `QuorumStateConfirmed` (value: `'QUORUM_STATE_CONFIRMED'`)

* `QuorumStateRejected` (value: `'QUORUM_STATE_REJECTED'`)

* `QuorumStateFailed` (value: `'QUORUM_STATE_FAILED'`)

* `QuorumStateSuper` (value: `'QUORUM_STATE_SUPER'`)

* `QuorumStateInitial` (value: `'QUORUM_STATE_INITIAL'`)

* `QuorumStateModifyMembership` (value: `'QUORUM_STATE_MODIFY_MEMBERSHIP'`)

* `QuorumStateModifyShards` (value: `'QUORUM_STATE_MODIFY_SHARDS'`)

* `QuorumStateFinalizeModification` (value: `'QUORUM_STATE_FINALIZE_MODIFICATION'`)

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
