load('//:buckaroo_macros.bzl', 'buckaroo_deps')
load('//:subdir_glob.bzl', 'subdir_glob')

cxx_library(
  name = 'flatbuffers',
  header_namespace = '',
  exported_headers = subdir_glob([
    ('include', '**/*.h'),
  ]),
  headers = subdir_glob([
    ('grpc', 'src/**/*.h'),
  ]),
  srcs = glob([
    'src/**/*.cpp',
  ]),
  licenses = [
    'LICENSE.txt',
  ],
  deps = buckaroo_deps(),
  visibility = [
    'PUBLIC',
  ],
)
