# Blue Wave Token (ERC20-Token)

## Overview

This is simple ERC20 token smart contract that uses the [OpenZeppelin Contract library](https://www.openzeppelin.com/contracts) with an added `mint` and `burn` token functionalities.

### Demo Video
https://www.loom.com/share/29d4ddda02c547c5bcd47d85747aabbc?sid=87fe5291-8f87-45fd-91fa-4159b659beca



### Token Information

- **Name:** Blue Wave Token
- **Symbol:** BWT
- **Maximum Supply:** 1000e18

### Functions

`Constructor` Initializes the ERC-20 token with the specified name and symbol.

- Sets the contract deployer as the owner.
- Mints and InitialSupply of `1e18` to the owner.

`mint(address \_to, uint \_amount)`,allows only the owner of the contract to mint new tokens.

- Checks to ensure that amount is not more than `MAXIMUM_SUPPLY`and then
- Mints new tokens and assigns them to the specified address.

`burn(uint \_amount)`, allows users to burn their token

- Checks to ensures that the caller has a sufficient balance to burn.
- Burns a specified amount of tokens from the caller's balance.

### Contract Interactions

- The contract owner can mint new tokens using the `mint` function.
- Any address can burn their tokens using the `burn` function, provided they have a sufficient balance.


## Author

Ugo Mars
[@metacraftersio](https://github.com/UgoMars)

## License

This project is licensed under the MIT License - see the LICENSE.md file for details.
