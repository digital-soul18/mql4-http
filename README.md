Overview
--------

This is a simple MQL4 wrapper that uses Windows native wininet.dll. It allows
you to send HTTP requests (currently supported only GET method) to a remote
destination and read the body response from MQL that was compiled in build 600
and newer (not in a strict mode).

How to use
----------

```c
#include <mql4-mysql.mqh>

int start () {

  string myIP = httpGET("http://icanhazip.com/");

  Print("My machine's IP is ", myIP);

  return(0);
}
```

Credits
-------

This library was based on following great resources:

- HTTP Wininet sample: http://codebase.mql4.com/8115

- EasyXML parser: http://www.mql5.com/code/1998

License
-------

This is free and unencumbered software released into the public domain.

Anyone is free to copy, modify, publish, use, compile, sell, or
distribute this software, either in source code form or as a compiled
binary, for any purpose, commercial or non-commercial, and by any
means.

In jurisdictions that recognize copyright laws, the author or authors
of this software dedicate any and all copyright interest in the
software to the public domain. We make this dedication for the benefit
of the public at large and to the detriment of our heirs and
successors. We intend this dedication to be an overt act of
relinquishment in perpetuity of all present and future rights to this
software under copyright law.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
IN NO EVENT SHALL THE AUTHORS BE LIABLE FOR ANY CLAIM, DAMAGES OR
OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
OTHER DEALINGS IN THE SOFTWARE.

For more information, please refer to [<http://unlicense.org/>](http://unlicense.org)
