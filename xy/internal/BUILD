load("@io_bazel_rules_go//go:def.bzl", "go_library", "go_test")

go_library(
    name = "go_default_library",
    srcs = [
        "cga.go",
        "coord_stack.go",
        "numbers.go",
        "test_data.go",
    ],
    visibility = ["//visibility:public"],
    deps = ["//:go_default_library"],
)

go_test(
    name = "go_default_test",
    srcs = ["cga_test.go"],
    library = ":go_default_library",
    deps = ["//:go_default_library"],
)

go_test(
    name = "go_default_xtest",
    srcs = [
        "coord_stack_test.go",
        "numbers_test.go",
    ],
    deps = [
        ":go_default_library",
        "//:go_default_library",
    ],
)
