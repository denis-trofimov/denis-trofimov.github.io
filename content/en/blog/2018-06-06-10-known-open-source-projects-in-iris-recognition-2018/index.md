---
title: 10 Known Open Source Projects in Iris Recognition 2018
authors:
  - me
type: blog
date: 2018-06-06T20:33:50+00:00
featured_image: Eye-Photo-by-Tom-Tolkien.jpg

categories:
  - iris recognition
tags:
  - c++
  - code
  - dataset
  - iris recognition
  - iris segmentation
  - matlab
  - open source
  - project
  - python

---

I found this pretty good list of [Iris Recognition open-source codes][1]. I am really appreciate work of the first author, [thanhkien84][2]. I asked myself, how to improve it? I have decided to add my value.

I have checked all links and found replacements for stale links to projects OSIRIS, UND.

In the year 2003 there was only one iris recognition open source code from Libor Masek. His source code, written in Matlab, has been the baseline for generations of iris recognition coders. Recently there are a number of new open source codes come up. They are more mature and meet state-of-the-art accuracy. I summarise them in a list here for your reference.
<!--more-->

| Iris recognition projects | Year/ Language | Approach | Performance (EER) |
|-------------------------|----------------|----------|-------------------|
| | | | ICE 2005 | MBGC portal | CASIA |
| | | | | | |
| Libor Masek [project][3] | 2003, Matlab | Hough Circle + 1D Log-Gabor | | | |
| OSIRIS 4.1 [project dead link][4] | 2013, C++ | Least square, Circle + 2D Gabor | 1.09% | | |
| 5455945/Iris_Osiris [project][5] | 2017, C++ | Same as OSIRIS 4.1 | | | |
| (OSIRIS 4.1 fork) Support OpenCV3.0+,OpenCV2.4.13 | | | | | |
| Python interface to OSIRIS Iris Segmentation and Recognition software [project][6] | 2017, Python | Same as OSIRIS 4.1 | | | |
| (OSIRIS 4.1 fork) | | | | | |
| VASIR 2.2 [project][7] | 2013, C++ | Circle + 2D Gabor | 3.5% | 13.9% best quality frame <br> 30.6% all frames | |
| NonidealIRIS [project] | 2006, Matlab | Ellipse +  2D, Gabor | | | |
| USIT [project][8] | 2016, C++ | Circle/Ellipse+ <br> 1D Log Gabor/ <br> 2D Gabor/ <br> DCT/ SIFT/ <br> SURF/LBP | | | | 0.82% |
| UND [project][9] | 2016, Matlab | Circle, <br> Crypts features | 3.58% | | 1.39% |

### Iris segmentation only

| IrisSeg [project][10] | 2017, Matlab | | ICB 2016 | IrisSeg: A Fast and Robust Iris Segmentation Framework for Non-Ideal Iris Images |
| IAADseg [project][11] | 2015, Matlab | Total-variation | ICCV 2015 | An Accurate Iris Segmentation Framework under Relaxed Imaging Constraints using Total Variation Model |
| IrisSeg [project][12] | 2015, Python | Geodesic Active Contours and GrabCut | PSIVT 2015 | Iris Segmentation using Geodesic Active Contours and GrabCut |

Iris datasets to consider:

| Dataset | Subset | Number of subjects | Number of images | Spectrum | Note |
|---------|--------|-------------------|-----------------|----------|------|
| **CASIA** | | | | | |
| CASIA-Iris-Thousand | | 10,000 | 20,000 | NIR | |
| CASIA-Iris-Interval | | | | Time lapse | |
| CASIA-Iris-Lamp | | | | | |
| CASIA-Iris-Twins | | 100 | | Twin | |
| CASIA-Iris-Distance | | | | At a distance | |
| CASIA-Iris-Syn | | 1000 | 10,000 | Synthesis | |
| **ND** | | | | | |
| ND-IRIS-0405 | | 356 | 64,980 | NIR | |
| ND-GFI | | | | Gender | |
| NDCLD15 | | 750 males <br> 750 females | 3000 | NIR | Contact Lens |
| ND-CrossSensor-Iris-2013 | | 676 | 29,986 from LG4000 and 116,564 from LG2200 | NIR | Cross Sensor |
| ND-TimeLapseIris-2012 | | 23 | 6797 | | Time lapse 2004 to 2008 |
| ND-Iris-Template-Aging-2008-2010 | | | 11,776 | | Time lapse 2008 to 2010 |
| **MBGC** | | | | NIR & NIR videos | One the move |
| **UBIRIS** | | 261 | 11,102 | Visible | On the move <br> At a distance |

&nbsp;

My sources:

1. [Iris Recognition open-source codes][1]
2. [What are some of the best open source iris recognition libraries available?][13]

- Eye Photo by Tom Tolkien [http://thomastolkien.wordpress.com/][14]

[1]: https://kiennguyenstuff.wordpress.com/2016/07/14/iris-recognition-open-source-codes/
[2]: https://kiennguyenstuff.wordpress.com/author/thanhkien84/
[3]: http://www.peterkovesi.com/studentprojects/libor/
[4]: http://svnext.it-sudparis.eu/svnview2-eph/ref_syst/Iris_Osiris_v4.1/
[5]: https://github.com/5455945/Iris_Osiris
[6]: https://github.com/vonclites/syris
[7]: http://www.nist.gov/itl/iad/ig/vasir.cfm
[8]: http://www.wavelab.at/sources/USIT/
[9]: https://ideacenter.nd.edu/commercialization-engine/for-industry/available-technologies/software-available-for-license/iris-recognition-based-on-human-intrepretable-features/
[10]: https://github.com/cdac-cvml/IrisSeg
[11]: http://www4.comp.polyu.edu.hk/~csajaykr/tvmiris.htm
[12]: https://github.com/sbanerj1/IrisSeg
[13]: https://www.quora.com/What-are-some-of-the-best-open-source-iris-recognition-libraries-available
[14]: http://thomastolkien.wordpress.com/