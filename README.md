For the XP11 version a linkable OpenAL32.dll was obtained as follows:
- get copy of libOpenAL32.dll e.g. from XP11's dll folder
- pick libOpenAL's *include/AL* header files, e.g. from the msys2 system
- run within a msys2 shell:
```
gendef OpenAL32.dll
dlltool -d OpenAL32.def -D OpenAL32.dll -k -a -l libopenal32.a -v
```
