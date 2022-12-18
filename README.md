# vs-code masto.js snippets

Useful masto javascript to improve your masto experience

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
## Statuses
### `ms-status-fetch`
```js
const fetch = await masto.statuses.fetch('id');
```
### `ms-status-create`
```js
const createStatus = await masto.statuses.create({
    status: 'Toot from TypeScript',
    visibility: 'direct',
});
```
### `ms-status-cwi`
```js
const attachment = await masto.mediaAttachments.create({
    file: fs.createReadStream('../some_image.png'),
    description: 'Some image',
});

const status = await masto.statuses.create({
    status: 'Toot from TypeScript',
    visibility: 'direct',
    mediaIds: [attachment.id],
});

console.log(status)
```
### `ms-status-update`
```js
const updateStatus = await masto.statuses.update('id', {
    status: 'Toot from Typescript'
});
```
### `ms-status-remove`
```js
const removeStatus = await masto.statuses.remove('id');
```
### `ms-status-fc`
```js
const fetchContext = await masto.statuses.fetchContext('id');
```
### `ms-status-favourite`
```js
const favourite = await masto.statuses.favourite('id');
```
### `ms-status-unfavourite`
```js
const unFavourite = await masto.statuses.unfavourite('id');
```
### `ms-status-mute`
```js
const muteStatus = await masto.statuses.mute('id');
```
### `ms-status-unmute`
```js
const unMuteStatus = await masto.statuses.unmute('id');
```
### `ms-status-frb`
```js
const fetchRebloggedBy = await masto.statuses.fetchRebloggedBy('id');
```
### `ms-status-ffb`
```js
const fetchFavouritedBy = await masto.statuses.fetchFavouritedBy('id');
```
### `ms-status-reblog`
```js
const reblob = await masto.statuses.reblog('id', {
    visibility: 'direct',
});
```
### `ms-status-unreblog`
```js
const unReblob = await masto.statuses.unreblog('id');
```
### `ms-status-pin`
```js
const pinStatus = await masto.statuses.pin('id');
```
### `ms-status-unpin`
```js
const unPin = await masto.statuses.unpin('id');
```
### `ms-status-bookmark`
```js
const bookmarkStatus = await masto.statuses.bookmark('id');
```
### `ms-status-unbookmark`
```js
const unBookmarkStatus = await masto.statuses.unbookmark('id');
```
### `ms-status-fh`
```js
const fetchHistory = await masto.statuses.fetchHistory('id');
```
### `ms-status-fs`
```js
const fetchSource = await masto.statuses.fetchSource('id');
```
## Accounts

### `ms-account-fetch`
```js
const fetchAccount = await masto.accounts.fetch('id');  
```
### `ms-account-create`
```js
const account = await masto.accounts.create({
    username: '',
    password: '',
    email: '',
    agreement: true,
    locale: '',
});
```
### `ms-account-vc`
```js
const credential = await masto.accounts.verifyCredentials();
console.log(credential)
```
### `ms-account-uc`
```js
const updateCredentials = await masto.accounts.updateCredentials({
    displayName: 'Fluffy elephant friend',
    note: 'Hi fediverse!',
    avatar: fs.createReadStream('../some_image.png'),
});
```
### `ms-account-ffs`
```js
const fetchFollowers = await masto.accounts.fetchFollowers('id', {
        
});
```
### `ms-account-ffg`
```js
const fetchFollowing = await masto.accounts.fetchFollowing('id', {
        
});
```
### `ms-account-fs`
```js
const fetchStatuses = await masto.accounts.fetchStatuses('id', {
        
});
```
### `ms-account-follow`
```js
const follow = await masto.accounts.follow('id', {
    /* optional */
    reblogs: true
});
```
### `ms-account-unfollow`
```js
const unFollow = await masto.accounts.unfollow('id', {
    /* optional */
    reblogs: true
});
```
### `ms-account-fr`
```js
const fetchRelationships = await masto.accounts.fetchRelationships('id: string[]');
```
### `ms-account-search`
```js
const search = await masto.accounts.search({
    q: ''
});
```
### `ms-account-block`
```js
const block = await masto.accounts.block('id');
```
### `ms-account-unblock`
```js
const unblock = await masto.accounts.unblock('id');
```
### `ms-account-pin`
```js
const pin = await masto.accounts.pin('id');
```
### `ms-account-unpin`
```js
const unpin = await masto.accounts.unpin('id');
```
### `ms-account-fl`
```js
const fetchLists = await masto.accounts.fetchLists('id');
```
### `ms-account-mute`
```js
const mute = await masto.accounts.mute('id', {  });
```
### `ms-account-unmute`
```js
const unmute = await masto.accounts.unmute('id');
```
### `ms-account-cn`
```js
const createNote = await masto.accounts.createNote('id', {
    comment: ''
});
```
### `ms-account-fft`
```js
const fetchFeaturedTags = await masto.accounts.fetchFeaturedTags('id');
```
### `ms-account-fip`
```js
const fetchIdentityProofs = await masto.accounts.fetchIdentityProofs('id');
```
### `ms-account-lookup`
```js
const lookup = await masto.accounts.lookup({
    acct: ''
});
```
### `ms-account-fff`
```js
const fetchFamiliarFollowers = await masto.accounts.fetchFamiliarFollowers();
```
### `ms-account-rff`
```js
const removeFromFollowers = await masto.accounts.removeFromFollowers('id');
```

### others coming soon...