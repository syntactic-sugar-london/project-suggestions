# Libra

## Language

Scala

## Description

Libra is a dimensional analysis library for Scala based on dependent types.  It provides compile time safety by using typelevel induction to encode the laws of dimensional analysis.

- Github: https://github.com/to-ithaca/libra
- Website: https://to-ithaca.github.io/libra/


Libra is a fairly young project, and has been around for just under a year.  Nevertheless, it's gaining traction as a solid dimensional analysis library.  It's main areas of focus as a growing project are:

 - Adding new dimensions and units.  This will become much easier once the unit conversion issue (detailed below) is resolved
 - Adding compat modules with other libraries.  The most interesting is probably refined.
 - Docs, docs, docs.  Some of the more complex areas, such as rolling custom dimensions, could do with better examples and explanations.


## Target Issues

- Anything that's labelled as a *good first issue* is good for first time contributors.
- If you want to explore typelevel induction, and shapeless, [implicitly chaining conversion factors](https://github.com/to-ithaca/libra/issues/50) is an interesting challenge.
- If you're interested in refinement types, [adding support for refined](https://github.com/to-ithaca/libra/issues/39) would be fun to explore.  This is an open ended issue to explore the possibilities of compat.

## Setup Instructions

There's a brief guide on [setting up Libra](https://github.com/to-ithaca/libra/blob/master/CONTRIBUTING.md#build-the-project).  It's a Scala project built using sbt.

## Representative

@zainab-ali is a maintainer of libra, and would be on site to represent it.
