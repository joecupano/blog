# From SWL to SIGINT

**Posted on October 18, 2021**

I am old enough to remember the heyday of Short Wave Listening. While listening to broadcast stations and searching for pirate stations was popular, trying to identify strange signals was more interesting. Many would start off listening to time stations such as [WWV](https://www.nist.gov/time-distribution/radio-station-wwv) and [CHU](https://nrc.canada.ca/en/certifications-evaluations-standards/canadas-official-time/nrc-shortwave-station-broadcasts-chu) and understanding the significance of some of tones (and other data shared), and then aeronautical signals used in transatlantic flights like [SELCAL](https://en.wikipedia.org/wiki/SELCAL). Then perhaps the mysteries of numbers stations and the “Russian Woodpecker.”

With software defined radio (SDR) we can “see” activity on a range of spectrum and drill-down on signals of interest. In turn signals have increased in complexity from analog demodulation to a known schema to digital analysis of the payload itself. The bar for what a SDR application can decode continually gets raised especially with signal UHF and up.

On HVDN I posted an article on [building a SIGINT platform](https://hvdnnotebook.blogspot.com/2021/10/chasing-dragon-building-signals.html). In that journey I’ve learned to best promote more SIGINT experimentation is to not get distracted using the myriad of applications out there focused on well understood modulations and protocols.

[SDRangel](https://rgetz.github.io/sdrangel/) and [SDR++](https://github.com/AlexandreRouma/SDRPlusPlus) reflect a new breed of SDR applications that provide documented plug-in frameworks to add further detail to signal analysis. Its’ the middle ground between doing it all in [GNU Radio’s GRC companion](https://wiki.gnuradio.org/index.php/Main_Page) or getting just enough capability from the more popular SDR applications out there. Good companions to any SDR application in helping identify captured signals include [SIGIDWIKI](https://www.sigidwiki.com/wiki/Signal_Identification_Guide) and [Artemis](https://aresvalley.com/artemis/).

With interesting signals as close as the smart devices around you, I encourage you to explore with these latest tools helping to raise the state of the art in RF exploration for the average enthusiast.

73,

Joe, NE2Z

