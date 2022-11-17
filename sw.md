1. Function Default Visibility
2. Interger overflow and Underflow
3. Outdated compiler Version
4. Floating Pragma
5. Unchecked Call return Value
6. Uprotected Ether Withdrawal
7. Uprotected selfdestruct insturction
8. reentrancy
9. state variable default visibility
10. Uninitialized Storage pointer
11. Assert Violation
12. Use of solidity deprecated solidity functions
13. Delegatecall to unstrusted callee
14. DoS with failed Call
15. Transcation Order Dependence
16. Authorizatoin through tx.origin
17. Signature malleability
18. Incorrect constructor name
19. Shadowing state variables
20. Weak Sources of randomness from chain attributes
21. Missing protection against signature replaly attacks
22. Lack of proper signature verification
23. Requirement violation
24. Write to Arbitrary Storage Location
25. Incorrect Inheritance Order
26. Insufficient Gas Griefing
27. Arbitrary Jump with Function Type Variable
28. DoS With block gas limit
29. Typographical Error
30. Right-To-Left-Override control character (U+202E)
31. Presence of unused variables
32. Unexpected ether balance
33. Hash Collisions With Multiple Variable Length Arguments
34. Message call with hardcoded gas amount
35. Code with no effects
36. Unecrypted private data on-chain

37. abi.encodePacked() should not be used with dynamic types when passing the result to a hash function such as keccak256()
    Use abi.encode() instead which will pad items to 32 bytes, which will prevent hash collisions (e.g. abi.encodePacked(0x123,0x456) => 0x123456 => abi.encodePacked(0x1,0x23456), but abi.encode(0x123,0x456) => 0x0...1230...456). "Unless there is a compelling reason, abi.encode should be preferred". If there is only one argument to abi.encodePacked() it can often be cast to bytes() or bytes32() instead. If all arguments are strings and or bytes, bytes.concat() should be used instead
