<p align="center">
<img src="https://res.cloudinary.com/droqoz7lg/image/upload/c_pad,ar_1:1/v1705943138/math-master_ctp4wc.png" width="400" alt="math-master">
<br/>

# Contest Details

### Prize Pool

- High - 100xp
- Medium - 20xp
- Low - 2xp

- Starts: January 25, 2024 Noon UTC
- Ends: January 02, 2024 Noon UTC

### Stats

- nSLOC: 46
- Complexity Score: 276

# Math Master

_This codebase was inspired by the [solady](https://github.com/Vectorized/solady), [obront.eth](https://twitter.com/zachobront), and [solmate](https://github.com/transmissions11/solmate) codebases. Huge thanks to [karma](https://twitter.com/0xkarmacoma) for the help on FV with Halmos.... which may be a hint._

_We will teach how to do Formal Verification and assembly in the upcoming Cyfrin Updraft course._

- [Contest Details](#contest-details)
    - [Prize Pool](#prize-pool)
    - [Stats](#stats)
- [Math Master](#math-master)
- [About](#about)
- [Getting Started](#getting-started)
  - [Requirements](#requirements)
  - [Quickstart](#quickstart)
- [Usage](#usage)
  - [Testing](#testing)
    - [Test Coverage](#test-coverage)
- [Audit Scope Details](#audit-scope-details)
  - [Compatibilities](#compatibilities)
- [Roles](#roles)
- [Known Issues](#known-issues)

# About

Welcome to the future of web3! We, the math MASTERS are titans of the algebraic and gas efficient. We have created a small library called `MathMasters` where we have the following functions/terms defined:

- `WAD`: fixed point decimal with 18 decimals (for basic quantities, e.g. balances)
- `mulWad`: Equivalent to `(x * y) / WAD` rounded down.
- `mulWadUp`: Equivalent to `(x * y) / WAD` rounded up.
- `sqrt`: Returns the square root of `x`.

We hope that people will use our hype optimized functions to make better codebases.

We are especially concerned with any function doing something "weird" at the EVM/assembly level. We would consider any of the following a valid LOW severity rating:

- Incorrect storage slot packaging
- Overriding the [solidity free memory pointer](https://docs.soliditylang.org/en/latest/internals/layout_in_memory.html)
- Any out of gas errors
- Incorrect use of function selectors

We expect any solidity project using version `^0.8.3` or above should be able to use our codebase. If not, that should be considered a vulnerability as well.

This is a great chance to test out your fuzzing and Formal Verification skills.

# Getting Started

## Requirements

- [git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git)
  - You'll know you did it right if you can run `git --version` and you see a response like `git version x.x.x`
- [foundry](https://getfoundry.sh/)
  - You'll know you did it right if you can run `forge --version` and you see a response like `forge 0.2.0 (816e00b 2023-03-16T00:05:26.396218Z)`
- [Halmos](https://github.com/a16z/halmos)
  - To know you've installed it run `halmos --version` and you should see something like `halmos 0.1.0 (816e00b 2023-03-16T00:05:26.396218Z)

## Quickstart

```
git clone https://github.com/Cyfrin/2024-01-math-master
cd 2024-1-math-master
make
```

# Usage

## Testing

```
forge test
```

### Test Coverage

```
forge coverage
```

and for coverage based testing:

```
forge coverage --report debug
```

# Audit Scope Details

- Commit Hash:
- In Scope:
  (For this contest, just use the main branch)

```
Hash:
```

## Compatibilities

- Solc Version: `0.8.3 < 0.9.0`
- Chain(s) to deploy contract to:
  - Ethereum
- Tokens:
  - None

# Roles

None

# Known Issues

None
