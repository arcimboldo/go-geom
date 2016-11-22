load("@io_bazel_rules_go//go:def.bzl", "go_library", "go_test")

go_library(
    name = "go_default_library",
    srcs = [
        "sql.go",
        "wkb.go",
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
        "sql_test.go",
        "wkb_test.go",
    ],
    library = ":go_default_library",
    deps = [
        "//:go_default_library",
        "//encoding/wkbcommon:go_default_library",
        "//internal/testdata:go_default_library",
        "@in_gopkg_DATA_DOG_go_sqlmock_v1//:go_default_library",
    ],
)
