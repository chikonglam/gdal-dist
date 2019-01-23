## Installation
1. Download the .deb files, and install the *gdal-bin*, *gdal-data* and *libgdal* deb with the following command:
  * `sudo  dpkg -i gdal-bin*.deb gdal-data*.deb libgdal20*.deb`

2. Check if the deployment is successful with the following command:
  * `apt list -a gdal-bin gdal-data libgdal20`
  
  If the deployment was successful, should be a *gdal-bin/now*, *gdal-data/now*, and a *libgdal20/now* entry that ends with dds, like the following:
  ```
gdal-bin/now 2.2.3+dfsg-2dds amd64 [installed,local]
gdal-data/now 2.2.3+dfsg-2dds all [installed,local]
libgdal20/now 2.2.3+dfsg-2dds amd64 [installed,local]
  ```

3. To check with gdalinfo, use the following command:
  * `gdalinfo --formats | grep DDS`
  
  If the one in your system is really the DDS enabled version, there should be an output like the following:
  
  `DDS (rwv): DirectDraw Surface`
