load("//tools/bzl:junit.bzl", "junit_tests")

junit_tests(
    name = "server_tests",
    srcs = [
        "AutoValueTest.java",
        "VersionTest.java",
    ],
    tags = ["no_windows"],
    deps = [
        "//java/com/google/gerrit/common:server",
        "//java/com/google/gerrit/common:version",
        "//java/com/google/gerrit/launcher",
        "//java/com/google/gerrit/reviewdb:server",
        "//lib:guava",
        "//lib/auto:auto-value",
        "//lib/auto:auto-value-annotations",
        "//lib/truth",
    ],
)
