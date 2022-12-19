# vs-code masto.js snippets

Useful [masto.js](https://github.com/neet/masto.js) javascript to improve your masto experience

*⚠️this snippet is under construction*

## Supported languages (file extensions)
- JavaScript (.js)
- TypeScript (.ts)

## Installation
---
## Visual Studio Marketplace
Launch Quick Open:

- Linux: ```Ctrl+P```
- macOS: ```⌘P```
- Windows: ```Ctrl+P```

Paste the following command and press ```Enter```:

---
## Snippets info

in the moment masto snippet have also snippets for:
- accounts
- statuses

### `ms-login`
its look like:
```js
import { login } from 'masto';

async function main() {
    const masto = await login({
        url: 'https://example.com',
        accessToken: 'TOKEN',
    });
}

main().catch((error) => {
    console.error(error);
});

```
### Statuses Repository

| prefix                   | Snippet                      | Propuser      |
| ----------------------   | -----------------------------| --------------|
| `ms-status-fetch`        | `MastoStatusFetch`             | `fetch to View information about a status` |
| `ms-status-create`       | `MastoStatusCreate`            | `create to Post a new status` |
| `ms-status-cwi`          | `MastoStatusCreateWithImage`   | `create status with image` |
| `ms-status-update`       | `MastoStatusUpdate`            | `update a status`|
| `ms-status-Remove`       | `MastoStatusRemove`            | `delete one of your own statuses` |
| `ms-status-fc`           | `MastoStatusFetchContext`      | `fetchContext View statuses above and below this status in the thread`  |
| `ms-status-favourite`    | `MastoStatusFavourite`         | `add a status to your favourites list` |
| `ms-status-unfavourite`  | `MastoStatusUnFavourite`       | `remove a status to your favorites list`  |
| `ms-status-mute`         | `MastoStatusMute`              | `do not receive notifications for the thread that this status is part of.`|
| `ms-status-unmute`       | `MastoStatusUnMute`            | `start receiving notifications again for the thread that this status is part of`|
| `ms-status-frb`          | `MastoStatusFetchRebloggedBy`  | `view who boosted a given status`|
| `ms-status-ffb`          | `MastoStatusFetchFavouritedBy` | `view who favourited a given status` |
| `ms-status-reblog`       | `MastoStatusReblob`            | `reblog re-share a status` |
| `ms-status-unreblog`     | `MastoStatusUnreblog`          | `undo a re-share of a status` |
| `ms-status-pin`          | `MastoStatusPin`               | `feature one of your own public statuses at the top of your profile`       |
| `ms-status-unpin`        | `MastoStatusUnPin`             | `un-feature a status from the top of your profile`  |
| `ms-status-bookmark`     | `MastoStatusBookmark`          | `privately bookmark a status` |
| `ms-status-unbookmark`   | `MastoStatusUnBookmark`        | `remove a status from your private bookmarks` |
| `ms-status-fh`           | `MastoStatusFetchHistory`      | `fetch a history` |
| `ms-status-fs`           | `MastoStatusFetchSource`       | `fetch source` |


### Accounts Repository

| prefix                    | Snippet                       | Propuser      |
| ----------------------    | ----------------------------- | --------------|
| `ms-account-fetch`        | `MastoAccountFetch`           | `fetch view information about a profile` |
| `ms-account-create`       | `MastoAccountCreate`          | `creates a user and account records. Returns an account access token` |
| `ms-account-vc`           | `MastoAccountVerifyCredentials`  | `test to make sure that the user token works` |
| `ms-account-uc`           | `MastoAccountUpdateCredentials`           | `update credentials update the user's display and preferences` |
| `ms-account-ffs`          | `MastoAccountFetchFollowers`           | `fetch followers give accounts which followv the given account` |
| `ms-account-ffg`          | `MastoAccountFetchFollowing`           | `fetch following give which the given account is following` |
| `ms-account-fs`           | `MastoAccountFetchStatuses`           | `fetch statuses Statuses posted to the given account` |
| `ms-account-follow`       | `MastoAccountFollow`           | `follow the given account` |
| `ms-account-unfollow`     | `MastoAccountUnFollow`           | `unfollow the given accoun` |
| `ms-account-fr`           | `MastoAccountFetchRelationship`  | `fetch relationships out whether a given account is followed, blocked, etc` |
| `ms-account-search`       | `MastoAccountSearch`           | `search for matching accounts by username or display name` |
| `ms-account-block`        | `MastoAccountBlock`           | `block the given account` |
| `ms-account-unblock`      | `MastoAccountUnBlock`           | `unblock the given account` |
| `ms-account-pin`          | `MastoAccountPin`                | `pin add the given account to the user's featured profiles` |
| `ms-account-unpin`        | `MastoAccountUnPin`           | `remove the given account from the user's featured profiles` |
| `ms-account-fl`           | `MastoAccountFetchLists`           | `Fetch the list with the given ID. Used for verifying the title of a list` |
| `ms-account-mute`         | `MastoAccountMute`           | `mute the given account.` |
| `ms-account-unmute`       | `MastoAccountUnMute`           | `unmute the given account.` |
| `ms-account-cn`           | `MastoAccountCreateNote`           | `createNote` |
| `ms-account-ftt`          | `MastoAccountFetchFeaturedTags`           | `get featured tag of the account` |
| `ms-account-fip`          | `MastoAccountFetchIdentityProofs`           | `identity proofs` |
| `ms-account-lookup`        | `MastoAccountLookup` | `This method allows to quickly convert a username of a known account to an ID that can be used with the REST API` |
| `ms-account-fff`        | `MastoAccountFetchFamiliarFollowers`           | `fetch familiar followers` |
| `ms-account-rff`        | `MastoAccountRemoveFromFollowers`           | `remove from followers` |

### App Repository

| prefix                   | Snippet                      | Propuser      |
| ----------------------   | -----------------------------| --------------|
| `ms-app-create`          | `MastoAppCreate`             | `create a new application to obtain OAuth2 credentials` |
| `ms-app-vc`              | `MastoAppVerifyCredentials`             | `confirm that the app's OAuth2 credentials work` |

### Announcements Repository

| prefix                   | Snippet                      | Propuser      |
| ----------------------   | -----------------------------| --------------|
| `ms-announcement-fa`     | `MastoAnnouncementFetchAll`  | `fetch announcements` |
| `ms-announcement-dismiss`| `MastoAnnouncementDismiss`   | `dismiss announcements` |
| `ms-announcement-ar`     | `MastoAnnouncementAddReaction`| `add a reaction to announcements` |
| `ms-announcement-rr`     | `MastoAnnouncementRemoveReaction` | `remove reaction to announcements` |

### Blocks Repository

| prefix                   | Snippet                      | Propuser      |
| ----------------------   | -----------------------------| --------------|
| `ms-block`               | `MastoBlockedIterate`        | `blocked users` |

### Bookmarks Repository

| prefix                   | Snippet                      | Propuser      |
| ----------------------   | -----------------------------| --------------|
| `ms-bookmark`            | `MastoBookmarkIterate`       | `Statuses the user has bookmarked` |

### Conversation Repository

| prefix                   | Snippet                      | Propuser            |
| ----------------------   | -----------------------------| ------------------- |
| `ms-conversation`        | `MastoConversationIterate`   | `Show conversation` |
| `ms-conversation-remove` | `MastoConversationRemove`    | `Show conversation` |
| `ms-conversation-read`   | `MastoConversationRead`      | `Show conversation` |

### CustomEmoji Repository

| prefix                   | Snippet                      | Propuser            |
| ----------------------   | -----------------------------| ------------------- |
| `ms-custom-emoji`        | `MastoCustomEmojiFetchAll`   | `return custom emojis that are available on the server` |

### Directory Repository

| prefix                   | Snippet              | Propuser            |
| ----------------------   | ---------------------| ------------------- |
| `ms-directory-fa`        | `MastoDirectory`     | `List accounts visible in the directory.` |

### DomainBlock Repository

| prefix                    | Snippet                     | Propuser            |
| ----------------------    | ----------------------------| ------------------- |
| `ms-domain-block-iterate` | `MastoDomainBlockIterate`   | `view domains the user has blocked` |
| `ms-domain-block-create`  | `MastoDomainBlock`          | `block a domain` |
| `ms-domain-block-remove`  | `MastoDomainUnBlock`        | `remove a domain block` |

### others coming soon...