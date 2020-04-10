1 | Setting up a FiveM server in 2020

    The official guide to setting up a FiveM server: http://docs.fivem.net/server-manual/setting-up-a-server/

    Mentioned web pages:
        Server Artifacts: https://runtime.fivem.net/artifacts/fivem/build_server_windows/master/
        CFX-server-data repo: https://github.com/citizenfx/cfx-server-data
        Server.cfg template: https://docs.fivem.net/docs/server-manual/setting-up-a-server/#server-cfg
        FiveM Keymaster: https://keymaster.fivem.net/
        Visual C++ Redistributable: https://support.microsoft.com/en-gb/help/2977003/the-latest-supported-visual-c-downloads

    Prerequisites: 
        A stable internet connection
        Visual Studio Code (recommended)
        Visual C++ redistributable
        FiveM application
    
    Installation / Set-up:

        1) Visit the Server Artifacts web page and download the latest 'server.zip' package
        2) Create a new folder in your desired directory that will store your FiveM server, call this folder 'server'
        3) Move the aforementioned 'server.zip' package into the server folder
        4) Extract the zipped server.zip file in this folder, you can now remove the 'server.zip' file
        5) Visit the 'cfx-server-data repo' and download the package
        6) Move the 'cfx-server-data.zip' file into the server folder and extract it like before, you can also now delete the .zip file
        7) Visit the official FiveM documentation page and copy the 'server.cfg' file
        8) Create the server.cfg file in the 'cfx-server-data' folder and paste the contents copied from the previous step into this file
        9) Visit the FiveM Keymaster web page and login/create an account, then create a new key with the valid information   

       10) Open the 'server.cfg' file in a text editor and edit the default values to the specified values for your server
           this includes the sv_licenseKey which can be obtained after registering your server on the FiveM Key master web page

       11) Creating a launcher file for the server:
                Create a 'starter.bat' file in your server folder, then open in with a text editor
                Copy the following template and change it to your directories for your server:

                    cd /d C:\testServer\server\cfx-server-data
                    C:\testServer\server\FXServer.exe +exec server.cfg

                (If your server was located on your desktop, then all you should need to change is the username in the directory)
                (Though this may not be the case for you, so we recommend checking the full directory name for differences)

       12) Launch the server by exceuting the starter.bat file we just created

    
    Common faults / errors:
        If you do not get any 'resource found' messages, and/or it says 'failed to start resource' , you did not type 'cd' into the starter.bat file
        If no resources get started, and you cannot connect, you did not add +exec into your starter.bat
        If you get 'no license key specified' , either of the above errors may apply

