# Vending machine
## Security
- VS1 - The system shall identify whether or not money is American and valid, or counterfeit(ref. TODO).
- VS2 - The system shall be accessible only by the owner, through a key, otherwise the internal inventory remains secured and inaccessible to others.
- VS3 - The system shall determine whether or not credit/debit cards have sufficient funds to cover the transaction(ref. TODO).
## Maintenance
- VMA1.  VMA1.  The system shall provide a refrigerant system that maintains a consistant temperature of drinks in 
         inventory (Ref. TODO) at a temperature range between 38 and 45 degrees fahrenheiht.

- VMA2.  The system shall detect conditions that prevent the vending system from dispensing drinks as requested 
         by the customer from the interface (Ref TODO).

-  VMA3.  The system shall provide secure access (Ref. TODO) to inventory shelving (Ref. TODO) for the purposes of 
           replenishing the drink inventory (Ref. TODO)

## Money
- Return change
  -M1 - The change dispensing system shall return the appropriate amount of change when the customer inserts change or cash.   
  -M2 - The change dispensing system shall display money still needed to pay for purchase.
- Senses if the money compartment is full
  -MC1 - The system shall display money compartment is full message.
  -MC2 - The system shall display money compartment coins status per coin.
  -MC3 - The change dispensing systen shall provide space for each of the pennies(1 Cent)/nickels(5 Cents)/dimes(10 Cents)/quarters(25 Cents).
  -MC4 - The change dispensing system shall limit coin category maximum(full) capacity per coin.
  -MC5 - The change dispensing system shall provide space for $1.00, $5.00, $10.00, $20.00 bills.
  -MC6 - The change dispensing system shall limit cash category maximum(full) capacity per bill.
- Senses if the change drawer is empty
  -MCD1 - The system shall display change drawer is empty message.
## Interface (GREG) testing...
- Receives money

- Displays products & prices

- Provides product selector

- Scans credit/debit cards

- Notify when a product is not available

- Notify when insufficient currency has been provided
   

## Vending
### Maintains an inventory
- [ ] VI1 - The system shall provide shelving appropriate for canned beverages.
- [ ] VI2 - The system shall provide space for up to 12 categories of beverage.
- [ ] VI3 - The system shall uniquely identify drink categories.
- [ ] VI4 - The system shall maintain a count of beverages in each drink category.

### Vend products selected
- [ ] VV1 - Upon receiving a drink selection (ref. TODO), when the specified quantity of currency for the selected category has been inserted (ref. TODO), and while drinks are in inventory to vend (ref. VI4) the system shall dispense at most one of the selected category of drink.

- [ ] VV2 - Upon vending a drink (ref. VV1), the system shall reduce the inventory count (ref. VI4) for the drink category by one prior to accepting further user input.

