Simulator Usage
=====

Initialization 
------------
Need to initalize settings as follows. Can choose between BLENDER_EEVEE and CYCLES and change image resolution as needed.

.. code-block:: python

    WorldGen.set_render_engine('BLENDER_EEVEE')
    WorldGen.set_metadata_properties()
    WorldGen.set_image_resolution(1084, 1084, 100)
    
    
Setting up the simulator
------------

To use WorldGen, first initialize by passing in the file path to the blend file, followed by coordinates to the scene in following format (minLon, minLat, maxLon, maxLat).

.. code-block:: python

   simulator = WorldGen("./city.blend")
   simulation.createScene(-122.4, 37.7865, -122.387, 37.7925)
   
If the scene is rural or suburbs then set isSuburbs to true for slanted roofs:

.. code-block:: python

   simulation.createScene(-122.4, 37.7865, -122.387, 37.7925, isSuburbs=True)
   
Adding textures/materials
------------

WorldGen uses LilySurface Scrapper (https://github.com/eliemichel/LilySurfaceScraper) for importing materials for the building, roads, and terrain. If you wish to use materials other than the default ones used, you can select them from 

- https://www.3dassets.one/#order=latest
- https://polyhaven.com/textures
- https://www.cgbookcase.com/textures/
- https://ambientcg.com/





