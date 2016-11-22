load("@io_bazel_rules_go//go:def.bzl", "go_library", "go_test")

go_library(
    name = "go_default_library",
    srcs = [
        "ewkb.go",
        "scan.go",
    ],
    visibility = ["//visibility:public"],
    deps = [
        "//:go_default_library",
        "//encoding/wkbcommon:go_default_library",
    ],
)

go_test(
    name = "go_default_test",
    srcs = [
        "ewkb_test.go",
        "scan_test.go",
    ],
    library = ":go_default_library",
    deps = [
        "//:go_default_library",
        "@in_gopkg_DATA_DOG_go_sqlmock_v1//:go_default_library",
    ],
)
