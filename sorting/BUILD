load("@io_bazel_rules_go//go:def.bzl", "go_library", "go_test")

go_library(
    name = "go_default_library",
    srcs = ["sorting.go"],
    visibility = ["//visibility:public"],
    deps = ["//:go_default_library"],
)

go_test(
    name = "go_default_xtest",
    srcs = [
        "sorting_examples_test.go",
        "sorting_test.go",
    ],
    deps = [
        ":go_default_library",
        "//:go_default_library",
    ],
)
