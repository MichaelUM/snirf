# Shared Near Infrared Spectroscopy Format (SNIRF)

This repository stores the Shared Near Infrared Spectroscopy Format (SNIRF).  
SNIRF is designed by the community in an effort to facilitate sharing and analysis of NIRS data.

View the most recent release version of the format: [here](https://github.com/fNIRS/snirf/blob/da550abf7ec70084e31ba428df09a9dcbf3e6036/snirf_specification.md).  
View the development version of the format: [here](snirf_specification.md).   


## User Information

To browse the latest version of the SNIRF Specification document, you may click on 
[this link](snirf_specification.md). A history of changes to the specification and
information on released versions is available in the [change log](CHANGELOG.md).

The following software packages support reading and/or writing SNIRF files.

| Software       |                   URL                        |
|----------------|----------------------------------------------|
| Homer2         | https://homer-fnirs.org                      |
| Homer3         | https://github.com/BUNPC/Homer3              |
| MNE-Python     | https://mne.tools                            |
| NIRS-Toolbox   | https://github.com/huppertt/nirs-toolbox     |
| FieldTrip      | https://www.fieldtriptoolbox.org             |
| NIRStorm       | https://github.com/Nirstorm/nirstorm         |


The following vendors export data in SNIRF format.

| Vendor         |              URL                 |
|----------------|----------------------------------|
| NIRx           | https://nirx.net                 |
| Kernel         | https://www.kernel.com           |


## Development Information

To download the latest specification document alone click on this
[download link](https://github.com/fNIRS/snirf/archive/master.zip),
or use the below command
```
   git clone https://github.com/fNIRS/snirf.git
```

You may optionally download the sample data, or a parser that you need. To do so, you need
to first `cd` the folder where the snirf repository was cloned, and then run the below commands
```
   cd snirf                                # cd the folder where the repo was cloned
   git submodule update samples            # checkout the sample data files (needs >240MB)
   git submodule update lib/matlab/easyh5  # checkout a specific matlab parsers, or
   git submodule update --init --remote    # checkout all components
```

To download the entire package at once, including the latest specification document, 
sample files and all currently supported parsers, you should use the below command
```
   git clone --recursive https://github.com/fNIRS/snirf.git
```


### Sample files and parsers

The latest versions of the individual submodules, including sample data and parsers, can also 
be downloaded by clicking on the the below links. After download, please follow the README
file in each package for instructions on how to use.

| Submodule      |                               URL                         |
|----------------|-----------------------------------------------------------|
| sample data    | https://github.com/rob-luke/BIDS-NIRS-Tapping/archive/master.zip   |
| EasyH5 Toolbox | https://github.com/fangq/easyh5/archive/v0.8.tar.gz       |
| JSNIRF Toolbox | https://github.com/fangq/jsnirfy/archive/v0.4.tar.gz      |
| SNIRF_HOMER3   | https://github.com/fNIRS/snirf_homer3/archive/master.zip  |

[This page](https://github.com/BUNPC/Homer3/wiki/Standalone-SNIRF-loading-and-saving)
provides examples of how to work with SNIRF files using the
[Homer3](https://github.com/BUNPC/Homer3) interface.
