java_library(
    sources = rglobs("*.java"),
    provides = artifact(
        org = "com.twitter",
        name = "finagle-thrift-java",
        repo = artifactory,
    ),
    dependencies = [
        "3rdparty/jvm/org/apache/thrift:libthrift",
    ],
)

# For usecases (like scrooge codegen) where this dependency is used, but not detected as
# used by zinc.
target(
    name = "forced",
    scope = "forced",
    dependencies = [":java"],
)
