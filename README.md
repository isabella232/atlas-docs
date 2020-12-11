Documentation for the atlas project
===================================

The documentation generated by this project is hosted at https://sites.ecmwf.int/docs/atlas

The documentation is written in ReStructuredText (rst), and converted by Pelican into HTML.
The C++ API is generated via Doxygen. The generated documentation is using m.css which results
in a nice looking and responsive web site.

The documentation is licensed with the Apache 2.0 license, see LICENSE file

Requirements for building:
--------------------------

- Python version 3.6 or higher
- Doxygen version 1.8.17 or higher
- LaTeX, optional: Recommended for rendering maths

Generate and view documentation
-------------------------------

#### Step 1: Generate the website

```
make html
```

For detailed options, see `make help`

#### Step 2: View the website

```
make serve
```

Now open browser at `http://localhost:8000`. Voila.


Publishing documentation
------------------------

Following script can be used to publish the website to https://sites.ecmwf.int/docs/atlas.

```
scripts/publish.sh
```

Note, this requires special access credentials, and is only intended for official maintainers.