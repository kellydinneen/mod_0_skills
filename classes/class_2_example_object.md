## Object: ourTable

### Attributes:
- `var tableNumber = 5`
- `var waiter = "Molly"`
- `var isReserved = false`
- `var numberOfSeats = 4`
- `var customersSeated = ["Kelly", "Livvy", "Ella"]`
- `var isSet = true`

### Methods:

**`addCustomer` results**

- adds `"Will"` to the array `customersSeated` using `push()` array method:
```
customersSeated.push("Will");
```
- so `customersSeated == ["Kelly", "Livvy", "Ella", "Will"]`

**`setTable` results**

- `customersSeated.length != 0` so the first conditional's conditional is not satisfied. The console will log : `"Table " + tableNumber + " is ready"` which comes to ``"Table 5 is ready"``

**`introduceWaiter` results**

- logs string `"Hello, my name is Molly"`

**`reserveTable` results**

- `isReserved = true`
- removes all items from `customersSeated` array by looping the `pop()` array method for all four customers now seated, so `customersSeated` is now assigned to empty array
