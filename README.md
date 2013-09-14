# Custom Cygwin ports
## Build ports
  1. Install cygport package.
  2. Get [custom_ports](https://github.com/6RUN0/custom_cygports/archive/master.zip).
  3. Run ``$ cygport [package-name]-[version]-[release].cygport download``.
  4. Run ``$ cygport [package-name]-[version]-[release].cygport prep``.
  5. Run ``$ cygport [package-name]-[version]-[release].cygport all``.
  6. Copy ``[package-name]-[version]-[relese]/dist/[package-name]`` to ``[custom-mirror]/(x86|x86_64)/[any-name]``.
  7. Change the working directory to ``[custom-mirror]/(x86|x86_64)``.
  8. Get [genini](http://cygwin.com/cgi-bin/cvsweb.cgi/genini/genini?cvsroot=cygwin-apps).
  9. Run ``$ ./genini ./[any-name]/* | bzip2 > setup.bz2``
  10. Run ``$ ./genini ./[any-name]/* > setup.ini``
