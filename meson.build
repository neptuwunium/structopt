# SPDX-FileCopyrightText: 2026 Neptuwunium
#
# SPDX-License-Identifier: EUPL-1.2

project(
	'structopt',
	'cpp',
	version : '0.1.3',
	meson_version : '>= 1.7.0',
	default_options : ['warning_level=3', 'cpp_std=c++17'],
)

magic_enum_dep = dependency('magic_enum')
visit_struct_dep = dependency('visit_struct')

structopt_include = include_directories('include')

structopt_dep = declare_dependency(
    include_directories: structopt_include,
	dependencies: [magic_enum_dep, visit_struct_dep],
)

if not meson.is_subproject()
	subdir('samples')
	subdir('tests')
endif

install_subdir('include/structopt', install_dir: get_option('includedir'))
pkg = import('pkgconfig')
pkg.generate(
  name: 'structopt',
  description: 'Parse command line arguments by defining a struct',
  url: 'https://github.com/p-ranav/structopt',
)
