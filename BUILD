load("@rules_cc//cc:defs.bzl", "cc_test", "cc_library")

cc_library(
    name = "hello-greet",
    srcs = ["hello-greet.cc"],
    hdrs = ["hello-greet.h"],
)

cc_test(
    name = "hello-world",
    srcs = ["hello-world.cc"],
    deps = [
        ":hello-greet",
    ],
    size = "small",
)

test_suite(
    name = "hello-world-test-suite",
    tests = [":hello-world"],
)