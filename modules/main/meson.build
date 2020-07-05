exe_lib = library('prog-lib', files('project.c'),
    include_directories: include_directories('.'))

exe_dep = declare_dependency(
    version: meson.project_version(),
    link_with: exe_lib,
    include_directories: include_directories('.'))




executable('prog', files('main.c'), dependencies: [exe_dep])