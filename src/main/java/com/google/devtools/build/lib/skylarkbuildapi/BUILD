# Description:
#   This package contains interfaces representing the skylark "build API"
#   (but not the implementation of that API). Ultimately, this package
#   may be broken out of the Bazel package hierarchy to be standalone.
#   Thus, this package should not depend on Bazel-specific packages (only
#   those which contain pure-Skylark concepts, such as the interpretter or
#   annotation interfaces).

package(default_visibility = ["//src/main/java/com/google/devtools/build/lib:__pkg__"])

licenses(["notice"])  # Apache 2.0

filegroup(
    name = "srcs",
    srcs = glob(["**"]),
)

java_library(
    name = "skylarkbuildapi",
    srcs = glob(["*.java"]),
    deps = [
        "//src/main/java/com/google/devtools/build/lib:events",
        "//src/main/java/com/google/devtools/build/lib:skylarkinterface",
        "//src/main/java/com/google/devtools/build/lib:syntax",
        "//third_party:guava",
        "//third_party:jsr305",
    ],
)
