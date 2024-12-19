project('f', 'c',
  version : '0.1.0',
  default_options : ['warning_level=3'])

inc = include_directories('include')

lib = static_library('f',
  'src/f.c',
  include_directories : inc,
  install : true)

install_headers('include/f/f.h',
  subdir : 'f')

pkg = import('pkgconfig')
pkg.generate(lib,
  name : 'f',
  description : 'F library',
  version : '0.1.0')
