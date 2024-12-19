project('c', 'c',
  version : '0.1.0',
  default_options : ['warning_level=3'])

inc = include_directories('include')

lib = static_library('c',
  'src/c.c',
  include_directories : inc,
  install : true)

install_headers('include/c/c.h',
  subdir : 'c')

pkg = import('pkgconfig')
pkg.generate(lib,
  name : 'c',
  description : 'C library',
  version : '0.1.0')
