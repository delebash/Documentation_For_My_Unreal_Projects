# Help -- Download heightmap, satellite, weightmap images for use in Unreal or other 3D programs

## Getting Started:
   1. Get an api key from Mapbox or Maptiler free account
   2. Open the Settings Panel and select either mapbox or maptiler from the Server Type dropdown
   3. Paste your api key
   4. Select a download directory
   5. Click the Save Button

## Map Controls:
   1. Left click to select an area
   2. Shift scroll to increase decrease the selection area
   3. Use mouse scroll to change your viewpoint, this does not change the heightmap size
   4. Left click and hold to move around the map
   5. Right click and hold to pan and tilt

## Info Panel:

Search box -- find a location by name and move the selection to that location

Map size -- increase decrease selection area

Auto calculate Base & Height -- Automatically chooses the best settings for heightmap creation

Base Level -- Changes the start altitude for your heightmap, More white means your start altitude is higher

Height Scale -- Changes the scale of your height

Water depth -- Slightly modifies height

Preview -- Loads the preview image based on your settings

## Export Options Panel:

Export Settings:

1. Export type -- Choose download png to manually download the heightmap to your directory
or choose import heightmap to automatically import into Unreal requires Bridge Plugin
3. Landscape Size -- resize the image to create the the size of your landscape in Unreal

Export type:

Override satellite zoom level -- higher zoom level equals better resolution, try 13 to start
The higher the zoom level means you will download more files, check your Tile count after you enter your zoom level
Too high of a zoom level could mean downloading thousands of files

Select image types to download:
Check one or all of the options

Manipulate heightmap: -- only applies to heightmap

Sea level -- Adjusts the heightmap so when you import into Unreal the map is at sea level -- default checked

Flip X -- Flips the image on the X axis

Flip Y -- Flips the image on the Y axis

Other Settings:

Enable World Partition -- Only applies when you Automatically import your heightmap into Unreal using the plugin

Grid Size -- Same setting in Unreal when you import your landscape with World Partition

Blur radius -- Applies a blur to your heightmap, can help smooth out your Unreal landscape
The higher the number the more smoothing is applied

Weightmap Blur -- Applies smoothing to your Weightmap images. Higher value equals more blur

Landscape Name -- Name of your landscape when you use the automatic import into Unreal

Export Button -- Start the creation of your selected image types -- Note sometimes the progress bar
Will freeze. Just be patient and wait for it to disappear. Downloading Weightmaps can take some extra time

Change map style Panel: -- changes what type of map you want to view

## Set lng/lat Panel:

Manually input lng/lat and move the selection to that location

## Settings Panel:

Api Key -- Paste the api key you got from either mapbox or maptiler
 
Weightmap Url -- <a href="https://api.mapbox.com/styles/v1/delebash/clfzz7dot000001qilz330eyt.html?title=copy&access_token=pk.eyJ1IjoiZGVsZWJhc2giLCJhIjoiY2xvYTR5d3NtMGZxdTJxbmJ2cjU5NjkyNCJ9.vzDIXEYSjfHszDBShCNanQ&zoomwheel=true&fresh=true#16.54/27.987686/-80.590789/0/7" target="_blank">Click Mapbox Weightmap Style</a> to copy this style to your mapbox account and then paste your new style address in text box below in the format name/style id example:

Desktop Server Url -- The backend server is for use when you need to download satellite images with a zoom greater than 14. You will need to download the desktop version from here Double click on the exe to start the application. Export image per normal, sat images will be processed on the backend. This could take a long time depending on how many tiles you are processing.

Desktop Directory: -- Directory to save images produced from the desktop app such as C:\map\sat_images. If you are using the automatic heightmap import via the plugin make this directory the same as Download Directory

## Weightmap Panel:

These list to colors to match features from the Weightmap style to create your
weightmap images. For now don't change and this only works in Mapbox
Just copy your user name/map id from Mapbox Studio Share button style url
The number on the left bar is your current viewing zoom level:
Use this to get an idea of what you will see when you download your satellite image with that zoom level