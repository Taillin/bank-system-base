# Bank System

> A console-based Java banking application that simulates real bank operations — account management, transactions, bill payments and admin controls — built with core data structures.

## Features

- **Bank mode** — Deposit, withdraw, view transaction history, undo last transaction, pay bills
- **ATM mode** — Check balance and withdraw money
- **Admin mode** — Approve account requests, manage bill queue, view all accounts
- **Transaction history** — Undo last operation with Stack
- **Bill queue** — FIFO processing of payment requests
- **Account requests** — Users submit requests, admin approves them

## Tech Stack

- **Language:** Java
- **Data Structures:** `LinkedList`, `Stack`, `Queue`, `Array`
- **I/O:** Java Scanner (console)

### Main menu

```
--- Bank System ---
1. Enter Bank
2. Enter ATM
3. Admin Area
0. Exit
```

## Project Structure

```
src/
├── BankAccount.java   # Account entity (deposit, withdraw)
└── BankSystem.java    # Main logic + menus (Bank / ATM / Admin)
```

## Data Structures Used

| Structure | Usage |
|-----------|-------|
| `LinkedList<BankAccount>` | Stores all bank accounts |
| `Stack<String>` | Transaction history (supports undo) |
| `Queue<String>` | Bill payment queue (FIFO) |
| `Queue<BankAccount>` | Account requests awaiting admin approval |
| `BankAccount[]` | Initial static account data |

## Key Learnings

- Practical use of `Stack` for undo functionality
- `Queue` for FIFO request and bill processing
- `LinkedList` as dynamic account storage
- Designing multi-role systems (User / ATM / Admin)

## Author

**Yermakov Ilya**
