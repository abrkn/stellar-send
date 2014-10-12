stellar-send
===

Command-lnie utilities for preparing, signing and broadcasting Stellar transactions.

Installation
---

`npm install -g stellar-send`

Usage
---

### prepare

Prepare a transaction for offline signing:

```
stellar-prepare --account gFrom --destination gTo --amount 1000000
```

If the amount is STR, then specify as drops (multiply by 1 million)

### sign

Sign a prepare transaction:

```
stellar-sign --secret sAccountSecret --tx '{tx:"json"}'
```

### broadcast

Broadcast a signed transaction:

```
echo TRANSACTIONHEX | stellar-broadcast
```

### send a payment

```
stellar-payment --account aAccount --secret sSecret --amount 1234
```

License
---

ISC
