load("@io_bazel_rules_go//go:def.bzl", "go_prefix", "go_library", "go_test")

go_prefix("github.com/twpayne/go-geom")

go_library(
    name = "go_default_library",
    srcs = [
        "bounds.go",
        "flat_area.go",
        "flat_deflate.go",
        "flat_geom0.go",
        "flat_geom1.go",
        "flat_geom2.go",
        "flat_geom3.go",
        "flat_inflate.go",
        "flat_length.go",
        "geom.go",
        "linearring.go",
        "linestring.go",
        "multilinestring.go",
        "multipoint.go",
        "multipolygon.go",
        "point.go",
        "polygon.go",
    ],
    visibility = ["//visibility:public"],
)

go_test(
    name = "go_default_test",
    srcs = [
        "area_test.go",
        "bounds_test.go",
        "geom_test.go",
        "length_test.go",
        "linearring_test.go",
        "linestring_test.go",
        "method_test.go",
        "multilinestring_test.go",
        "multipoint_test.go",
        "multipolygon_test.go",
        "point_test.go",
        "polygon_test.go",
    ],
    library = ":go_default_library",
)
