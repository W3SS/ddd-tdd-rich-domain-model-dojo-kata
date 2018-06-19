# Small .NET Standard solution with DDD Building Blocks covered with Unit Tests [![Build status](https://ci.appveyor.com/api/projects/status/ujilt0luhnvpm4to?svg=true)](https://ci.appveyor.com/project/ivanpaulovich/ddd-tdd-rich-domain) [![codecov](https://codecov.io/gh/ivanpaulovich/ddd-tdd-rich-domain/branch/master/graph/badge.svg)](https://codecov.io/gh/ivanpaulovich/ddd-tdd-rich-domain)

We designed the Finance Domain using Aggregate Roots, Entities and Value Objects and we covered the uses cases with Unit Tests, run them in your first time here. The Domain and Unit Tests projects were implemented with .NET, the classes are as closed as possible.

## :gem: Compiling from source

To run Acerola from source, clone this repository to your machine, compile and test it:

```sh
git clone https://github.com/ivanpaulovich/ddd-tdd-rich-domain.git
./build.sh
```

## :construction_worker: Use cases

This project was designed do cover the following use cases:

1. The customer should be able to register a new account.
2. Allow to deposit into an account.
3. Allow to withdraw from an account.
4. Accounts can only be closed if they have zero balance.
5. Do not allow to withdraw more than the account balance.

The following diagram shows the bounded contexts:

## :memo: Good to know

Aggregate Roots
1. Customer
2. Account

Entities
1. Customer
2. Account
3. Credit
3. Debit

Value Objects
1. SSN
2. Name
3. Amount

## :computer: Tech stuff

* .NET Core / Standard
* xUnit
* Moq
