1. Ensure compliance with the Eip standards( eg EIP4626 specifies how functions should be rounded)
2. Attack vector sending of assets to un address before it's deployed.
3. Gas consumption of a function
4. Breaking of functions due to failed hooks.
5. ERC 777 re-entrancy problems
6. Overflow due to casting.
7. Zero address checks are missing
8. Events are not emitted for important state changes
9. Contracts are using outdated Library(openzeppelin, solmate)
10. Misleading comments

---

### Title:

- Severity:
- Description:
- Impact
- Remediation:
- Count:
- Location:
- Code:
- Proof of Concept:

1. Solidity Visual Developer.
2. Run the code in remix.
3. Evaluate function by function.
4. Library used solmate, Openzeppelin version, Compiler used.
5. Function emit events for state changes. Possible monitoring systems.
6. Access controls of every functions. User roles in the system.
7. Pauseable function are well implemented
8. Verify input handling any potential for flash loan, Mint attacks
9. Gas usage by function potential issuficient gas grieving.
10. Business logic (Pull funds,)
11. Denial of Service.
12. Token (Starndard EIP, ERC 777, With callbacks, re-entrancy)
13. Code Clarity.
14. Test coverage against specification.
15. MEV attacks (Flash loan, Assuming balances).
16. Look at git commit history

17. Variables opportunities to pack
18. Storage layout from the compiler
19. Use Custom errors.
20. Don't initialize to zero values.
21. Modifier logic is separated.
