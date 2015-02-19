## Snap Grid

```scss
// Asymmetric grid and the gutter width of the grid to snap to.
@include add-grid(snap(2 4 4 2, 1/3));
```

<img src="img/snap.png">

<p class="small">
  This is most useful if you're using a symmetric and an asymmetric grid near
  each other and the gutters need to align. Remember that the <em>sum</em> of
  the asymmetric widths needs to equal the number of columns in the matching
  symmetric grid.
</p>
