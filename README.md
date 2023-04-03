*************************
CSSRlib - Toolkit for PPP-RTK/RTK in Python using Compact SSR
*************************

# What is CSSRlib? 

CSSRLIB is a open toolkit in Python for high accuracy GNSS positioning. It supports SSR (State-Space Representation) based potitioning such as PPP (Precise Point Positioning) or PPP-RTK (Realtime Kinematic), but also supporting RTK. The goal of the CSSRlib toolkit is to provide an easy-to-understand open implementation to learn PPP/PPP-RTK positioning provided by satellite-based open PPP/PPP-RTK services such as QZSS CLAS, Galileo HAS, BeiDou 3 PPP. It also supports ground based open service by IGS. The code is based on RTKlib.

It supports the following open format:

- The obserbation data and the ephemeis in RINEX
- The PPP/PPP-RTK correction data in RTCM SSR, IGS SSR, Compact SSR, ...
- The precise orbit/clock data in SP3 format.

Prerequisites
=============
Additional python packages are required as prerequisites and can be installed via the following commands

```
pip install bitstruct
pip install cbitstruct
pip install galois
pip install cartopy
```

If the installation of `cartopy` fails, try installing `libgeos++-dev` first.

```
sudo apt-get install libgeos++-dev
```

Install
=======
You can install CSSRlib using pip.

```
pip install cssrlib
```

additional python packages are required as prerequisites and can be installed via the following commands:

```
pip install notebook, numpy, matplotlib
pip install bitstruct,cbitstruct,galois,cartopy
```

Testing
=======

Run orbit plot sample.

```
python test_eph.py
```

Run RTK sample.

```
 python test_rtk.py
```

Other samples are also available in a separate repository `cssrlib-data` including :

- Galileo-HAS decoder
- BDS-PPP decoder
- Jupyter-Notebook including samples for RTK/PPP-RTK.

