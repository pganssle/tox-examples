# Example package using the `changedir` parameter

This is an example package that uses the `changedir` parameter to run the tests against the package as it will be installed, rather than as it exists in the repository. Note that the `setup.cfg` here is deliberately misconfigured to miss `mypkg.subpkg`, so the tests *should* fail. To see that it fails correctly, make sure `tox` is installed and invoke `tox -e py`, you should see an `ImportError`.
