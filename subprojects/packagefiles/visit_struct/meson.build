# SPDX-FileCopyrightText: 2026 Neptuwunium
#
# SPDX-License-Identifier: EUPL-1.2

project(
	'visit_struct',
	'cpp',
	version : '1.2.0',
	meson_version : '>= 1.7.0',
	default_options : ['warning_level=3', 'cpp_std=c++17'],
)

visit_struct_include = include_directories('include')

visit_struct_dep = declare_dependency(
    include_directories: visit_struct_include,
)

install_subdir('include/visit_struct', install_dir: get_option('includedir'))
pkg = import('pkgconfig')
pkg.generate(
  name: 'visit_struct',
  description: 'A miniature library for struct-field reflection in C++',
  url: 'https://github.com/cbeck88/visit_struct',
)
