
## Intro

Make your landscape interact with weather, wind, water, foliage and your player like the real world.  Global Environmental System or GES for short combines various systems with Ultra Dynamic Sky and Weather to make your environment act more like the real world.  As you change the weather from Calm Skies to Thunderstorm your foliage and trees will change in speed accordingly. **NOTE:** Ultra Dynamic Sky is the only requirement and is a paid plugin on the UE Marketplace you can get <a href="https://www.unrealengine.com/marketplace/en-US/product/ultra-dynamic-sky" target="_blank">here</a> 

Video Demo <div style="position: relative; width: 100%; padding-bottom: 56.25%">
<iframe src="https://www.youtube.com/embed/CfE0y1k4r6w" 
        title="GES Demo" frameborder="0" allowfullscreen
        allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" 
        style="position: absolute; width: 100%; height: 100%;">
</iframe>
</div>


## What you get

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


### Copy Folders

If you want, you can show a loading dialog before docsify starts to render your documentation:

```html
<!-- index.html -->

<div id="app">Please wait...</div>
```

You should set the `data-app` attribute if you changed `el`:

```html
<!-- index.html -->

<div data-app id="main">Please wait...</div>

<script>
  window.$docsify = {
    el: '#main',
  };
</script>
```

Compare [el configuration](configuration.md#el).