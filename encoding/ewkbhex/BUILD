load("@io_bazel_rules_go//go:def.bzl", "go_library", "go_test")

go_library(
    name = "go_default_library",
    srcs = ["ewkbhex.go"],
    visibility = ["//visibility:public"],
    deps = [
        "//:go_default_library",
        "//encoding/ewkb:go_default_library",
    ],
)

go_test(
    name = "go_default_test",
    srcs = ["ewkbhex_test.go"],
    library = ":go_default_library",
    deps = [
        "//:go_default_library",
        "//encoding/ewkb:go_default_library",
        "//encoding/wkbcommon:go_default_library",
    ],
)
