# go-geom

Package geom implements efficient geometry types.

See https://godoc.org/github.com/twpayne/go-geom.

Example:

```go
func ExampleNewPolygon() {
	unitSquare := NewPolygon(XY).MustSetCoords([][][]float64{
		{{0, 0}, {1, 0}, {1, 1}, {0, 1}, {0, 0}},
	})
	fmt.Printf("unitSquare.Area() == %f", unitSquare.Area())
	// Output: unitSquare.Area() == 1.00000
}
```

[License](LICENSE)