# embeddedWoT HTTP Binding
HTTP and LongPoll binding library for embeddedWoTServient project.
This library is a part of [WoT Microcontroller Servient](https://github.com/Chello/WoT-microcontroller-servient-GUI) project. 

This library manages the binding for HTTP protocol, in order to respond to HTTP requests to Interaction Affordances for WoT Protocol in embedded boards

For including it in the Arduino library path use these commands:

```shell
cd ~/Arduino/libraries
git clone https://github.com/Chello/embeddedWoT_HTTP_LongPoll.git
```

For including the library in the Arduino project:

```c
#include <embeddedWoT_HTTP_LongPoll.h>
```

An example of usage:

```c
embeddedWoT_HTTP_LongPoll *hlp = new embeddedWoT_HTTP_LongPoll
//expose an array of actions
hlp->exposeActions(<<String[N] of endpoinst>>, <<callback[N]>>, N);
hlp->begin();
```

The library has several functions. These are documented in the .h header file.