
If you go to the parser crate and type

```
rg usage
```

You will see in parse/def.rs

```
//Add commands comments to signature usage
signature.usage = call.comments_joined();
```

Block is defined in nu-protocol under hir.rs

```rust
pub struct Block {
    pub params: Signature,
    pub block: Vec<Group>,
    pub definitions: IndexMap<String, Block>,
    pub span: Span,
}
```
