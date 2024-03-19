# Things you have to do

The default name of the library is "franz", if you want to change
it you would do it under "name" in the toml file.

Add some code to src/franz and them install with "pip3 install -e" and
the path to the directory where you have the toml file. You should then
be able to access the code from anywhere in your computer with something
like "from franz import ..."

## Other stuff you might want

If your package depends on something (say numpy) you indicate it in the
depencencies list of the toml file. You add a dependency with the name and
the minimum version required. For example, if you just want numpy 3.6 you
need

dependencies = ["numpy>=3.6"]

pip will automatically install all the packages in the dependencies list
if needed when you install your library

And that's it :)
There's a lot of really good docs in setuptools, but this is fun so just ask me
