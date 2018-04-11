# Scalaz

## Language

Scala

## Description

Scalaz is a Scala library for functional programming.  It contains purely functional data structures, typeclasses and corresponding instances.

- GitHub: https://github.com/scalaz/scalaz
- Developer guide: https://github.com/scalaz/scalaz/blob/series/7.3.x/CONTRIBUTING.md

Our main focus will be on a subset of issues relating to [scalaz-deriving](https://gitlab.com/fommil/scalaz-deriving), which provides semi-automatic typeclass derivation.

Take a look at [#1](https://github.com/syntactic-sugar-london/project-suggestions/issues/1) for some more background.


## Target Issues

- [#1662](https://github.com/scalaz/scalaz/issues/1662) fromIso everywhere.

  This adds a `fromIso` function to each typeclass, which lets us do generic derivation of `F[_]` shaped things as per the `MonadErrorTest`.
  This will later be used to create a `@ideriving` annotation in scalaz-deriving - take a look at [scalaz-deriving#74](https://gitlab.com/fommil/scalaz-deriving/issues/74) for the bigger picture.
  This is suitable for Scalaz 7.2.

- [#1618](https://github.com/scalaz/scalaz/issues/1618) Laws for codivide and coapplicative

  This ticket covers all the loose ends, but we're interested in `Codivide` and `Coapplicative` laws in particular.

  `Codivide` and `Coapplicative` are the coproduct analogues of `Divide` and `Applicative` respectively.  You'll need to have a think about what laws these need.


- [#1658](https://github.com/scalaz/scalaz/issues/1658) Monad Reader needs laws.

  This adds laws to the currently lawless MonadReader.  Some decent laws have been detailed in [mtl#5](https://github.com/haskell/mtl/issues/5) in the mtl library in Haskell, which this can be extended to.  This is suitable for Scalaz 7.3.

## Setup Instructions

The contributor's guide has a section on [setting up the project](https://github.com/scalaz/scalaz/blob/series/7.3.x/CONTRIBUTING.md#building-and-testing-scalaz-locally).

## Representative

@zainab-ali on behalf of @fommil, the author of [scalaz-deriving](ttps://gitlab.com/fommil/scalaz-deriving)
