load("@io_bazel_rules_go//go:def.bzl", "go_library", "go_test")

go_library(
    name = "go_default_library",
    srcs = ["ray-crossing-counter.go"],
    visibility = ["//xy:__subpackages__"],
    deps = [
        "//:go_default_library",
        "//xy/internal/robustdeterminate:go_default_library",
        "//xy/location:go_default_library",
    ],
)

go_test(
    name = "go_default_xtest",
    srcs = ["ray_crossing_test.go"],
    deps = [
        ":go_default_library",
        "//:go_default_library",
        "//xy/location:go_default_library",
    ],
)
