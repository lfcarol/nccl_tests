# Note
copy from nvidia/nccl_tests repo for testing "bazel build"
引用 nvidia/nccl_tests (git@github.com:NVIDIA/nccl-tests.git) 作为测试demo

# Usage
    1.clone apollo代码 ```git clone -b master git@github.com:lfcarol/apollo.git```
    2.在apollo目录下下载demo源码 ```git clone git@github.com:lfcarol/nccl_tests.git```
    3.执行```bstart```指令，启动apollo_dev镜像
    4.执行```binto```指令，进入apollo_dev镜像
    5.执行bazel编译，```bazel build --config=gpu /apollo/nccl_tests/src/...```
    6.测试```/apollo/bazel-bin/nccl_tests/src/XXXX```可执行文件
