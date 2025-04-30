# Weapon Script Events

When creating weapons you'll be able to assign functions to various events. Below is a list of the events and their behaviors.

| **Event IDs** | Descriptions | Arguments | Function Example |
|---|---|---|---|
| "weapon_fire" | Occurs when the weapon is fired. Runs within the context of the player instance. | Player Instance | `WeaponSetScript("weapon", "weapon_fire",func(_inst){})` |
| "weapon_reload" | Occurs when the weapon is reloaded. Runs within the context of the player instance. | Player Instance | `WeaponSetScript("weapon", "weapon_fire",func(_inst){})` |
| "bullet_spawn" | Occurs when the weapon is fired. Runs within the context of the bullet instance. | Bullet Instance | `WeaponSetScript("weapon", "bullet_spawn", func(_inst){})` |