2 | Creating Your First Resource
    
    A step-by-step guide on creating your first custom resource for your FiveM server

    Creating a Resource Template
      A brilliant starting task is to make a resource template so you can quickly
      create resources in the future by following the template resource.
      
      NOTE: All resources MUST be located in the resources folder of your server directory.
      
      Creating a resource template:
        1) Enter your resources folder, and create a new folder called firstResource
        2) Enter the firstResource folder and create 2 subfolders called client and server
        3) Create a .lua file in the firstResource folder called fxmanifest.lua
        4) If your resource contains SERVER-SIDED scripts, create a server.lua file in the firstResource\server folder.
        5) If your resource contains CLIENT-SIDED scripts, create a client.lua file in the firstResource\server folder.
        6) Create a 'files' and 'stream' folder for any additional files that may be used.
        
      [NOTE]: You can (and should) follow steps 4, 5 and 6 for the template resource,
      as this will save you from having to create them for each resource,
      and they will not cause errors if you aren’t using them in a resource.

    What is an 'fxmanifest.lua' and why do I need it for EVERY resource?
      This file is the 'brain' of each resource, basically meaning that it defines
      that the specified folder is actually a resource. It will also define which
      files are server scripts and client scripts, along with other data files which are sometimes present.


    Here is an example 'fxmanifest.lua':
    #################################################################

    fx_version 'adamant'

    game "gta5"

    description "This is a template resource"

    client_scripts {
      "client/*.lua"
    }

    server_scripts {
      "server/*.lua"
    }

    files{
      "files/*.meta"
    }

    data_file "*Example Data*" "files/*.meta"

    #################################################################
    EDIT THE '*.lua' IN EACH SET OF "SPEECH MARKS" TO YOUR FILE NAME

    If you copy this template above ^ REMEMBER to remove the text in each set of "speech marks" to avoid errors,
    ONLY type in the speech marks if you are defining a file as a resource script.

    The FX_Version 'adamant' means that the version of the resource is resolute and unchanging,
    this is a new resource manifest format that is compatible with new cfx and FiveM updates.

    You may have seen '__resource.lua' files before, but these are deprecated and you should convert
    the __resource.lua to an fxmanifest.lua to avoid incompatibility in the future.


    Common faults / errors:
      If your resource is not found or cannot start, you may have an error in the 'fxmanifest.lua'
      ensure that you have no text in the fxmanifest that should not be there and that you have a LUA file not a TEXT file.
      
      If the console outputs a files and line, such as 'firstResource/client/client.lua:43' [ERROR MESSAGE]
      you should refer to this line in the specified file and follow the error message's syntax report.
