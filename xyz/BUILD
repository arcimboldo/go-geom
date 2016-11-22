load("@io_bazel_rules_go//go:def.bzl", "go_library", "go_test")

go_library(
    name = "go_default_library",
    srcs = [
        "vector.go",
        "xyz.go",
    ],
    visibility = ["//visibility:public"],
    deps = [
        "//:go_default_library",
        "//xy:go_default_library",
    ],
)

go_test(
    name = "go_default_xtest",
    srcs = [
        "vector_examples_test.go",
        "vector_test.go",
        "xyz_examples_test.go",
        "xyz_test.go",
    ],
    deps = [
        ":go_default_library",
        "//:go_default_library",
    ],
)
