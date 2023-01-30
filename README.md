**Contacts for Support**
- @rupertlssmith on https://elmlang.slack.com
- @rupert on https://discourse.elm-lang.org

# elm-nonempty-set

`elm-nonempty-set` provides a variation on the `elm/core` `Set` module, for
non-empty sets.

The APIs are identicial where possibly, but have different types in places depending on the non-emptiness property.

For example in `elm/core` `Set`:

```
fromList : List comparable -> Set comparable
```

corresponds to:

```
fromList : List comparable -> Maybe (NonemptySet comparable)
```

as the list may be empty, so cannot create a non-empty set.
