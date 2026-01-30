Economy System

## Scope

Systems in this category may include:
- Currency management
- Player balances and resource tracking
- Economy-related services used by shops or progression systems

Monetization logic, UI, and game-specific rules are intentionally kept separate to
ensure systems remain reusable and easy to extend.

---

## Design Principles

- **Server Authority**  
  All economy values are managed on the server. Clients never directly modify
  currency or resources.

- **Single Source of Truth**  
  Player balances are stored and updated in one controlled location to prevent
  desyncs or exploits.

- **Modularity**  
  Systems are designed to be used independently and called by other server-side
  systems rather than tightly coupled to gameplay code.

- **Readability & Maintainability**  
  Code is structured to be easy to understand, debug, and expand over time.

---

## Current Systems

- **CurrencySystem**  
  Handles loading, saving, and modifying a player’s in-game currency in a secure
  and server-authoritative way.

---

## Notes

These systems are intended as portfolio examples that demonstrate architecture,
best practices, and multiplayer-safe design. Feature scope is kept focused to
prioritise clarity and correctness over complexity.
