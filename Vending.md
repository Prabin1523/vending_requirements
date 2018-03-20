# Vending machine
## Security
- Ensures money is real
- Secures internal inventory
- Validates credit/debit cards

## Maintenance
- Runs a refrigerant system

- Senses issues with the vending system

- Provides a method of restocking

## Money
- Return change

- Senses if the money compartment is full

- Senses if the change drawer is empty

## Interface
### Receives money
- IR1 - The system shall provide a means of receiving paper currency.
- IR2 - The system shall provide a means of receiving coin currency.
- IR3 - The system shall provide a means of reading a credit/debit card.
- IR4 - Upon receiving paper currency (ref. IR1), when the currency is determined to be real (ref. TODO), the system shall identify the amount of the currency.
- IR5 - Upon receiving coin currency (ref. IR2), when the currency is determined to be real (ref. TODO), the system shall identify the amount of the currency.
- IR6 - Upon identifying the amount of currency received (ref. IR1 and IR2), the system shall update the amount received.
- IR7 - Upon update of amount received (ref. IR6), the system will hold any authorization for 60 seconds or beverage dispensed or canceled.
- IR8 - Upon update of amount received (ref. IR6), the system will hold any currency received until beverage dispensed or canceled.

### Displays products & prices
- ID1 - The system will provide a means of selecting 12 unique categories of beverages.
- ID2 - The system will provide a means of identifying the price of each of the 12 unique categories.
- ID3 - 

### Provides product selector

### Scans credit/debit cards
- IS1 - Upon reading a credit/debit card, the system will initiate credit/debit authorization.

### Notify when a product is not available

### Notify when insufficient currency has been provided
   

## Vending
### Maintains an inventory
- VI1 - The system shall provide shelving appropriate for canned beverages.
- VI2 - The system shall provide space for up to 12 categories of beverage.
- VI3 - The system shall uniquely identify drink categories.
- VI4 - The system shall maintain a count of beverages in each drink category.

### Vend products selected
- VV1 - Upon receiving a drink selection (ref. TODO), when the specified quantity of currency for the selected category has been inserted (ref. TODO), and while drinks are in inventory to vend (ref. VI4) the system shall dispense at most one of the selected category of drink.

- VV2 - Upon vending a drink (ref. VV1), the system shall reduce the inventory count (ref. VI4) for the drink category by one prior to accepting further user input.

