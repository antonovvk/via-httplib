cc_library(
    name = "viahttplib",
    srcs = glob(
        ["src/via/**/*.cpp"],
    ),
    hdrs = glob([
        "include/via/**/*.hpp",
    ]),
    includes = [
        "include",
    ],
    copts = [
        "-std=c++11",
        "-Wall",
    ],
    visibility = ["//visibility:public"],
)

cc_test(
    name = "tests",
    srcs = glob([
        "tests/**/*.cpp",
        "tests/test_main.cpp"
    ]),
    deps = [
        ":viahttplib",
    ],
    linkopts = [
        "-lboost_unit_test_framework",
    ]
)
