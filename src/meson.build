xmppdbg_sources = [
  'main.c',
  'xmppdbg-window.c',
  'xmppdbg-application.c',
]

xmppdbg_deps = [
  dependency('libadwaita-1', version: '>= 1.0'),
]

gnome = import('gnome')

xmppdbg_sources += gnome.compile_resources('xmppdbg-resources',
  'xmppdbg.gresource.xml',
  c_name: 'xmppdbg'
)

executable('xmppdbg', xmppdbg_sources,
  dependencies: xmppdbg_deps,
  install: true,
)
