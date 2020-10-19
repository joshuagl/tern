load("@tern_deps//:requirements.bzl", "requirement")
load("@rules_python//python:defs.bzl", "py_binary")

py_library(
    name = "libtern",
    srcs = [],
    deps = [
        requirement("PyYAML"),
        requirement("docker"),
        requirement("dockerfile-parse"),
        requirement("requests"),
        requirement("stevedore"),
        requirement("pbr"),
        requirement("debut"),
        requirement("regex"),
        # do we need transitive dependencies?
    ],
)

py_binary(
    name = "tern",
    srcs = ["__main__.py"],
    deps = [":libtern"],
)
