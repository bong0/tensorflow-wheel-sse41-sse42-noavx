# tensorflow-wheel-sse41-sse42-noavx 

This is a wheel for tensorflow built with
  * Python 3.5.2
  * Tensorflow 1.1.0
  * Linux X86_64 (Debian Jessie)
  * SSE4.1
  * SSE4.2
  * **NO** AVX

It's compatible to my 2012 Xeon X5-2620v2 Dualsocket machine.

Build command: `bazel build -c opt --copt=-msse4.2 --copt=-msse4.1 -k //tensorflow/tools/pip_package:build_pip_package`


# tensorflow-wheel-sse41-sse42-avx

with avx: `bazel build -c opt --copt=-mavx --copt=-msse4.
2 --copt=-msse4.1 -k //tensorflow/tools/pip_package:build_pip_package`

