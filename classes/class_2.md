## Class: Table

### Attributes:
- `tableNumber` (integer)
- `waiter` (string)
- `isReserved` (boolean)
- `numberOfSeats` (integer)
- `customersSeated` (array)
- `isSet` (boolean)

### Methods:

**`addCustomer` (modifies `customersSeated`)**

- adds name of customer, a string (e.g. "Joe"), to the array `customersSeated` using `push()` array method

**`setTable` (uses `customersSeated`, `isSet`, `tableNumber` and `waiter` to modify `isSet` and print a string)**

- If there are no customers seated and the table is not set, this method logs a command telling the waiter to set the table and reassigns the value of `isSet` to true:
  ```
  if (customersSeated.length === 0 && isSet === false) {
    console.log(waiter + ", go set Table " + tableNumber);
    isSet = false;
  } else {
    console.log("Table " + tableNumber + " is ready");
  }
  ```

**`introduceWaiter` (uses `waiter`)**

- logs concatenation of string "Hello, my name is " and value of `waiter`

**`reserveTable` (modifies `isReserved` and `customersSeated`)**

- reassigns `isReserved` to `true`
- removes all items from `customersSeated` array by looping the `pop()` array method for as many items as their are in the array
