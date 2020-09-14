## Class: CupOfCoffee

### Attributes:
- `temperatureDegreesF` (float)
- `isTakenWithCream` (boolean)
- `originCountry` (string)
- `pH` (float)
- `aroma` (string)
- `roastLevel` (string)

### Methods:

**`addCream` (modifies `takenWithCream`, `pH`, and `temperatureDegreesF`, )**

- assigns `takenWithCream` to `true`
- reassigns `pH` to a value 0.15 higher than its starting value (e.g. if `pH = 4.8`, this method evaluates `4.8 + 0.15` and reassigns `pH` to the result, which is `4.95`)
- reassigns `temperatureDegreesF` to a value 5 lower than its starting value (e.g. if `temperatureDegreesF = 90.7`, this method evaluates `90.7 - 5` and reassigns `temperatureDegreesF` to the result, which is `85.7`)


**`tellAboutOrigin` (uses `originCountry`)**

- prints concatenation of predetermined string and value of `originCountry`:
`console.log("These beans were grown on a farm in " + originCountry + ".")`

**`coolOff` (modifies `temperatureDegreesF`)**

- reassigns `temperatureDegreesF` to a value 10 lower than its starting value (e.g. if `temperatureDegreesF = 85.7`, this method evaluates `85.7 - 10` and reassigns `temperatureDegreesF` to the result, which is `75.7`)

**`calculateRoastLevel` (modifies `roastLevel` and uses `acidity`, `aroma`, `takenWithCream`)**

- conditional function that assigns a string value to `roastLevel` depending on the values of `acidity`, `aroma`, and `takenWithCream`:

```
if ((aroma == "fruity") && (((pH < 4.6) && (takenWithCream = false)) || ((pH < 4.75) && (takenWithCream = true)))) {
roastLevel = "light";
} else if ((aroma == "nutty") && (((pH > 4.6) && (pH < 5.2) && (takenWithCream = false)) || ((pH > 4.75) && (pH < 5.35) && (takenWithCream = true)))) {
roastLevel = "dark";
} else if (
  ((aroma = "fruity") && (((pH > 4.6) && (pH < 5.2) && (takenWithCream = false)) || ((pH > 4.75) && (pH < 5.35) && (takenWithCream = true)))) ||  ((aroma == "nutty") && (((pH < 4.6) && (takenWithCream = false)) || ((pH < 4.75) && (takenWithCream = true))))) {
  roastLevel = "medium";
} else {
  roastLevel = "burnt or worse"
}
```
