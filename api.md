For information about the libosinfo C library API, it is recommended to
consult the documentation that ships with the library installation on your
development machine. On a Fedora / RHEL distro, this will typically be found
in the following directory (once the ``libosinfo-devel`` RPM is installed):

```
  /usr/share/gtk-doc/html/Libosinfo/index.html
```

This is directly viewable in a web browser, but if running the GNOME desktop,
can also be accessed by launching the ``devhelp`` program from your shell /
desktop and selecting the ``Libosinfo`` library.

For those wishing to access the ``Libosinfo`` API from Python, there are some
online docs that are generated from the GObject Introspection metadata:

* [http://lazka.github.io/pgi-docs/#Libosinfo-1.0](http://lazka.github.io/pgi-docs/#Libosinfo-1.0)

Finally, the raw introspection data and or C headers files can also be browsed
to see what APIs are exposed from the C library

```
  /usr/share/gir-1.0/Libosinfo-1.0.gir
  /usr/include/libosinfo-1.0/
```