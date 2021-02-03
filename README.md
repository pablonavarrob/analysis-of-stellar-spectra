# Data Science Project: Analysis of Spectroscopic Data

The field of Astrophysics lends itself to be studied through diverse types of observational data and a myriad of different analysis techniques. While many traditional methods have proven very successful so far, they might no longer be suitable for exploiting the full potential of the high-dimensional and highly non-linear data being gathered almost daily, on the order of terabytes per night. The challenges posed by these large, complex data sets demand a perspective change and a shift towards more efficient and scalable solutions. Some of these new solutions do include approaches that are derived directly from known Machine Learning or Artificial Neural Networks. For these reasons, many firmly believe that the field of Astrophysics requires a swift transition to a methodology appropriate for the era of Big Data, which has the potential to change the paradigm in the field and the way we perceive it [1], [2].

Astronomical data sets have very different origins and natures: some are time series (mostly aperiodic, due to the difficulties that repeated observations arise in astronomy, e.g. cloudy skies, telescope malfunctions, etc.), other are comprised of photometry values while others measure the amount of light per unit wavelength from stars. It is this last type, that we will be dealing with throughout this project and it receives the name of spectroscopy or spectroscopic data. Ever since its discovery, spectroscopy has become one of the best ways astronomers have to study stars as they do not need to be fully resolved to extract important information from. In the recent years, there has been a consistent increase in the amount of spectroscopic surveys and in the amounts of data available (such as and the RAdial Velocity Experiment, Rave [3], or GALactic Archeology with Hermes, GALAH [4]).

Spectroscopic data consists of one flux (light intensity) per wavelength unit, given by the sampling (process that converts continuous analog signal to discrete digital, quantization). Essentially this means that for measurements with a sampling of 0.004 nm/px and a range of 100 nm in wavelength there will be 25.000 measurements, which in turn indicates that each star will stand for data point and comprise 25.000 individual features or dimensions. Due to this high dimensionality, spectroscopic data lends itself to be studied through Data Science methods. For our purposes, it is comprised by a constant level or continuum which fluctuates around 1 (fluctuations due to noise and other processes) and large dips in the continuum, called absorption lines. While the approaches to handle spectra involve, generally, the usage of synthetic, self made templates for a given type of star (obtained through simulations), we will try a different, much simpler approach based on statistical modelling of the spectral lines and the use of machine learning for their analysis. Within the scope of this project is to define a model to replicate the shape of one of the spectral lines present in the data, obtain as series of parameters to reduce the dimensions of the spectra, and create a machine learning model, trained on this data, to perform classification tasks on a set of labels. Through this procedure, we aim to present a simple way to find whether a single line leads to better results than others.

<br>
![](spectrum_plot_20111023_0359m65_106_teff5486.png)

#### Resulting Figures 


#### References

[1] D. Baron, “Machine learning in astronomy: a practical overview,” 2019.

[2] M. Su ̈veges, F. Barblan, I. Lecoeur-Ta ̈ıbi, A. Prˇsa, B. Holl, L. Eyer, A. Kochoska, N. Mowlavi, and L. Rimoldini, “Gaia eclipsing binary and multiple systems. supervised classification and self-organizing maps,” Astronomy and Astrophysics, vol. 603, p. A117, Jul 2017.

[3] M. Steinmetz, G. Guiglion, P. J. McMillan, G. Matijevic, H. Enke, G. Kordopatis, T. Zwitter, M. Valentini, C. Chiappini, L. Casagrande, et al., “The sixth data release of the radial velocity experiment (rave)–ii: Stellar atmospheric parameters, chemical abundances and distances,” arXiv preprint arXiv:2002.04512, 2020.

[4] S. Buder, S. Sharma, J. Kos, A. M. Amarsi, T. Nordlander, K. Lind, S. L. Martell, M. Asplund, J. Bland-Hawthorn, A. R. Casey, G. M. D. Silva, V. D’Orazi, K. C. Free- man, M. R. Hayden, G. F. Lewis, J. Lin, K. J. Schlesinger, J. D. Simpson, D. Stello, D. B. Zucker, T. Zwitter, K. L. Beeson, T. Buck, L. Casagrande, J. T. Clark, K. Cotar, G. S. D. Costa, R. de Grijs, D. Feuillet, J. Horner, S. Khanna, P. R. Kafle, F. Liu, B. T. Montet, G. Nandakumar, D. M. Nataf, M. K. Ness, L. Spina, G. Traven, T. Trepper- Garcia, Y.-S. Ting, R. Vogrincic, R. A. Wittenmyer, M. Zerjal, and the GALAH col- laboration, “The galah+ survey: Third data release,” 2020.

# License

MIT
