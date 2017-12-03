# DimuonSpectrum2011

This is a simple analysis example to compute the spectrum of two muon final state with CMS Open Data.

Run this code in CMS Open Data VM [http://opendata.cern.ch/VM/CMS/2011]

If you have not installed the CMSSW area do the following:
```
cmsrel CMSSW_5_3_32
```
If you already have, start directly with:

```
cd CMSSW_5_3_32/src
cmsenv
```
For this example, you need to create an additional directory, you can call it `WorkDir` or choose another name.
Go to this directory, and download the example code.

```

mkdir WorkDir
cd WorkDir
git clone https://github.com/cms-opendata-analyses/DimuonSpectrum2011.git

```
Go to the example directory, and compile with `scram b`. 

```
cd DimuonSpectrum2011
scram b
```
Run the example as configured in the configuration file. 

```
cmsRun demoanalyzer_cfg.py
```
The output of the example is a root file containing several histograms, by default DoubleMu.root with 10000 input events (small subset of data). These can be looked at using a Root Browser.

For more detailed information, read the comments in src/DimuonSpectrum2011.cc.
