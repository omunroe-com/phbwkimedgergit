load("//tools/bzl:junit.bzl", "junit_tests")

MEDIUM_TESTS = ["RefUpdateUtilRepoTest.java"]

junit_tests(
    name = "medium_tests",
    size = "medium",
    timeout = "short",
    srcs = MEDIUM_TESTS,
    tags = ["no_windows"],
    deps = [
        "//java/com/google/gerrit/git",
        "//lib:guava",
        "//lib:junit",
        "//lib/jgit/org.eclipse.jgit:jgit",
        "//lib/jgit/org.eclipse.jgit.junit:junit",
        "//lib/truth",
    ],
)

junit_tests(
    name = "small_tests",
    size = "small",
    srcs = glob(
        ["*.java"],
        exclude = MEDIUM_TESTS,
    ),
    deps = [
        "//java/com/google/gerrit/git",
        "//lib:guava",
        "//lib/jgit/org.eclipse.jgit:jgit",
        "//lib/truth",
    ],
)
