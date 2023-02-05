# no-unnecessary-curly-braces-for-strings

🔧 The `--fix` option on the command line can automatically fix some of the problems reported by this rule.

string values need not be wrapped in the mustache expressions.

## Examples

This rule **forbids** the following:

```hbs
class={{"btn"}}
```
This rule **allows** the following:

```hbs
class="btn"
```
## References

* Ember's [Helper Functions](https://guides.emberjs.com/release/components/helper-functions/) guide