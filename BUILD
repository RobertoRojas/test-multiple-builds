cc_library(
    name = "f1",
    srcs = ["f1/src/f1.c"],
    hdrs = ["f1/hdr"],
    includes = ["f1/hdr"],
)

cc_library(
    name = "f2",
    srcs = ["f2/src/f2.c"],
    hdrs = ["f2/hdr"],
    includes = ["f2/hdr"],
)

"""
cc_library(
    name = "f1_prebuild",
    srcs = ["test/f1.pic.o"],
    hdrs = ["f1/hdr"],
    includes = ["f1/hdr"],
)
"""

cc_binary(
    name = "program",
    srcs = ["main/src/main.c"],
    deps = [
        ":f1",
        ":f2"
    ],
)