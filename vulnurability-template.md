### Title:

- Severity: Medium/ High/ Low/ Informational/ Quality Assurance
- Description:
- Impact:
- Remediation:
- count: 1
- locations: [GolemToken.sol#L36](https://github.com/code-423n4/2022-07-golom/blob/main/contracts/governance/GolomToken.sol#L36)
- Proof of Concept:
- Code:

```solidity
function mint(address _account, uint256 _amount) external onlyMinter {
    _mint(_account, _amount);
}
```

- Tools Used: Visual Studio.
