# Steps for L2 processing:
Mosaic and map daily L2 images using gpt operator.

Three product suites: OC, SST, IOP.

Input files: /srv/imars-objects/gom/L2_MODA_r2018/OC (or SST4, SST, IOP).

Tasks:
1. Read input files and parse filenames by year and day of year (DOY)
2. Loop on year/DOY and create a gpt calling sequence for each year/DOY/product suite
3. Eeach ROI and product suite needs an xml graph with processing parameters (spatial extent, products, bandmaths)
4. GPT calling sequence: '/opt/snap_6_0/bin/gpt ' xml_file ' -t ' path_out 'V' time_start '_' roi_2 '_' pc '_1D.nc -f NetCDF-BEAM ' list of output files ''';'])
5. Execute calling sequence
6. Output L3 daily files go here: /srv/imars-objects/fk/L3_1D_MODA/OC (or SST,SST4,IOP)

Parameters to consider:
Sensors: VSNPP and MODA (could add S3)

ROI: fk, fgb, wfs, gom, other?

Product suites: OC, SST/SST4, IOP
