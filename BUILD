load("@com_github_grpc_grpc//bazel:python_rules.bzl",
     "py_proto_library",
     "py_grpc_library",
)

proto_library(
    name = "helloworld_proto",
    srcs = ["helloworld.proto"],
)

py_proto_library(
    name = "helloworld_py_pb2",
    deps = [":helloworld_proto"],
)

py_grpc_library(
    name = "helloworld_py_pb2_grpc",
    srcs = [":helloworld_proto"],
    deps = [":helloworld_py_pb2"],
)
