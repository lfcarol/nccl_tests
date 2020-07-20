load("@rules_cc//cc:defs.bzl", "cc_library")
load("@rules_cc//cc:defs.bzl", "cc_binary")
load("@local_config_cuda//cuda:build_defs.bzl", "cuda_binary")
load("@local_config_cuda//cuda:build_defs.bzl", "cuda_library")
load("@local_config_cuda//cuda:build_defs.bzl", "cuda_header_library")
package(default_visibility = ["//visibility:public"])

cuda_binary(
  name = "all_gather",
  srcs = [
    "all_gather.cu",
  ],
  deps = [
    "@local_config_cuda//cuda:nccl",
    ":test_common",
  ],
  linkopts = [
    "-lpthread",
  ],
)

cuda_binary(
  name = "all_reduce",
  srcs = [
    "all_reduce.cu",
  ],
  deps = [
    "@local_config_cuda//cuda:nccl",
    ":test_common",
  ],
  linkopts = [
    "-lpthread",
  ],
)

cuda_binary(
  name = "alltoall",
  srcs = [
    "alltoall.cu",
  ],
  deps = [
    "@local_config_cuda//cuda:nccl",
    ":test_common",
  ],
  linkopts = [
    "-lpthread",
  ],
)

cuda_binary(
  name = "broadcast",
  srcs = [
    "broadcast.cu",
  ],
  deps = [
    "@local_config_cuda//cuda:nccl",
    ":test_common",
  ],
  linkopts = [
    "-lpthread",
  ],
)

cuda_binary(
  name = "reduce_scatter",
  srcs = [
    "reduce_scatter.cu",
  ],
  deps = [
    "@local_config_cuda//cuda:nccl",
    ":test_common",
  ],
  linkopts = [
    "-lpthread",
  ],
)

cuda_binary(
  name = "reduce",
  srcs = [
    "reduce.cu",
  ],
  deps = [
    "@local_config_cuda//cuda:nccl",
    ":test_common",
  ],
  linkopts = [
    "-lpthread",
  ],
)


cuda_library(
  name = "test_common",
  srcs = [
    "common.cu"
  ],
  hdrs = [
    "common.h",
    "nccl1_compat.h",
  ]
)








