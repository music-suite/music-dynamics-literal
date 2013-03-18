
# music-dynamics-literal

Overloaded dynamic level literals for Haskell. 

This package allow you to write the dynamic levels of musical notation as expressions overloaded on result type. This works exactly like numeric literals (and string literals when using the `OverloadedStrings` extension).

For example:

```haskell
import Music.Dynamics.Literal

frere :: Dynamic a => [a]

frere1 =  [pp, cresc, _f] 
       ++ [ppp `crescFromTo` mf]
       ++ [sfz]
```

## Requirements

* [Haskell Platform](http://www.haskell.org/platform)

## Installation

    cabal configure
    cabal install
