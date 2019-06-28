# Getting started

Download [MicroPython](https://micropython.org/download#esp32) for ESP32.  
For full documentation visit [mkdocs.org](https://mkdocs.org).

## Commands

* `mkdocs new [dir-name]` - Create a new project.
* `mkdocs serve` - Start the live-reloading docs server.
* `mkdocs build` - Build the documentation site.
* `mkdocs help` - Print this help message.

<div class="admonition warning">
<p class="admonition-title">Do try this at home</p>
<p>...</p>
</div>

    
## Project layout

    ls /dev/tty*

This will list your ESP32 e.g. > `ttyUSB0`
 
    pip install esptool
    
blabla > rshell '
``` Bash
esptool.py --chip esp32 --port /dev/ttyUSB0 erase_flash
```
blabla > rshell '
``` Bash
pip3 install rshell
```

this will give

    esptool.py v2.6
    Serial port /dev/ttyUSB0
    Connecting........_____....._____....._____....._____.
    Chip is ESP32D0WDQ6 (revision 1)
    Features: WiFi, BT, Dual Core, 240MHz, VRef calibration in efuse, Coding Scheme None
    MAC: 3c:71:bf:47:ba:d0
    Uploading stub...
    Running stub...
    Stub running...
    Erasing flash (this may take a while)...
    Chip erase completed successfully in 9.2s
    Hard resetting via RTS pin...

whaaa

``` Bash
screen -port /dev/ttyUSB0 115200
```

whaaa

``` Bash
rshell -p /dev/ttyUSB0
```


whaaa

``` Bash
ls /pyboard/
```

whadafuck

```Bash tab=
#!/bin/bash
STR="Hello World!"
echo $STR
```

```C tab=
#include 

int main(void) {
  printf("hello, world\n");
}
```

```C++ tab=
#include <iostream>

int main() {
  std::cout << "Hello, world!\n";
  return 0;
}
```

```C# tab=
using System;

class Program {
  static void Main(string[] args) {
    Console.WriteLine("Hello, world!");
  }
}
```

``` python tab=
""" Bubble sort """
def bubble_sort(items):
    for i in range(len(items)):
        for j in range(len(items) - 1 - i):
            if items[j] > items[j + 1]:
                items[j], items[j + 1] = items[j + 1], items[j]
```



<iframe width="560" height="315" src="https://www.youtube.com/embed/5W3WvXAmDJc" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
