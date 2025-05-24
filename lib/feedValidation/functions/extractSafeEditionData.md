[**REJKT.xyz Feed and Filter System Documentation v0.1.0**](../../../README.md)

***

[REJKT.xyz Feed and Filter System Documentation](../../../modules.md) / [lib/feedValidation](../README.md) / extractSafeEditionData

# Function: extractSafeEditionData()

> **extractSafeEditionData**(`item`): `object`

Safely extracts edition data (amount left and total supply)

## Parameters

### item

`any`

Feed item (BaseListing, ArtistListing, or GalleryToken)

## Returns

`object`

Object containing amount and supply (both could be null if not available)

### amount

> **amount**: `null` \| `number`

### supply

> **supply**: `null` \| `number`
