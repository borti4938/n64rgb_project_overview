N64RGB Projects
---

### History and Introduction

The N64 projects presented here were part of a single repository, which is for versioning still an accessible [archive on Github](https://github.com/borti4938/n64rgb).

The project started with a tiny THS7374 based RGB bypass board back in 2015 or so.
Later, I started with writing my code for viltetims N64RGB as I was wishing to have features like VI-DeBlur (skipping interpolation pixels in 320x240 video mode) and a reset which can be triggered via a controller combination (in game reset).
Things were going, I designed a DIY PCB for myself allowing me to add new features.

Over the time the repository grew a lot, especially with the N64Advanced project and the N64Advanced2.
For an easier management and maybe also to give interested people an better overview on the different projects I decided to break down the different parts into several dedicated repositories.
My greatest wish is that features like release and issue tracking will be a lot easier as they can be focused in smaller repositories instead of being hidden in a large one.

The projects are meant as "Do It Yourself"-projects (DIY-projects).
So the repositories should be sufficient that everybody having appropriate knowledge (e.g. knowing how to order PCBs, sourcing components, soldering skills for assembly and installation) are able to build everything on its own.
However, there are some shops out there selling ready to install modification kits and/or offering installation services.
I am not affiliated to any of those shops, which means that I do not get any profit of their sales (besides of testing prototypes, one time gifts or donations, thinks like that).

So, if you like what I am doing, please consider leaving me a short message via email or twitter or even buying me a coffee or two (link on my GitHub profile page) like many others did.
Thank you very much - I really appreciate any kind of feedback!
It helps me keeping my motivation up for further projects.
This hobby is very time consuming and especially the N64Advanced and N64Advanced2 were very intensive projects for me.

Back to topic.
In the following I will guide you to the different projects.
The repositories are linked.


### Brief Description of Projects

#### N64Advanced
  
- FPGA based digital to analog video mod with advanced feature set compared to smaller CPLD based RGB mods
  - Outputs RGB, RGsB, YPbPr
  - Line doubling (480p / 576p) and trippling (NTSC only, 720p (non-standard)) incl. (simple) scanline emulation
  - VI-DeBlur
  - 16bit mode
  - In game reset
  - On screen menu for configuration
  - ...
- Repository for PCB: [n64adv\_pcb](https://github.com/borti4938/n64adv_pcb)
  - PCB file, BOM, etc. for DIY or production
  - Kit installation instruction
  - Please note that flexible PCBs assisting installation can be found in [n64rgb\_project\_misc](https://github.com/borti4938/n64rgb_project_misc)
- Repository for Firmware: [n64adv\_fw](https://github.com/borti4938/n64adv_fw)
  - Firmware for hardware kit
  - User Information
  - Developer Information


#### N64Advanced2

- FPGA based digital to digital video mod with advanced feature set and powerful scaling capabilities
  - Comparable to N64Digital and UltraHDMI, both great modding kits, but this is open source: DIY
  - Resolution up to 1440p
  - Flexible scaler for each resolution
  - Scanline emulation
  - VI-Deblur, 16bit mode
  - In game reset
  - On screen menu for configuration
  - ...
- Repository for PCB: [n64adv2\_pcb](https://github.com/borti4938/n64adv2_pcb)
  - PCB files (main, flex), BOM, etc. for DIY or production
  - Kit installtion instruction
- Repository for Firmware: [n64adv2\_fw](https://github.com/borti4938/n64adv2_fw)
  - Firmware for hardware kit
  - User Information
  - Developer Information


#### N64RGB

- A CPLD based digital to analog video mod
  - A rather simple universal RGB modding kit
  - Comparable to the commercial solution of viletim, but with a dedicated digital to analog converter IC instead of a r2r ladder
  - VI-DeBlur and 16bit mode switchable with the controller or with a mechanical switchable
  - In game reset via controller
- Repository for PCB: [n64rgb\_pcb](https://github.com/borti4938/n64rgb_pcb)
  - PCB file, BOM, etc. for DIY or production
  - Kit installation instruction
  - Please note that flexible PCBs assisting installation can be found in [n64rgb\_project\_misc](https://github.com/borti4938/n64rgb_project_misc)
- Repository for Firmware: [n64rgb\_fw](https://github.com/borti4938/n64rgb_fw)
  - Firmware for hardware kit
  - User Information
  - Developer Information


#### N64RGB for Viletims Commercial Modding Kit

- An alternative firmware for [viletims N64RGB](http://www.etim.net.au/n64rgb/)
  - VI-DeBlur and 16bit mode switchable with the controller or a mechanical switchable
  - In game reset via controller
- Repository for Firmware: [n64rgb\_viletim\_fw](https://github.com/borti4938/n64rgb_fw4viletim)
  - Firmware for viletims commercial hardware kit
  - User Information
  - Developer Information


#### Miscellaneous Add Ons

- Several helpful tiny projects for the other N64RGB projects
- Repository: [n64rgb\_project\_misc](https://github.com/borti4938/n64rgb_project_misc)
  - Filter AddOn
  - Flexible PCBs for N64RGBv2.1 and N64Adv installation
  - Power Regulator for older/other CPLD based N64RGB kits
  - THS7374 based RGB amp for N64s already outputting RGB


### Acknowledgement

This project would not be what is with the help and contribution of many other people.
The following 'list' is neither sorted by importance, nor complete.

Of course, many thanks to viletim for his initial CPLD-based DAC project, for providing a valuable commercial modding board as well as for publishing the schematics and source codes for his [N64RGB project](http://www.etim.net.au/n64rgb/).

I also want to send many thanks to Ikari_01.
He wrote the code to detect 480i and PAL/NTSC output of the N64 with the CPLD.
He provides a source code for the XC9572XL, which can be accessed here: [URL to Ikari_01's GitHub repository](https://github.com/mrehkopf/n64rgb)

Many thanks to Bob and his website contributors for his website [RetroRGB](http://retrorgb.com) and especially in this context here for collecting and sharing all the [RGB information regarding the N64](http://retrorgb.com/n64.html).

Thank you very much also to many, many other persons, not limited to sftwninja, Xenogears, ArcadeTV, ManCloud, TzorriMahm, marqs85, ...
