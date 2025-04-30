# ItemMedicalSetAnimation

### Syntax

`ItemMedicalSetAnimation(item_id, animation);`

**Returns** “*<strong>true</strong>*“, if successful, otherwise it will crash.

| **Argument** | **Type** | **Description**                     |
| :----------- | :------- | :-------------------------------------- |
| item_id      | String   | The name of the item to update.       |
| animation    | String   | ID of animation/image.                |

Changes the animation used while this item is being consumed.

The animation must already be made using SpriteLoad()

### Example:

```
SpriteLoad("daves_dance_animation","daves_medical_animation.png",1,0,0,0) 
ItemMedicalSetAnimation("daves_magical_pills", "daves_dance_animation") 
```

The above code will change the item called "daves_magical_pills" so that when its being consumed the players sprite will change to be "daves_medical_animation.png"