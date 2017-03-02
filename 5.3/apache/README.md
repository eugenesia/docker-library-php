# Bug

Compiling PHP is not working for PHP 5.3.

Error:

```bash
/usr/bin/ld: ext/pcre/pcrelib/.libs/pcre_compile.o: relocation R_X86_64_PC32 against symbol `php_pcre_compile2' can not be used when making a shared object; recompile with -fPIC
/usr/bin/ld: final link failed: Bad value
collect2: error: ld returned 1 exit status
make: *** [libphp5.la] Error 1
make: *** Waiting for unfinished jobs....
```

