# Tools for handling swap construction and cashflow manipulation

# Placeholder: load py_library
# Placeholder: load py_test

package(
    default_visibility = ["//tf_quant_finance:__subpackages__"],
    licenses = ["notice"],
)

py_library(
    name = "analytics",
    srcs = ["__init__.py"],
    deps = [
        ":cashflows",
        ":forwards",
        ":swap",
    ],
)

py_library(
    name = "forwards",
    srcs = ["forwards.py"],
    deps = [
        "//tf_quant_finance/math:segment_ops",
        # numpy dep,
        # tensorflow dep,
    ],
)

py_test(
    name = "forwards_test",
    size = "small",
    srcs = ["forwards_test.py"],
    shard_count = 4,
    deps = [
        "//tf_quant_finance",
        # test util,
        # absl/testing:parameterized dep,
        # numpy dep,
        # tensorflow dep,
    ],
)

py_library(
    name = "cashflows",
    srcs = ["cashflows.py"],
    deps = [
        # numpy dep,
        # tensorflow dep,
    ],
)

py_test(
    name = "cashflows_test",
    size = "small",
    srcs = ["cashflows_test.py"],
    shard_count = 4,
    deps = [
        "//tf_quant_finance",
        # test util,
        # absl/testing:parameterized dep,
        # numpy dep,
        # tensorflow dep,
    ],
)

py_library(
    name = "swap",
    srcs = ["swap.py"],
    deps = [
        ":cashflows",
        # numpy dep,
        # tensorflow dep,
    ],
)

py_test(
    name = "swap_test",
    size = "small",
    srcs = ["swap_test.py"],
    shard_count = 4,
    deps = [
        "//tf_quant_finance",
        # test util,
        # absl/testing:parameterized dep,
        # numpy dep,
        # tensorflow dep,
    ],
)

filegroup(
    name = "docs",
    srcs = [
        "README.md",
    ],
)
