This project shows basically the template of using pants with your python project 

## Create Pants env, python 2.7.6
```bash
$ pip install virtualenv
$ virtualenv PANTS
$ source ./PANTS/bin/activate
$ pip install pantsbuild.pants
```

## Run
```bash
$ git clone https://github.com/3quanfeng/pants_python_project_template.git
$ cd pants_python_project_template
$ pants -V
$ pants -q run src/python/myproject:myapp
```
## Build pex
```bash
$ pants binary src/python/myproject:myapp
```

## Test
```
PANTS_VERBOSE=1 pants test test/python/:testsum
```

## Interactive python REPL session
```
PANTS_VERBOSE=1 pants repl run src/python/myproject:myapp
>>> import sum2
>>> sum2.sum(2,2)
4
```
