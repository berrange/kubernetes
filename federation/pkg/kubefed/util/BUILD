package(default_visibility = ["//visibility:public"])

licenses(["notice"])

load(
    "@io_bazel_rules_go//go:def.bzl",
    "go_library",
)

go_library(
    name = "go_default_library",
    srcs = ["util.go"],
    tags = ["automanaged"],
    deps = [
        "//federation/client/clientset_generated/federation_clientset:go_default_library",
        "//pkg/api:go_default_library",
        "//pkg/client/clientset_generated/internalclientset:go_default_library",
        "//pkg/kubectl/cmd:go_default_library",
        "//pkg/kubectl/cmd/util:go_default_library",
        "//vendor:github.com/spf13/cobra",
        "//vendor:k8s.io/apimachinery/pkg/apis/meta/v1",
        "//vendor:k8s.io/client-go/tools/clientcmd",
        "//vendor:k8s.io/client-go/tools/clientcmd/api",
    ],
)

filegroup(
    name = "package-srcs",
    srcs = glob(["**"]),
    tags = ["automanaged"],
    visibility = ["//visibility:private"],
)

filegroup(
    name = "all-srcs",
    srcs = [":package-srcs"],
    tags = ["automanaged"],
)
