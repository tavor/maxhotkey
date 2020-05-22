# maxhotkey
Generates 3DS Max key bindings and map for macro scripts based off a JSON configuration.

Inspired by [this post](https://polycount.com/discussion/82907/3ds-max-keyboard-shortcuts).
### Adding a macro
1. Create a new file in the `macros` directory and paste your MaxScript there.
2. Replace an existing `macro`'s name in config.json with the new filename or create a new `macro` with a structure like:
```    
    <key>: {
        "key": {
          "macro": {
            "name": "<your-macro-name>"
          }
        }
    },
```
 Where `<key>` can be any lowercase letter from a-z. If `<key>` is a number, use "No\<number>".

3. Add key location in keys.cfg to make hotkey appear on key map.
4. Run `python maxhotkey.py`
