package(default_visibility = [
    "//tensorflow_model_optimization:__subpackages__",
])

licenses(["notice"])  # Apache 2.0

py_library(
    name = "transforms",
    srcs = [
        "transforms.py",
    ],
    srcs_version = "PY2AND3",
    visibility = ["//visibility:public"],
    deps = [
        # six dep1,
    ],
)

py_test(
    name = "transforms_test",
    srcs = [
        "transforms_test.py",
    ],
    python_version = "PY3",
    srcs_version = "PY2AND3",
    visibility = ["//visibility:public"],
    deps = [
        ":transforms",
        # tensorflow dep1,
    ],
)

py_library(
    name = "model_transformer",
    srcs = [
        "model_transformer.py",
    ],
    srcs_version = "PY2AND3",
    visibility = ["//visibility:public"],
    deps = [
        ":transforms",
        # six dep1,
        # tensorflow dep1,
        # python/keras tensorflow dep2,
    ],
)

py_test(
    name = "model_transformer_test",
    srcs = [
        "model_transformer_test.py",
    ],
    python_version = "PY3",
    srcs_version = "PY2AND3",
    visibility = ["//visibility:public"],
    deps = [
        ":model_transformer",
        # tensorflow dep1,
        # python/keras tensorflow dep2,
    ],
)
