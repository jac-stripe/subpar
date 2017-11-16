package(default_visibility = ["//compiler:__pkg__"])

py_library(
    name = "support",
    srcs = [
        "__init__.py",
        "support.py",
        "//:__init__.py",
    ],
    srcs_version = "PY2AND3",
)

load("@runtime_test_deps//:requirements.bzl", "requirement")

py_test(
    name = "support_test",
    size = "small",
    srcs = ["support_test.py"],
    main = "support_test.py",
    srcs_version = "PY2AND3",
    deps = [
        ":support",
        requirement("mock"),
        requirement("funcsigs"),
        requirement("pbr"),
        requirement("six"),
    ],
)
