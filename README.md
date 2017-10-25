# DimuonSpectrum2011

This is a simple analysis example to compute the spectrum of two muon final state with CMS Open Data.

Run this code in CMS Open Data VM [http://opendata.cern.ch/VM/CMS/2011]
```
cmsrel CMSSW_5_3_32
cd CMSSW_5_3_32/src
cmsenv
git clone https://github.com/cms-opendata-analyses/DimuonSpectrum2011.git

cd DimuonSpectrum2011
scram b

cmsRun demoanalyzer_cfg.py
```
The output of the example is a root file containing several histograms, by default DoubleMu.root with 10000 input events (small subset of data). These can be looked at using a Root Browser.

For more detailed information, read the comments in src/Demoanalyzer.cc.
