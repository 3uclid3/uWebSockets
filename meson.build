project('uWebSockets', 'cpp')

uwebsockets = custom_target(
    'uWebSockets',
    command: ['make', 'install', '-B', '-C', meson.project_source_root()],
    env: ['DESTDIR=install'],
    output: 'App.h',
    build_by_default: true,
)

uwebsockets_dep = declare_dependency(
    sources: uwebsockets,
    include_directories: 'install/usr/local/include/uWebSockets',
)