# Experiments in Repeater Controller Design (Part 1)

**Posted on November 20, 2016**

Back in the mid 1980’s, my ham radio activity was almost exclusively via 2 Meter repeaters. It was all my budget could allow especially given my (ahem) social priorities. I knew the owners of a few of the repeaters enjoying runs to small buildings on mountain tops as they tweaked/tuned/upgraded the equipment. Most notable were the first install of WB2BQW/R on [Schunemunk Mountain](https://en.wikipedia.org/wiki/Schunemunk_Mountain), midnight runs to the highest repeater in New Jersey, [KA2DEW/R](http://www.torborg.com/ka2dew/catfish.htm), and when N2ETY/R was first put on the air from the Circleville Fire Department site.

Though I lost interest in talking on repeaters, I did not lose interest in repeater technology itself. The repeater controllers that ran KA2DEW/R and N2ETY/R intrigued me with their use of homebrew and commercially available technology respectively. The [KA2DEW/R homebrew Z80 microprocessor-based controller](http://www.torborg.com/ka2dew/catfish.htm) was one of the first of it’s kind back in 1982. The commercial controller that ran on N2ETY/R was an ACC RC-850. Since I was invited as a control operator of the repeater, I was given a copy of the [reference manual](http://www.repeater-builder.com/acc/pdfs/acc-rc-85-manual.pdf).

Pouring through that manual helped me reverse engineer what constructs and flow would be required if I wanted to write my own repeater controller software. But since I had little success in building hardware to date I just satisfied myself with paper exercises of what that software would like like among various languages and platforms. A functional prototype and all the hardware would be a dream. Given my impatience, prototyping with [PIC microcontrollers](https://en.wikipedia.org/wiki/PIC_microcontroller) was considered too adventurous for me in the 80s.

In the 90s the inspiration returned when Parallax released the [BASIC Stamp Microcontroller](https://www.parallax.com/microcontrollers/basic-stamp). Prototyping the software would be easier since I could rapidly iterate and test versions of software without having to have multiple PIC with EPROMS to erase. The I/O pins were durable for simple LED and push-button test circuits on a breadboard to simulate radio connections. The [first HAM STAMP Program](/assets/RIC-Linx_STAMP.doc) I wrote for the STAMP was in 1995. The controller I wrote was simple; detect carrier and PL (simulated with push buttons), key the radio (light an LED), and counters for repeater tail and timeout. I never got the chance to see if it worked in the real world so to the shelf it went. It would be almost 20 years until the subject of repeater controllers would capture my interest again.

The inspiration returned again in 2012 when helping my local amateur radio club get it’s own repeater on the air. I started with the BASIC stamp code I produced to refresh my memory programming with a STAMP and then looked around on the Internet to see if there is existing code I could use or be inspired by. I found that with some work done by [M0ZPT](http://www.m0pzt.com/projects/) and produced a second more comprehensive version of my [repeater controller program for the STAMP](/assets/NE2Z_Repeater_Controller_v-09.bs2_.txt). I then decided to [port my code to the Arduino](/assets/NE2Z_Repeater_Controller_Arduino_v6.ino_.txt). Unfortunately neither prototype left the bench to be tested in the real world and again my interest waned.

The next dose of inspiration came in late 2014 when thinking of Ham Radio ideas for the [HOPE XI conference](https://xi.hope.net/) suggesting we setup a temporary repeater, as mentioned in [my previous blog post](/assets/hope-xi-repeater/index.md). Though I shelved the prototype for the conference, I continued to build the prototype running [SVXlink](http://www.svxlink.org/) on a [Raspberry Pi 2](https://www.raspberrypi.org/products/raspberry-pi-2-model-b/) into a functioning repeater.

I will discuss that work in detail in an upcoming post.

For what it’s worth,

- Joe, NE2Z
