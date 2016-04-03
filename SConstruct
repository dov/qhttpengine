env = Environment(tools=['default','qt5','textfile'],
                  CPPPATH=['#', '#/src', '#/src/QHttpEngine'],
                  CPPFLAGS=['-w','-g','-std=c++1y','-fPIC'],
                  VERSION="0.1.0",  # From CMakeLists.txt
                  CPPDEFINES=['QT_NO_SIGNALS_SLOTS_KEYWORDS',
                              'QHTTPENGINE_LIBRARY']
                  )

env.SConscript(['src/SConscript',
                'examples/SConscript',
                ],
               exports='env')

