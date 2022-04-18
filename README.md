# Laser System - front page and docs

Welcome to the home page of the Laser System asset for Unity. 

## About the project

The project is a complete and ready to use laser system that includes

 - **Logic** that handles finding the _laser actors_ and firing the events to help you write your game
 - **Drawing** out the laser beams and particle effects for eye candy
   - Shaders, textures
   - Textured models with changeable **Primary**, **Secondary**, **Paint** and **Dirt** colors to match your game's style
 - **.blend** files to enable you to change anything to your liking, should you prefer to
 - **Prefabs** to speed up work
 - **Automated tests** to verify the functionality of the project and the integrity of the prefabs
 - **Complete, detailed documentation** to help you understand what's going on or if you just want to learn how a system like this is done
 - **Scripting reference** for easy navigation inside the comments

While the project itself contains the in-depth documentation as part of the package the quickstart with the scripting reference is available on this repository. 

## Who is this project for

Anyone who wants to develop games in Unity that require a complete laser system (kinds that remind you of hit games like Portal 2). As an example, if you intend to create a laser-based puzzle game then the asset is an ideal choice for you.

Keeping in mind that one size might not fit all, the system is designed so that the logic for *drawing* the beams / particles is completely decoupled from the logic of the *lasers*. So much so in fact that all these are present as separate scripts that are attached to the prefabs inside the project. 

If you're just interested in learning how a system like this is implemented then the project itself and its documentation will prove very useful to you. Note that basic programming concepts and C# language constructs are not detailed inside the docs, however, links are included for the documentation. 

## About the docs

The latex reference is exported as a _pdf_ file. 

The detailed documentation is exported as a _pdf_ file as well. 

See the html docs starting from the _index.html_ file after downloading the _html-reference_ folder.

## Setting up the project

You can improve the performance of the raycasts by adding which layers the emitters should take into account. If left empty, all layers will be included in the raycasting process. 

All the included textures are 4K or 8K in the case of some more detailed normal maps, except particle textures where this would not make sense. This is to make sure the assets look correct in the case of close up shots, should you need those. Compress the textures into a lower resolution of you encounter performance problems on your particular platform. 

To run the Play Mode automated tests you do not need to add the demo scenes to your build settings. The test assembly should be detected by Unity Test upon finishing import and all the tests should pass. If one or two tests fail, please run them again - there might have been some issues with the timings inside the tests due to varying frame rates, inspite of all the tests being constraned to a certain frame rate. 
