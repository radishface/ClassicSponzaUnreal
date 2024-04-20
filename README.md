# Classic Sponza - Unreal Engine Remaster

![ClassicSponza-Unreal-0](https://github.com/radishface/ClassicSponzaUnreal/assets/1553981/d9163ffa-942f-4744-bb19-95d7483c19f1)

## Summary

The Atrium Sponza Palace scene is widely used by graphics programmers and artists. It provides an ideal lighting test environment as it contains both indoor and outdoor areas. 

The goal of this conversion was to modernize the project in key areas and make it compliant with modern rendering standards.

Please refer to the [Releases](https://github.com/radishface/ClassicSponzaUnreal/releases) page for Unreal Engine compatibility.

The Unity version of this project can be found [here](https://github.com/Unity-Technologies/Classic-Sponza).

### Features

- All textures and materials are PBR compliant.
- Physically accurate lighting and exposure.
- Manually created Lightmap UVs.
- Baked Global Illumination using GPU Lightmass.

## Setup

### Cloning the project

#### Using the GitHub Desktop client
Click on the green Code button at the top, and select *Open in Desktop* option.

#### Using alternative git clients
Paste the following web URL into your preferred git client: `https://github.com/radishface/ClassicSponzaUnreal.git`.

#### Using command line or terminal
Open your preferred command line application and enter the following command: `git clone https://github.com/radishface/ClassicSponzaUnreal.git`.

### Setting up the project in Unreal Engine
After importing the project, the correct level should open automatically. If it doesn't, please follow these steps:
1. Go to **Content > ClassicSponza > Maps**.
2. Open the **SponzaPersistent** level file.
3. In the top menu bar, navigate to **Window > Levels**.
4. Make sure that **SponzaGeometry** and **SponzaLightingDay** are nested under the **Persistent Level** dropdown.

To access the flythrough sequence and screenshot cameras, simply drag and drop the **SponzaCinematics** level into the **Levels** window after following the steps above.

## Troubleshooting

### LIGHTING NEEDS TO BE REBUILT message in the viewport
1. In the top menu bar, navigate to **Build > GPU Lightmass**.
2. In the window that opens, uncheck the **Viewport Realtime is ON** checkmark. This will speed up the baking process.
3. Click on the green **Build Lighting** button.
You can also build the lighting using the old CPU Lightmass, though keep in mind that the results will not be the same.

### REFLECTION CAPTURES NEED TO BE REBUILT message in the viewport
1. In the top menu bar, navigate to **Build > Build Reflection Captures**.
2. Wait for the process to complete.

## Credits

- Sponza model authored by Frank Meinl at [Crytek](https://www.crytek.com/).
- Sponza model acquired from [McGuire Computer Graphics Archive](https://casual-effects.com/data/).
- Unreal Engine conversion carried out by [Kristijonas Jalnionis](https://github.com/radishface).
- HDRI acquired from [NoEmotion HDRs](http://noemotionhdrs.net/).
