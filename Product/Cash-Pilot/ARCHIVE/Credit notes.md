# Credit notes

# Why take care of it?

Credit Note can be received or sent by Business Owners through the Invoice and Expense channels.

Since they can alter the amount of cash flow a company will receive, we need to study it, understand the market use cases and how it is handled in the Shine environment.

# How it is handled at Shine for the moment?

## Invoice

- A credit note is created solely on the basis of an existing invoice.
- Creating a credit note does not change the status of the reference invoice.
- The amount of the credit note is equal to the amount of the reference invoice (as a negative figure). ONLY POSSIBILITY
- CN can be technically identified

## Expense

- CN can be stand alone or can be attached to an expense.
- You can create an expense that is a CN: first status is Unpaid, the amount is negative.
- The status remain Unpaid until there is reconciliation with a transaction, then it becomes Paid.
- You can only void CN
- CN can be technically identified

API description:

https://www.billy.dk/api/#v2bills

# Use case

Use cases that are available on the market.

#### Invoice

1. Give a full refund to a customer of product/service that was sold to him. CN attached to an Invoice. **(possible in Shine)**
2. Give a partial refund to a customer of product/service that was sold to him. CN attached to an Invoice.
3. Give a discount to a customer for a future purchase. CN not attached to an Invoice.

#### Expense

1. Receive a discount on a future purchase from a provider. CN not attached to an Expense  **(possible in Shine)**
2. Receive a partial discount on a product/service the BO bought from a provider. CN attached to an Expense **(possible in Shine)**
3. Receive a full refund on a a product/service. CN attached to an Expense. 

# Status for Cash Pilot

Since:

- Use case handling is not homogeneous between Invoice and Expense
- It is not possible to distinguish CN attached to a Invoice/Expense from independent one.
- This use case need a full study to create choose what to tackle and designs to make CN distinguishable

**Decision: the handling of Credit Note will not be added to the MVP scope of Cash Pilot.**---

## 📚 Related Documentation

**Hub:** [[../../../../Cash Pilot - Overview.md|Overview]]
**Product:** [[../../../../product-and-features.md]]
