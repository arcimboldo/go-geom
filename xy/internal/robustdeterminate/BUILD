load("@io_bazel_rules_go//go:def.bzl", "go_library", "go_test")

go_library(
    name = "go_default_library",
    srcs = ["robust_determinate.go"],
    visibility = ["//xy:__subpackages__"],
)

go_test(
    name = "go_default_xtest",
    srcs = ["robust_determinate_test.go"],
    deps = [":go_default_library"],
)
