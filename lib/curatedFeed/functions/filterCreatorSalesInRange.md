[**REJKT.xyz Feed and Filter System Documentation v0.1.0**](../../../README.md)

***

[REJKT.xyz Feed and Filter System Documentation](../../../modules.md) / [lib/curatedFeed](../README.md) / filterCreatorSalesInRange

# Function: filterCreatorSalesInRange()

> **filterCreatorSalesInRange**(`listing`, `minXtz`, `maxXtz`): `Promise`\<`boolean`\>

Filter: Include listings where the creator has total sales in the [minXtz, maxXtz] range.
(Combines listings_sold and offers_accepted.)

## Parameters

### listing

[`BaseListing`](../interfaces/BaseListing.md)

### minXtz

`number`

### maxXtz

`number`

## Returns

`Promise`\<`boolean`\>
