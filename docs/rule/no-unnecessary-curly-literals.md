# no-unnecessary-curly-literals

literals need not be wrapped in the mustache expressions.

## Examples

This rule **forbids** the following:

```hbs
<FooBar class={{"btn"}} />
```

```hbs
<FooBar value={{12345}} />
```

```hbs
<FooBar value={{true}} />
```

```hbs
<FooBar value={{undefined}} />
```

```hbs
<FooBar value={{null}} />
```

```hbs
<FooBar class="btn">{{"Hello"}}</FooBar>
```

This rule **allows** the following:

```hbs
<FooBar class="btn" />
```

```hbs
<FooBar class="btn">Hello</FooBar>
```

```hbs
<FooBar value=12345 />
```

```hbs
<FooBar value=true />
```

```hbs
<FooBar value=undefined />
```

```hbs
<FooBar value=null />
```

## References

* Ember's [Helper Functions](https://guides.emberjs.com/release/components/helper-functions/) guide
