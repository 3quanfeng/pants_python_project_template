python_library(name="app-lib",
               sources=globs("*.py"),
              )



python_binary(name="myapp",
              source="hello_world.py",
              dependencies=[':app-lib',
                            'src/python/test:sumapp',
                            '3rdparty/python:requests',
                           ]
              )
