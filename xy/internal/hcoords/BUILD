load("@io_bazel_rules_go//go:def.bzl", "go_library", "go_test")

go_library(
    name = "go_default_library",
    srcs = ["hcoords.go"],
    visibility = ["//xy:__subpackages__"],
    deps = ["//:go_default_library"],
)

go_test(
    name = "go_default_xtest",
    srcs = ["hcoords_test.go"],
    deps = [
        ":go_default_library",
        "//:go_default_library",
    ],
)
