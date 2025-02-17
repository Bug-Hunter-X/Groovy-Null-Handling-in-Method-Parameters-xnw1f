# Groovy Null Handling in Method Parameters

This repository demonstrates a subtle bug related to null handling in Groovy methods.  The `myMethod` function aims to return either `a`, `b`, or their sum, but the behavior with null values might not be immediately intuitive.

## Bug Description

The core issue arises from the use of `==` for null checks, and Groovy's dynamic typing. While seemingly straightforward, this can lead to unexpected behavior depending on the specific input types and implicit conversions performed.

## How to Reproduce

1. Clone this repository.
2. Run `groovy bug.groovy`.
3. Observe the output, noting the behavior when both `a` and `b` are null.

## Solution

The solution involves explicit null checks and type handling to clarify the expected behavior.