# Pair Adjacent Violators

## Overview

An implementation of the [Pair Adjacent Violators](http://gifi.stat.ucla.edu/janspubs/2009/reports/deleeuw_hornik_mair_R_09.pdf) algorithm for [isotonic regression](https://en.wikipedia.org/wiki/Isotonic_regression).  Written in Kotlin, but usable from any language that can use Java libraries (including Java itself, of course).

Note this algorithm is also known as "Pool Adjacent Violators".

## Usage

### Adding library dependency

You can use this library by adding a dependency for Gradle, Maven, SBT, Leiningen or another Maven-compatible dependency management system thanks to Jitpack:

[![](https://jitpack.io/v/trystacks/pairAdjacentViolators.svg)](https://jitpack.io/#trystacks/pairAdjacentViolators)

### Kotlin usage

```kotlin
import com.trystacks.pav.PairAdjacentViolators
import com.trystacks.pav.PairAdjacentViolators.*
// ...
val inputPoints = listOf(Point(3.0, 1.0), Point(4.0, 2.0), Point(5.0, 3.0), Point(8.0, 4.0))
val pav = PairAdjacentViolators(inputPoints)
val interpolator = pav.interpolator()
println("Interpolated: ${interpolator(6.0)}")
```
### License
Released under the [LGPL](https://en.wikipedia.org/wiki/GNU_Lesser_General_Public_License) version 3 by [Stacks](http://trystacks.com/).
