load("@io_bazel_rules_go//go:def.bzl", "go_library", "go_test")

go_library(
    name = "go_default_library",
    srcs = ["geojson.go"],
    visibility = ["//visibility:public"],
    deps = ["//:go_default_library"],
)

go_test(
    name = "go_default_test",
    srcs = ["geojson_test.go"],
    library = ":go_default_library",
    deps = [
        "//:go_default_library",
        "@com_github_d4l3k_messagediff//:go_default_library",
    ],
)
