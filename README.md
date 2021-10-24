# lib-py-pypitemplate
This is template repository with an easy set up to release packages to pypi

## Guide on how to use this repository
1. Generate an account with PYPI and make an api token
2. On your repo ON GITHUB, create 2 new environment variables
    - PYPI_USERNAME - Can be your username or "\_\_token\_\_" depending if you want to use an apikey
    - PYPI_PASSWORD - Can be your password or apikey depending if you want to use an apikey
3. Add your dependencies on requirement.txt
4. Fill out "setup.py" - I made it pretty obvious. Just look at it.
5. Change the "my_pkg_name" folder to what your project name is and add your code in that dir
6. Commit your code
7. Decide on a version number.Version numbers must be in the x.x.x format. Valid examples:
    - 1.2.1
    - 300.0.1
    - 77.38.34
8. Create a new github release. Make the tag and the name your version number. Add whatever you want for the description.
9. GitHub workflows will trigger and automatically release now. Easy mode.


## Notes
- I added "pck_unit_tests.py" file to quickly set up some unit testing
- Your README file will be used for the PYPI description
- This was primarily made to be a quick guide. If you need to do something specific and more detailed, you'll actually need to learn how to actually make python packages.