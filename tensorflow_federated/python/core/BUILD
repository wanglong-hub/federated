package_group(
    name = "core_visibility",
    packages = [
        "//tensorflow_federated/python/learning/...",
        "//tensorflow_federated/python/simulation/...",
    ],
)

package(default_visibility = ["//visibility:private"])

licenses(["notice"])

py_library(
    name = "core",
    srcs = ["__init__.py"],
    srcs_version = "PY3",
    visibility = [
        "//tensorflow_federated:__pkg__",
        "//tensorflow_federated/tools:__subpackages__",

        # TODO(b/143772942): This visibility is temporary and can be removed
        # once the `learning` and `simulation` packages depend on targets
        # explicitly.
        "//tensorflow_federated:__subpackages__",
    ],
    deps = [
        "//tensorflow_federated/python/core/api:computation_base",
        "//tensorflow_federated/python/core/api:computation_types",
        "//tensorflow_federated/python/core/api:computations",
        "//tensorflow_federated/python/core/api:intrinsics",
        "//tensorflow_federated/python/core/api:placements",
        "//tensorflow_federated/python/core/api:typed_object",
        "//tensorflow_federated/python/core/api:value_base",
        "//tensorflow_federated/python/core/api:values",
        "//tensorflow_federated/python/core/backends",
        "//tensorflow_federated/python/core/framework",
        "//tensorflow_federated/python/core/impl/executors:default_executor",
        "//tensorflow_federated/python/core/templates",
        "//tensorflow_federated/python/core/test",
        "//tensorflow_federated/python/core/utils",
    ],
)
