# msys2libs
Visual Studio needs these `.lib` files to link against MSYS2 `.dll`'s

`gendef /c/msys64/mingw64/bin/*.dll`

That generates lots of `*.def` files

Then convert these `.def` files to `.lib` files:

```
lib /MACHINE:X64 /DEF:libasprintf-0.def                      /OUT:libasprintf-0.lib
lib /MACHINE:X64 /DEF:libatk-1.0-0.def                       /OUT:libatk-1.0-0.lib
lib /MACHINE:X64 /DEF:libatomic-1.def                        /OUT:libatomic-1.lib
lib /MACHINE:X64 /DEF:libbz2-1.def                           /OUT:libbz2-1.lib
lib /MACHINE:X64 /DEF:libcairo-2.def                         /OUT:libcairo-2.lib
lib /MACHINE:X64 /DEF:libcairo-gobject-2.def                 /OUT:libcairo-gobject-2.lib
lib /MACHINE:X64 /DEF:libcairo-script-interpreter-2.def      /OUT:libcairo-script-interpreter-2.lib
lib /MACHINE:X64 /DEF:libcharset-1.def                       /OUT:libcharset-1.lib
lib /MACHINE:X64 /DEF:libcroco-0.6-3.def                     /OUT:libcroco-0.6-3.lib
lib /MACHINE:X64 /DEF:libexpat-1.def                         /OUT:libexpat-1.lib
lib /MACHINE:X64 /DEF:libffi-6.def                           /OUT:libffi-6.lib
lib /MACHINE:X64 /DEF:libfontconfig-1.def                    /OUT:libfontconfig-1.lib
lib /MACHINE:X64 /DEF:libfreetype-6.def                      /OUT:libfreetype-6.lib
lib /MACHINE:X64 /DEF:libgailutil-18.def                     /OUT:libgailutil-18.lib
lib /MACHINE:X64 /DEF:libgcc_s_seh-1.def                     /OUT:libgcc_s_seh-1.lib
lib /MACHINE:X64 /DEF:libgdk_pixbuf-2.0-0.def                /OUT:libgdk_pixbuf-2.0-0.lib
lib /MACHINE:X64 /DEF:libgdkglext-win32-1.0-0.def            /OUT:libgdkglext-win32-1.0-0.lib
lib /MACHINE:X64 /DEF:libgdk-win32-2.0-0.def                 /OUT:libgdk-win32-2.0-0.lib
lib /MACHINE:X64 /DEF:libgettextlib-0-19-7.def               /OUT:libgettextlib-0-19-7.lib
lib /MACHINE:X64 /DEF:libgettextpo-0.def                     /OUT:libgettextpo-0.lib
lib /MACHINE:X64 /DEF:libgettextsrc-0-19-7.def               /OUT:libgettextsrc-0-19-7.lib
lib /MACHINE:X64 /DEF:libgfortran-3.def                      /OUT:libgfortran-3.lib
lib /MACHINE:X64 /DEF:libgio-2.0-0.def                       /OUT:libgio-2.0-0.lib
lib /MACHINE:X64 /DEF:libglib-2.0-0.def                      /OUT:libglib-2.0-0.lib
lib /MACHINE:X64 /DEF:libgmodule-2.0-0.def                   /OUT:libgmodule-2.0-0.lib
lib /MACHINE:X64 /DEF:libgmp-10.def                          /OUT:libgmp-10.lib
lib /MACHINE:X64 /DEF:libgmpxx-4.def                         /OUT:libgmpxx-4.lib
lib /MACHINE:X64 /DEF:libgobject-2.0-0.def                   /OUT:libgobject-2.0-0.lib
lib /MACHINE:X64 /DEF:libgomp-1.def                          /OUT:libgomp-1.lib
lib /MACHINE:X64 /DEF:libgraphite2.def                       /OUT:libgraphite2.lib
lib /MACHINE:X64 /DEF:libgthread-2.0-0.def                   /OUT:libgthread-2.0-0.lib
lib /MACHINE:X64 /DEF:libgtkglext-win32-1.0-0.def            /OUT:libgtkglext-win32-1.0-0.lib
lib /MACHINE:X64 /DEF:libgtk-win32-2.0-0.def                 /OUT:libgtk-win32-2.0-0.lib
lib /MACHINE:X64 /DEF:libharfbuzz-0.def                      /OUT:libharfbuzz-0.lib
lib /MACHINE:X64 /DEF:libharfbuzz-gobject-0.def              /OUT:libharfbuzz-gobject-0.lib
lib /MACHINE:X64 /DEF:libharfbuzz-icu-0.def                  /OUT:libharfbuzz-icu-0.lib
lib /MACHINE:X64 /DEF:libiconv-2.def                         /OUT:libiconv-2.lib
lib /MACHINE:X64 /DEF:libintl-8.def                          /OUT:libintl-8.lib
lib /MACHINE:X64 /DEF:libjasper-1.def                        /OUT:libjasper-1.lib
lib /MACHINE:X64 /DEF:libjpeg-8.def                          /OUT:libjpeg-8.lib
lib /MACHINE:X64 /DEF:liblzma-5.def                          /OUT:liblzma-5.lib
lib /MACHINE:X64 /DEF:liblzo2-2.def                          /OUT:liblzo2-2.lib
lib /MACHINE:X64 /DEF:libminizip-1.def                       /OUT:libminizip-1.lib
lib /MACHINE:X64 /DEF:libpango-1.0-0.def                     /OUT:libpango-1.0-0.lib
lib /MACHINE:X64 /DEF:libpangocairo-1.0-0.def                /OUT:libpangocairo-1.0-0.lib
lib /MACHINE:X64 /DEF:libpangoft2-1.0-0.def                  /OUT:libpangoft2-1.0-0.lib
lib /MACHINE:X64 /DEF:libpangowin32-1.0-0.def                /OUT:libpangowin32-1.0-0.lib
lib /MACHINE:X64 /DEF:libpcre-1.def                          /OUT:libpcre-1.lib
lib /MACHINE:X64 /DEF:libpcre16-0.def                        /OUT:libpcre16-0.lib
lib /MACHINE:X64 /DEF:libpcre32-0.def                        /OUT:libpcre32-0.lib
lib /MACHINE:X64 /DEF:libpcrecpp-0.def                       /OUT:libpcrecpp-0.lib
lib /MACHINE:X64 /DEF:libpcreposix-0.def                     /OUT:libpcreposix-0.lib
lib /MACHINE:X64 /DEF:libpixman-1-0.def                      /OUT:libpixman-1-0.lib
lib /MACHINE:X64 /DEF:libpng16-16.def                        /OUT:libpng16-16.lib
lib /MACHINE:X64 /DEF:libquadmath-0.def                      /OUT:libquadmath-0.lib
lib /MACHINE:X64 /DEF:librsvg-2-2.def                        /OUT:librsvg-2-2.lib
lib /MACHINE:X64 /DEF:libssp-0.def                           /OUT:libssp-0.lib
lib /MACHINE:X64 /DEF:libstdc++-6.def                        /OUT:libstdc++-6.lib
lib /MACHINE:X64 /DEF:libtiff-5.def                          /OUT:libtiff-5.lib
lib /MACHINE:X64 /DEF:libtiffxx-5.def                        /OUT:libtiffxx-5.lib
lib /MACHINE:X64 /DEF:libturbojpeg-0.def                     /OUT:libturbojpeg-0.lib
lib /MACHINE:X64 /DEF:libwinpthread-1.def                    /OUT:libwinpthread-1.lib
lib /MACHINE:X64 /DEF:libxml2-2.def                          /OUT:libxml2-2.lib
lib /MACHINE:X64 /DEF:zlib1.def                              /OUT:libb1.lib
```

Run that `.bat` with this shell:

`C:\Program Files (x86)\Microsoft Visual Studio\2017\Community\VC\Auxiliary\Build\vcvarsall.bat`
