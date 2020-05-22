4 | Importing Custom Vehicles

    A step-by-step guide on importing custom vehicles into your server

    Mentioned web pages:
        gta5-mods:  https://www.gta5-mods.com/
        OpenIV:     https://openiv.com/

    Prerequisites: 
        A stable internet connection
        Visual Studio Code (recommended)
        Visual C++ redistributable
        FiveM application
        OpenIV modding application
    
    Choosing a vehicle:

        When looking for a custom vehicle, you will want to ensure that the vehicle you are looking for
        is what you are looking for, an example of this is having an addon OR a replacement vehicle.

    What is the difference between and ADDON and a REPLACEMENT vehicle?
        
        An ADDON vehicle will be a completely new vehicle that has a unique value and spawn code.

        A REPLACEMENT vehicle will replace an existing GTA5 vehicle and keep the handling and spawn code of
        the vehicle that it replaces.

    I have downloaded the vehicle, but now I have a dlc.rpf file, what do I do with that?

        You will need to open this dlc.rpf file using OpenIV, which will then allow you to extract
        the data and stream files inside, these are what allow us to stream the vehicle into
        our FiveM server.
    
    Where do I put the data and stream files?

        Inside your resource to stream the vehicle, you will need a 'data' and 'stream' folder.
        You should place the data files into the data folder and the stream files into the stream folder.

    
    Common faults / errors:
        If you do not get any 'resource found' messages, and/or it says 'failed to start resource' , you did not type 'cd' into the starter.bat file
        If no resources get started, and you cannot connect, you did not add +exec into your starter.bat
        If you get 'no license key specified' , either of the above errors may apply

