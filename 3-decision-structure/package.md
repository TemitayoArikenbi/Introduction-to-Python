# Write your modules
firstpackage.py
Create a package folder. You can call it example_pkg

## firstpackage.py

def add_one(number):
    print("Our package adds 100 to the number we specify"),
    return number + 100

## Init and Setup Files
Create a blank __init__.py file, which will be used by Python to recognize this as a package.
$ touch __init__.py
At this point, our file structure should look like this:
dir/
    example_pkg/
              firstpackage.py
              __init__.py

Next, create a setup.py file outside of your package directory

## setup.py

import setuptools
setuptools.setup(name='example_pkg',
version='0.1',
description='An example package',
url='#',
author='tayo arikenbi',
install_requires=['opencv-python'],
author_email='tayo.arikenbi@csulb.edu',
packages=setuptools.find_packages(),
zip_safe=False)

Note that packages not included in the python standard library should be included in install_requires. Our file structure should now look like:

dir/
    example_pkg/
              firstpackage.py
              __init__.py
    setup.py

## Build and install your package

If you are using virtual environments (generally good practice for Python development), create and activate your environment.
$ python3 -m venv myenv
$ source myenv/bin/activate
Install wheel.
$ pip install wheel
Install the package into your environment.
$ pip install .
Our package has been created, and we can now use it from anywhere. Let’s create a simple app which incorporates our package contents.

sample_prg.py

## sample_prg.py

from example_pkg.firstpackage import add_one
add_one(270)


We have now built and implemented a basic python package! More information regarding package distribution, licensing, and installation can be found in the documentation.
