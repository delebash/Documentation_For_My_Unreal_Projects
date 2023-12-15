
## 1) <u>Intro</u>

Make your landscape interact with weather, wind, water, foliage and your player like the real world.  Global Environmental System or GES for short combines various systems with Ultra Dynamic Sky and Weather to make your environment act more like the real world.  As you change the weather from Calm Skies to Thunderstorm your foliage and trees will change in speed accordingly. **NOTE:** Ultra Dynamic Sky is the only requirement and is a paid plugin on the UE Marketplace you can get <a href="https://www.unrealengine.com/marketplace/en-US/product/ultra-dynamic-sky" target="_blank">here</a> 

Video Demo <div style="position: relative; width: 100%; padding-bottom: 56.25%">
<iframe src="https://www.youtube.com/embed/CfE0y1k4r6w" 
        title="GES Demo" frameborder="0" allowfullscreen
        allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" 
        style="position: absolute; width: 100%; height: 100%;">
</iframe>
</div>


## 2) <u>What you get</u>

1) Global Environmental System Blueprint (GES) -- Change wind strength, direction, seasons, health, and weather effects on trees, foliage and props such as rocks or logs. Season and health changes are limited to Megascan trees and foliage.

2) Ultra Dynamic Sky/Weather Integration -- Weather effects are added to MS Materials. https://www.unrealengine.com/marketplace/en-US/product/ultra-dynamic-sky?sessionInvalidated=true

2) Megascan Foliage and Trees Integration  -- Wind and Weather effects added. Trees https://www.unrealengine.com/marketplace/en-US/product/megascans-trees-european-hornbeam-early-access

3) Foliage Interaction and Wind System -- This system was extracted and modified from the awesome Project Nature pack -- Permenantly Free Nature Assets on UE Marketplace https://www.unrealengine.com/marketplace/en-US/profile/Project+Nature?count=20&sortBy=effectiveDate&sortDir=DESC&start=

4) Foliage Health And Season -- Adjust the color of your foliage.  Extracted from MS Global Foliage Actor. Season color change linked to UDW season change for Megascan foliage and trees.

5) Ambient Wind System Integration -- Enable any actor to receive wind  https://www.unrealengine.com/marketplace/en-US/product/ambient-wind-system

6) Project Nature Integration   -- https://www.unrealengine.com/marketplace/en-US/profile/Project+Nature?

6) UE Water Integration -- Change the Wave Asset file based on the current Weather 

7) SpeedTree Integration 

8) Brushify Integration

9) MAE Integration

10) Particle and Wind Control System Integration -- Free from Unreal https://www.unrealengine.com/marketplace/en-US/product/particles-and-wind-control-system

11) Mawi Integration -  Wind and direction don't work as well as the other systems due to Mawi's wind system.

12) Easily add any other system for basic wind speed and direction change by changing that systems Material Parameter Collection values.  Example included.

## 3) <u>Installation</u>

1) GES has many systems already integrated.  You need to download the systems you want to use and add them to your project before installing GES.  For example if you are using Brushify make sure it is added to your project first.

2) Download the latest release for your version of Unreal.  Currently only the latest version of UE will receive bug fixes and enhancements.  Download the release from <a href="https://github.com/delebash/UE_GlobalEnvironmentalSystem/releases" target="_blank">here</a>

3) Unzip the download and copy the Content and Plugin folder to your root project folder.

5) Setup individual systems, see next section


## 4) <u>Individual System setup</u>

### Megascan Setup

1) First you need to download some megascan assets so that all the default materials will be downloaded that we will eventually overwrite some of them in the MSPreset folder.

2) When you download MS assets it creates an MSPreset folder with the materials for the asset type you downloaded.

3) List of materials that will need to be downloaded in the MSPreset folder.  You only need to download what you will use.  The _VT will only show up if you have Runtime Virtual Textures enabled for your project.  

> MS_Foliage_Material, M_MS_Surface_Material_VT, M_MS_Surface_Material, M_MS_Foliage_Material, M_MS_Default_Material_VT, M_MS_Default_Material, M_MS_Default_Fuzz_Material_VT, M_MS_Default_Fuzz_Material, M_MS_Billboard_Material

> Example downloads I use. I download a rock or log -- uses the M_MS_Default_Material.  Next a rock with moss -- uses the M_MS_Default_Fuzz_Material.  Some foliage -- uses M_MS_Foliage_Material. A Surface -- M_MS_Surface_Material. A Tree pack - use the MS_Foliage_Material.

