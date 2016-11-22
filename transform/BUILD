load("@io_bazel_rules_go//go:def.bzl", "go_library", "go_test")

go_library(
    name = "go_default_library",
    srcs = [
        "transform.go",
        "tree_set.go",
    ],
    visibility = ["//visibility:public"],
    deps = ["//:go_default_library"],
)

go_test(
    name = "go_default_test",
    srcs = [
        "transform_test.go",
        "tree_set_test.go",
    ],
    library = ":go_default_library",
    deps = [
        "//:go_default_library",
        "//sorting:go_default_library",
    ],
)

go_test(
    name = "go_default_xtest",
    srcs = [
        "transform_example_newuniquecoordtransform_test.go",
        "tree_set_examples_test.go",
    ],
    deps = [
        ":go_default_library",
        "//:go_default_library",
        "//sorting:go_default_library",
    ],
)
