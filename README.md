# UnitySDR
UnitySDR is a beginner-friendly cross-platform sdr client using the SoapySDR library and Electron to package the application.

Currently in a non-working state of development. I am creating this project as a labor of love.
I am somewhat of a beginner in software-defined radio, however i can see the need for
cross-platform software that is easy to use and reasonably feature rich.

looking for developers to contribute their knowledge, specifically anyone that knows how to interact with the 
SoapySDR library. I am just one person right now, and I work full time, so I can only really work on this during my free time.
I am actively learning how to interact with this library better but it will take some time!

# Proposed Features
* Spectrum Scan:
  I wish to add a feature to the program that scans the entire working spectrum of a given sdr(to prevent overheating and such),
  or a selected chunk of spectrum, and uses some logic to quickly identify signals that are higher than the average noise floor
  by a given amount. EX: you scan 100Mhz - 150Mhz, and there is a signal with a high SNR(signal to noise ratio) at 113.500. The program would return this
  frequency in a list along with its SNR value, and any common signals found near this frequency.
  
* APT Decode:
  An incredibly popular beginner sdr project is receiving images from NOAA Satellites using APT. Currently, the premier software for
  decoding is windows optimized and abandoned (@WXtoIMG :/ ). I would like to use python to either live-decode the image so it can be
  seen as it builds, or add recording features for the APT decoder to use to create the image. Even though the NOAA Satellites are past
  their end of mission date, two of them still reliably transmit apt signals as they pass overhead. (eventually meteor-M2 decoding would be nice
  but I am unsure of how to accomplish that)
  
* Clean UI:
  Most SDR products have messy UIs made for pros or just designed poorly. By using Electron, we can write the UI in html/css, and any frameworks
  that are found to be useful. (I'm personally a fan of the Bulma CSS framework). This allows potentially much more customization than the 
  currently available cardware or OS-Specific applications that are widely used.
  
As this project is going to be built with both seasoned sdr users and beginners in mind, I'm always open to new feature suggestions. It's always
worth looking into the possibility of cool features, and nothing is necessarily too ambitious with the right people working the problem!

# Help Wanted
Currently I would love if anyone that is very familiar with the SoapySDR Library could help out with the backend. Im pretty seasoned in
front-end web development in html/css/js, but I am rather unfamiliar with Node.js and Electron, as well as working with low level
drivers and libraries to get the data they return.

feel free to send any email discussion to wnstudiosky@gmail.com
 
