## Object: kellysCoffee

### Attributes:
- `var temperatureDegreesF = 97.1`
- `var takenWithCream = false`
- `var originCountry = "Colombia"`
- `var pH = 4.4`
- `var aroma = "fruity"`
- `var roastLevel = ""` (assigned with `calculateRoastLevel` method below)

### Methods:
**results of `addCream`**
- `takenWithCream = true`
- `pH = 4.55`
- `temperatureDegreesF = 92.1`

**results of `tellAboutOrigin`**
- the console logs `"These beans were grown on a farm in Colombia.")`

**results of `coolOff`**
- assuming this is done after `addCream` method then `temperatureDegreesF = 82.1`
- if done without/before `addCream` then `temperatureDegreesF = 87.1`

**results of `calculateRoastLevel`**
- `roastLevel = "light"` (evaluates to same whether or not `addCream` method has been performed)