4) With your project closed.  From your folder explorer in your projects Content Folder, navigate to the folder GlobalEnvironmentalSystem --> Integrations --> Megascans.  Copy the MSPreset folder and paste it in your Content folder overwriting the existing MSPreset folder. 

#### Material Instance for Foliage
##### Wind

I have replaced the default wind for Megascan foliage with Project Natures foliage and interaction system. For each MI you will need to check the 3 check boxes shown below under Preset Parameters. 
![](../_images/megascan%20wind.png)

Additional information on wind and bending settings can be found in the [Project Nature Documentation](./ProjectNatureDocumentation.pdf)

##### Ultra Dynamic Weather and Automatic Season

1) Check box Use UDW Weather ? and enable it.  
  

2) Megascan foiliage material also has automatic integration with UDW season change. To enable check the boxes for Use UDS date For Autumn? and/or Use UDS date For Winter?.  Additional settings for withered leaves will become available.

3) Once you have enabled Use UDS Date scroll up to the Seasons section and enable Affected by Winter/Autumn.  Additional Autumn settings will be available.

![](../_images/ms%20foliage%20enable%20udw.png)

![](../_images/udw%20season%20affected%20by.png)

##### Manual Health and Season
If you are not using automatic season change you can check the Seasons checkbox and manually adjust the color.  In addition there are global settings in the BP_GES for seasons.


#### Material Instance for Trees
For trees the wind system is the default system that comes with MS trees.  I have added Project Nature interaction to the tree materials.  In addition we have UDW and season change.

1) To enable UDW and Season change select your tree in the scene or find the MI's for tree you want. You will notice several MI's for leaves, bark, and imposter.  For each MI you will need to enable settings to get the effect you want.


![](../_images/blackalder%20mi.png)

2) Open the leaves MI.  Check enable Use UDW Weather?

![](../_images/ms%20tree%20enable%20udw.png)


##### Ultra Dynamic Weather and Automatic Season

MS tree leaves have the same settings as MS foliage except in how you enable winter.  MS trees has the Season setting enabled by default.  .

![](../_images/ms%20tree%20udw%20season.png)

To get automatic season change for Winter enable Winter under Season.  For Autumn enable affected by Autumn.
![](../_images/ms%20tree%20winter.png)

The Bark MI's only have Use UDW Weather ?

The Impostor has the same settings as the leaves, depending on performance you may or may not want to enable.


##### Manual Health and Season

Same as foliage

### Brushify Setup

1) With your project closed.  From your folder explorer in your projects Content Folder, navigate to the folder GlobalEnvironmentalSystem --> Integrations --> Brushify

2) Copy the Materials folder and paste in your Content --> Brushify folder overwriting the Materials folder.

### Project Nature Setup

1) With your project closed.  From your folder explorer in your projects Content Folder, navigate to the folder GlobalEnvironmentalSystem --> Integrations --> Project Nature

2) Copy the Materials folder and paste in each of your Project Nature packs folders overwriting the Materials folder.

3) If you want UDW weather effects you need to add that UDW function to the material function you want to use.  As an example for the spruce pack you can copy the PN_interactiveSpruceForest and overwrite the existing one.  All I am doing is adding the UDW function to it. GES comes with a convenience function that wraps the UDW Weather effects.  In the material you want to add the weather effects to type MF_ApplyWetnessSnowDustUDW and hook it up to your material at the end.

### SpeedTree setup

1) With your project closed.  From your folder explorer in your projects Content Folder, navigate to the folder GlobalEnvironmentalSystem --> Integrations --> SpeedTree

2) Copy SpeedTreeBillboardMaster.uasset and SpeedTreeMaster.uasset and overwrite those files in you Engine folder.  As an alternative in your project make sure you show your Engine folder by clicking the asterick and checking Show Engine.  Search for each of the above assets and for each one choose delete and then in the delete window choose replace.  In the replace with choose the assets with the same name inside the Integrations --> SpeedTree folder. 


### Mae -- no setup needed

### Mawi -- no setup needed

### Particle and Wind Control System -- no setup needed

### Ambient Wind System -- no setup needed

## 5) <u>Add GES Blueprint to your Scene</u>

1) Navigate to GlobalEnvironmentalSystem --> Blueprints and drage BP_GES to your scene.
