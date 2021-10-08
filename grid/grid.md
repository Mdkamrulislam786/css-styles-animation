#### Grid

diff ways to write grid-temeplates / defining columns and rows

```
grid-template-columns: 100px 100px 50px;
grid-template-rows: 50px 50px 200px;
<!-- or -->
grid-template-columns: 1fr 2fr 1fr
grid-template-columns:repeat(1, 1fr 2fr 1fr)
grid-template-rows:repeat(2,50px)
grid-template: repeat(2, 50px) / repeat(1, 1fr 2fr 1fr)
(row, columns)
```

#### positioning items

defing how much space(row or column) a item is going to get

```
grid-column: grid-column-start / grid-column-end;
grid-column: 1 / (-1 | span 2 | 3);
grid-rows: 1 / (-1 | span 2 | 3);
```

using grid-template-areas

```
.container{
grid-template-areas:
'h h h h h h h h h h h h'
'm c c c c c c c c c c c'
'f f f f f f f f f f f f';
}

.header{
    grid-area: h;
}
.menu{
    grid-area: m;
}
.footer{
    grid-area: f;
}
```

### auto-fit , minmax

```
 grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
 grid-template-rows: repeat(2, 100px);
```
