# ItemArmorSetAnomaly

### Syntax

`ItemArmorSetAnomaly(item_id, anomaly);`

**Returns** “*true*“, if successful, otherwise it will crash.

| **Argument** | **Type** | **Description**                                 |
| :----------- | :------- | :---------------------------------------------- |
| item_id      | String   | The name of the item to update.                 |
| anomaly      | Real     | When equipped how much defence from Anomaly. |

When equipped provides reduced damage from anomaly. This value should normally be between 0 and 75 with 75 providing the best defence against Anomaly.