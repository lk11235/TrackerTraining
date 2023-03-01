# TrackerTraining

### Updated twiki with instructions to compile and run the HipPy algorithm
[SWGuideHipPyAlgorithm < CMSPublic < TWiki (cern.ch)](https://twiki.cern.ch/twiki/bin/view/CMSPublic/SWGuideHipPyAlgorithm)

### Legacy page with further information about HipPy options
[SWGuideHIPAlgorithm < CMSPublic < TWiki (cern.ch)](https://twiki.cern.ch/twiki/bin/view/CMSPublic/SWGuideHIPAlgorithm)

### OOTB working example
1. Compile HipPy with the appropriate CMSSW release (`CMSSW_12_4_9` for this example)
2. Copy the sample configuration files into your run directory 
3. Edit the run number and paths in `submit_template.sh` to avoid overwriting past alignments
    1. Previous runs are listed in `/afs/cern.ch/cms/CAF/CMSALCA/ALCA_TRACKERALIGN2/HipPy/alignments` 
5. If you have tier computing access as part of the Alignment group, you should load the tzero module with `module load lxbatch/tzero`
6. Make sure your VOMS proxy is initialized with `voms-proxy-init --voms cms`
7. Commit your changes and run `./submit_script.sh submit_template.sh`
