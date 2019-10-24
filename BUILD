load("@com_github_grpc_grpc//bazel:python_rules.bzl",
     "py_proto_library",
     "py_grpc_library",
)

proto_library(
    name = "simple_proto",
    srcs = ["simple.proto"],
)

py_proto_library(
    name = "simple_py_pb2",
    deps = [":simple_proto"],
)

py_grpc_library(
    name = "simple_py_pb2_grpc",
    srcs = [":simple_proto"],
    deps = [":simple_py_pb2"],
)
