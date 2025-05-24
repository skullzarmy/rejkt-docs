[**REJKT.xyz Feed and Filter System Documentation v0.1.0**](../../../README.md)

***

[REJKT.xyz Feed and Filter System Documentation](../../../modules.md) / [hooks/useGalleryFeedPersistence](../README.md) / GalleryFeedPersistenceResult

# Interface: GalleryFeedPersistenceResult

Interface for the gallery feed persistence return object

## Properties

### addTokens()

> **addTokens**: (`newTokens`) => `void`

#### Parameters

##### newTokens

[`GalleryToken`](../../../lib/galleryFeed/interfaces/GalleryToken.md)[]

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

### offset

> **offset**: `number`

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

### setOffset()

> **setOffset**: (`offset`) => `void`

#### Parameters

##### offset

`number`

#### Returns

`void`

***

### setTokens()

> **setTokens**: (`tokens`) => `void`

#### Parameters

##### tokens

[`GalleryToken`](../../../lib/galleryFeed/interfaces/GalleryToken.md)[]

#### Returns

`void`

***

### tokens

> **tokens**: [`GalleryToken`](../../../lib/galleryFeed/interfaces/GalleryToken.md)[]
