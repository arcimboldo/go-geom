load("@io_bazel_rules_go//go:def.bzl", "go_library", "go_test")

go_library(
    name = "go_default_library",
    srcs = ["big_cga.go"],
    visibility = ["//visibility:public"],
    deps = [
        "//:go_default_library",
        "//xy/orientation:go_default_library",
    ],
)

go_test(
    name = "go_default_xtest",
    srcs = [
        "big_cga_examples_test.go",
        "big_cga_test.go",
    ],
    deps = [
        ":go_default_library",
        "//:go_default_library",
        "//xy/orientation:go_default_library",
    ],
)
