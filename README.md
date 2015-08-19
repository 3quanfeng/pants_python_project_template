# Create Pants env, python 2.7.6
$ pip install virtualenv
$ virtualenv PANTS
$ source ./PANTS/bin/activate
$ pip install pantsbuild.pants


## Run
$ git clone https://github.com/3quanfeng/pants_python_project_template.git
$ cd pants_python_project_template
$ pants -V
$ pants -q run src/python/myproject:myapp

## Build
$ pants binary src/python/myproject:myapp

