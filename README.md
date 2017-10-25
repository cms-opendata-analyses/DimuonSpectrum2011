# DimuonSpectrum2011

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

