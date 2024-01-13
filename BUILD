load("@genrules//gcs:index.bzl", "gcs_deploy")

gcs_deploy(
    name = "deploy",
    bucket_name = "$BUCKET_NAME",
    deps = [":static"],
)

filegroup(
    name = "static",
    srcs = glob([
        "static/**",
    ]),
)
