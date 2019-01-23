## Installation
1. Download the .deb files, and install the *gdal-bin* and *libgdal* deb with the following command:
  * `sudo dpkg -i gdal-bin_1.11.3+dfsg-3build2dds_amd64.deb libgdal1i_1.11.3+dfsg-3build2dds_amd64.deb`

2. Check if the deployment is successful with the following command:
  * `apt list -a gdal-bin libgdal1i`
  If the deployment was successful, should be a gdal-bin/now, and a libgdal1i/now entry that ends with dds, like the following:
  ```
   gdal-bin/now 1.11.3+dfsg-3build2dds amd64 [installed,local]
   libgdal1i/now 1.11.3+dfsg-3build2dds amd64 [installed,local]
  ```
3. To check with gdalinfo, use the following command:
  * `gdalinfo --formats | grep DDS`
  If the one in your system is really the DDS enabled version, there should be an output like the following:
  `DDS (rwv): DirectDraw Surface`
