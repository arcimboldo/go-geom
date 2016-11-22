load("@io_bazel_rules_go//go:def.bzl", "go_library", "go_test")

go_library(
    name = "go_default_library",
    srcs = [
        "line_intersector.go",
        "nonrobust_line_intersector.go",
        "robust_line_intersector.go",
        "test_data.go",
    ],
    visibility = ["//xy:__subpackages__"],
    deps = [
        "//:go_default_library",
        "//bigxy:go_default_library",
        "//xy/internal:go_default_library",
        "//xy/internal/centralendpoint:go_default_library",
        "//xy/internal/hcoords:go_default_library",
        "//xy/lineintersection:go_default_library",
        "//xy/orientation:go_default_library",
    ],
)

go_test(
    name = "go_default_test",
    srcs = [
        "nonrobust_line_intersector_test.go",
        "robust_line_intersector_test.go",
    ],
    library = ":go_default_library",
)
