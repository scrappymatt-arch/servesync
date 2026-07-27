# ServeSync preheat fix

This update fixes oven preheating.

Before:
- each oven item could generate its own preheat instruction.

Now:
- preheating belongs to the appliance, not the food;
- one oven preheats once for a continuous run at the same temperature;
- another heating step is only created when that oven genuinely needs to change temperature;
- same-temperature dishes can continue using the already-hot oven.

Example:
- 17:00 Preheat oven to 200°C
- 17:10 Chicken in
- 17:40 Potatoes in
- 17:50 Yorkshires in

There is no second or third 200°C preheat.

Upload these same 7 files over the current GitHub repository files and commit. GitHub Pages does not need to be configured again.
