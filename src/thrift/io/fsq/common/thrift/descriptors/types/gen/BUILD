
scala_record_library(
  name = 'gen',
  sources = globs('*.thrift'),
  dependencies = [
    'src/jvm/io/fsq/spindle/runtime',
    'src/thrift/io/fsq/common/thrift/descriptors/headers/gen',
  ],
  tags = [
    'fscommon',
    'opensource',
    'dependencies_must_have:fscommon',
    'dependencies_must_have:opensource',
  ],
)

# Required to bring the thrift files into an integration test's chroot.
files(
  name = 'files',
  sources = globs('*thrift'),
  scope="runtime",
)
