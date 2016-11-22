load("@io_bazel_rules_go//go:def.bzl", "go_library", "go_test")

go_library(
    name = "go_default_library",
    srcs = [
        "angle.go",
        "area_centroid.go",
        "centroid.go",
        "cga.go",
        "convex_hull.go",
        "line_centroid.go",
        "point_centroid.go",
        "radial_comparator.go",
    ],
    visibility = ["//visibility:public"],
    deps = [
        "//:go_default_library",
        "//bigxy:go_default_library",
        "//sorting:go_default_library",
        "//transform:go_default_library",
        "//xy/internal:go_default_library",
        "//xy/internal/lineintersector:go_default_library",
        "//xy/internal/raycrossing:go_default_library",
        "//xy/location:go_default_library",
        "//xy/orientation:go_default_library",
    ],
)

go_test(
    name = "go_default_test",
    srcs = ["convex_hull_test.go"],
    library = ":go_default_library",
    deps = [
        "//:go_default_library",
        "//xy/internal:go_default_library",
    ],
)

go_test(
    name = "go_default_xtest",
    srcs = [
        "angle_examples_test.go",
        "angle_test.go",
        "area_centroid_examples_test.go",
        "area_centroid_test.go",
        "centroid_test.go",
        "cga_examples_test.go",
        "cga_test.go",
        "convex_hull_examples_test.go",
        "line_centroid_examples_test.go",
        "line_centroid_test.go",
        "point_centroid_examples_test.go",
        "point_centroid_test.go",
        "radial_comparator_examples_test.go",
        "radial_comparator_test.go",
    ],
    deps = [
        ":go_default_library",
        "//:go_default_library",
        "//xy/internal:go_default_library",
        "//xy/orientation:go_default_library",
    ],
)
