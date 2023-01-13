Simulator Usage
=====

Initialization 
------------
Need to initalize settings as follows. Can choose between BLENDER_EEVEE and CYCLES and change image resolution as needed.

.. code-block:: python

    set_render_engine('BLENDER_EEVEE')
    set_metadata_properties()
    set_image_resolution(1084, 1084, 100)
    
    
Setting up the simulator
------------

To use WorldGen, first initialize by passing in the file path to the blend file, followed by coordinates to the scene in following format (minLon, minLat, maxLon, maxLat).

.. code-block:: python

   simulator = WorldGen("./test.blend")
   simulation.createScene(-122.4, 37.7865, -122.387, 37.7925)




