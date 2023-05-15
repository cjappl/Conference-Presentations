![Taming real-time logging](./slides-export/001.png)

![About me](./slides-export/002.png)

<div class="absolute left-5px bottom-5px">
<SlideCurrentNo />
</div>

<br>
<br> !

![Why do we need a real-time logger?](./slides-export/003.png)

![Motivation](./slides-export/004.png)

![Version 0](./slides-export/005.png)

![Version 0: The problem with simple printf logging](./slides-export/006.png)

![Real-time safety recap](./slides-export/007.png)

![Version 1](./slides-export/008.png)

![Version 1: Logging thread with lock free queue](./slides-export/009.png)

![A lock free queue](./slides-export/010.png)

![Version 1: Logging thread with lock free queue](./slides-export/011.png)

![Version 1: Logging thread with lock free queue](./slides-export/012.png)

![Truncation and data loss](./slides-export/013.png)

Also, messages can get "caught in the queue" you crash or don't shut down properly! Leaving valuable data behind.

also mention speed

![All done??](./slides-export/014.png)

![What's wrong here?](./slides-export/015.png)

![undefined](./slides-export/016.png)

![Log thread using std library snprintf functions](./slides-export/017.png)

![A group more paranoid than audio software engineers?](./slides-export/018.png)

![Embedded systems engineers!](./slides-export/019.png)

![`stb` - single file libraries](./slides-export/020.png)

![Version 2: Using a third party vsnprintf](./slides-export/021.png)

![Is using va_args real-time safe?](./slides-export/022.png)

![Yes!](./slides-export/023.png)

![Variadic Templates as an alternative to va_args[^1]](./slides-export/024.png)

FIXME

![Version 2: Logging thread + `stb_vsnprintf`](./slides-export/025.png)

![A note on ordering](./slides-export/026.png)

![A note on ordering](./slides-export/027.png)

![A note on ordering](./slides-export/028.png)

![Version 3: An atomic "sequence number"](./slides-export/029.png)

![Logging thread + `stb_vsnprintf` + seq number](./slides-export/030.png)

![Implementation summary](./slides-export/031.png)

![`cjappl/rtlog-cpp`](./slides-export/032.png)

![What did we learn?](./slides-export/033.png)

![Special thanks](./slides-export/034.png)

![Appendix](./slides-export/035.png)

![Variadic templates and `libfmt`](./slides-export/036.png)

![CAUTION:](./slides-export/037.png)

![`rtlog-cpp`](./slides-export/038.png)

![`rtlog-cpp`](./slides-export/039.png)

