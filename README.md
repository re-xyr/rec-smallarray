# rec-smallarray

An immutable extensible record type based on `SmallArray`s, intended to provide fast reads on small structures.

## Asymptotics

- Index: Amorized `O(1)` with low constant factor
- Update: `O(n)`
- Slice: `O(1)`
- Cons: `O(n)`

Note that this structure slows down GC when its size exceeds 128.

## Contribution

This library started out as a module in [`cleff`](https://github.com/re-xyr/cleff), an extensible effects library, and it needs to continue accommodating that. Contribution is welcome as long as it does not impede this library's performance nor increase its dependency footprint.
