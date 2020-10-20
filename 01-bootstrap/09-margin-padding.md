# Bootstrap Margin and Padding

Formats: 
- `{property}{sides}-{size}` for `xs`
- `{property}{sides}-{breakpoint}-{size}` for `sm`, `md`, `lg`, and `xl`

Property:
- `m` - for margin
- `p` - for padding

Specify a side:
- `t` or `b` - top or bottom
- `l` or `r` - left or right
- `x` or `y` - left+right or top+bottom
- leave the side out to specify all 4 sides

Specify a size:
- `0` - none
- `1` to `5` - increasing space
- `auto` - for classes that specify margin to auto

## Examples
```html
<div class="p-3 m-auto">Lorem ipsum</div>
<div class="p-3 pb-2 pb-md-0">Lorem ipsum</div>
```
