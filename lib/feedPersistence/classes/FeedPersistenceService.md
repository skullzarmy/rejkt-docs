[**REJKT.xyz Feed and Filter System Documentation v0.1.0**](../../../README.md)

***

[REJKT.xyz Feed and Filter System Documentation](../../../modules.md) / [lib/feedPersistence](../README.md) / FeedPersistenceService

# Class: FeedPersistenceService

Feed Persistence Service
Core service for feed state persistence operations

## Constructors

### Constructor

> **new FeedPersistenceService**(): `FeedPersistenceService`

#### Returns

`FeedPersistenceService`

## Methods

### cleanupExpiredFeeds()

> **cleanupExpiredFeeds**(): `Promise`\<`number`\>

Clean up expired feeds

#### Returns

`Promise`\<`number`\>

Promise resolving to number of items cleaned up

***

### clearArtistFeedState()

> **clearArtistFeedState**(`filters?`): `Promise`\<`void`\>

Clear artist feed state

#### Parameters

##### filters?

[`FiltersRecord`](../../curatedFeed/type-aliases/FiltersRecord.md)

Optional filters to clear specific state

#### Returns

`Promise`\<`void`\>

Promise resolving to void

***

### clearGalleryFeedState()

> **clearGalleryFeedState**(`offset?`): `Promise`\<`void`\>

Clear gallery feed state

#### Parameters

##### offset?

`number`

Optional offset to clear specific state

#### Returns

`Promise`\<`void`\>

Promise resolving to void

***

### clearMainFeedState()

> **clearMainFeedState**(`filters?`): `Promise`\<`void`\>

Clear main feed state

#### Parameters

##### filters?

[`FiltersRecord`](../../curatedFeed/type-aliases/FiltersRecord.md)

Optional filters to clear specific state

#### Returns

`Promise`\<`void`\>

Promise resolving to void

***

### getArtistFeedState()

> **getArtistFeedState**(`filters`): `Promise`\<`null` \| \{ `lastId`: `null` \| `string`; `listings`: [`BaseListing`](../../curatedFeed/interfaces/BaseListing.md)[]; `scrollPosition`: `number`; `seenArtists`: `string`[]; \}\>

Get artist feed state

#### Parameters

##### filters

[`FiltersRecord`](../../curatedFeed/type-aliases/FiltersRecord.md)

Current filter state to match

#### Returns

`Promise`\<`null` \| \{ `lastId`: `null` \| `string`; `listings`: [`BaseListing`](../../curatedFeed/interfaces/BaseListing.md)[]; `scrollPosition`: `number`; `seenArtists`: `string`[]; \}\>

Promise resolving to artist feed state or null

***

### getGalleryFeedState()

> **getGalleryFeedState**(`offset`): `Promise`\<`null` \| \{ `offset`: `number`; `scrollPosition`: `number`; `tokens`: [`GalleryToken`](../../galleryFeed/interfaces/GalleryToken.md)[]; \}\>

Get gallery feed state

#### Parameters

##### offset

`number`

Current pagination offset to match

#### Returns

`Promise`\<`null` \| \{ `offset`: `number`; `scrollPosition`: `number`; `tokens`: [`GalleryToken`](../../galleryFeed/interfaces/GalleryToken.md)[]; \}\>

Promise resolving to gallery feed state or null

***

### getMainFeedState()

> **getMainFeedState**(`filters`): `Promise`\<`null` \| \{ `lastId`: `null` \| `string`; `listings`: [`BaseListing`](../../curatedFeed/interfaces/BaseListing.md)[]; `scrollPosition`: `number`; \}\>

Get main feed state

#### Parameters

##### filters

[`FiltersRecord`](../../curatedFeed/type-aliases/FiltersRecord.md)

Current filter state to match

#### Returns

`Promise`\<`null` \| \{ `lastId`: `null` \| `string`; `listings`: [`BaseListing`](../../curatedFeed/interfaces/BaseListing.md)[]; `scrollPosition`: `number`; \}\>

Promise resolving to main feed state or null

***

### getStorageStats()

> **getStorageStats**(): `Promise`\<\{ `artistFeedCount`: `number`; `galleryFeedCount`: `number`; `mainFeedCount`: `number`; `singleArtistFeedCount`: `number`; `totalItems`: `number`; \}\>

Get storage usage statistics

#### Returns

`Promise`\<\{ `artistFeedCount`: `number`; `galleryFeedCount`: `number`; `mainFeedCount`: `number`; `singleArtistFeedCount`: `number`; `totalItems`: `number`; \}\>

Promise resolving to storage statistics

***

### saveArtistFeedState()

> **saveArtistFeedState**(`listings`, `filters`, `lastId`, `scrollPosition`, `seenArtists`): `Promise`\<`boolean`\>

Save artist feed state

#### Parameters

##### listings

[`BaseListing`](../../curatedFeed/interfaces/BaseListing.md)[]

Array of artist listings to save

##### filters

[`FiltersRecord`](../../curatedFeed/type-aliases/FiltersRecord.md)

Current filter state

##### lastId

Last ID for pagination

`null` | `string`

##### scrollPosition

`number`

Current scroll position

##### seenArtists

`string`[] = `[]`

Array of seen artist wallet addresses

#### Returns

`Promise`\<`boolean`\>

Promise resolving to success flag

***

### saveGalleryFeedState()

> **saveGalleryFeedState**(`tokens`, `offset`, `scrollPosition`): `Promise`\<`boolean`\>

Save gallery feed state

#### Parameters

##### tokens

[`GalleryToken`](../../galleryFeed/interfaces/GalleryToken.md)[]

Array of gallery tokens to save

##### offset

`number`

Current pagination offset

##### scrollPosition

`number`

Current scroll position

#### Returns

`Promise`\<`boolean`\>

Promise resolving to success flag

***

### saveMainFeedState()

> **saveMainFeedState**(`listings`, `filters`, `lastId`, `scrollPosition`): `Promise`\<`boolean`\>

Save main feed state

#### Parameters

##### listings

[`BaseListing`](../../curatedFeed/interfaces/BaseListing.md)[]

Array of listings to save

##### filters

[`FiltersRecord`](../../curatedFeed/type-aliases/FiltersRecord.md)

Current filter state

##### lastId

Last ID for pagination

`null` | `string`

##### scrollPosition

`number`

Current scroll position

#### Returns

`Promise`\<`boolean`\>

Promise resolving to success flag
