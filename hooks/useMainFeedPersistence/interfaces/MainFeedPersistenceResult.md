[**REJKT.xyz Feed and Filter System Documentation v0.1.0**](../../../README.md)

***

[REJKT.xyz Feed and Filter System Documentation](../../../modules.md) / [hooks/useMainFeedPersistence](../README.md) / MainFeedPersistenceResult

# Interface: MainFeedPersistenceResult

Interface for the main feed persistence return object

## Properties

### addListings()

> **addListings**: (`newListings`) => `void`

#### Parameters

##### newListings

[`BaseListing`](../../../lib/curatedFeed/interfaces/BaseListing.md)[]

#### Returns

`void`

***

### clearFeedState()

> **clearFeedState**: () => `Promise`\<`void`\>

#### Returns

`Promise`\<`void`\>

***

### isFeedRestored

> **isFeedRestored**: `boolean`

***

### isRestoring

> **isRestoring**: `boolean`

***

### isStale()

> **isStale**: () => `Promise`\<`boolean`\>

#### Returns

`Promise`\<`boolean`\>

***

### lastId

> **lastId**: `null` \| `string`

***

### listings

> **listings**: [`BaseListing`](../../../lib/curatedFeed/interfaces/BaseListing.md)[]

***

### restoreScrollPosition()

> **restoreScrollPosition**: () => `void`

#### Returns

`void`

***

### saveFeedState()

> **saveFeedState**: () => `Promise`\<`boolean`\>

#### Returns

`Promise`\<`boolean`\>

***

### scrollPosition

> **scrollPosition**: `number`

***

### setLastId()

> **setLastId**: (`lastId`) => `void`

#### Parameters

##### lastId

`null` | `string`

#### Returns

`void`

***

### setListings()

> **setListings**: (`listings`) => `void`

#### Parameters

##### listings

[`BaseListing`](../../../lib/curatedFeed/interfaces/BaseListing.md)[]

#### Returns

`void`
