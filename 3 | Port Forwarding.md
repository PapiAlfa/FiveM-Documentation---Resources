3 | Port forwarding Your FiveM Server

    A step-by-step guide on your FiveM server
    
    Setting a Static IP Address
        To be able to maintain your forwarded ports you will need to set a static IP address
        to your device so the device's IP will not change - This is set through your device 
        or your router.
    
    Finding your IPv4 address & Default Gateway:
        1) Open Command Prompt as Administrator
        2) Enter 'ipconfig' then enter
        3) Locate your IPv4 address & Default Gateway
        3) Note this down for future reference. 
      
    What is an IPv4 Address?
        An IPv4 address is an address assigned to every device on your local network to designate where external packets will be sent         to what device when received to your router. 

    What is a Default Gateway?
        A Default Gateway is the address assigned to central Router or Switch on your network. This is the device that sends and                receives all data for your network.
    
    Windows Method:
        1)Open up Network Settings. Settings > Network & Internet > Ethernet / Wireless Connection
        2)Open the Change Adapter options page
        3)Right click on your connection source and open properties
        4)Locate the IPv4 Connection, Select then open its properties
        5)Select ‘Use the following IP Address’
        6)Enter the following 3 boxed with the IPv4 Address, Subnet Mask and Default Gateway from Command Prompt earlier on.        
        
        [NOTE]: If you use custom DNS, these are fine to be entered below – If not do not worry it will work just fine still.
          
        7)Select OK to enter and save the settings. 
        8)Restart your device to ensure you keep the same IP Address, this can be tested by opening Command Prompt again and checking           with the Local IPv4 Address as earlier.
        
    Router Method:
        1)	Open a browser and enter your default gateway in the address bar and confirm.
        2)	When prompted to do so enter your administrator login and password.
            a.	This can be found on the back of the router or online here (https://portforward.com/router.htm)
                i.	Find the make and model of your router, then find the default login details.
        3)	Locate the device in the devices page.
        4)  Find the option to set an IP address.
        5)  Enter the devices IPv4 address from earlier and save to confirm the changes.


    Port Forwarding
        This act of 'forwarding' the ports allows data to be transmitted through these ports which are used for transmitting
        data online. It is like opening a door and allowing people to talk through.
        
        1)  Navigate to your default gateway from earlier and login using your details you found earlier.
        2)  Try to locate the port forwarding page on your router.
            a. If this does not exist head to your devices page and select your device you are hosting from.
            b. This may also be located in the advanced section.
        3)  Select 'Create new Port Forwarding Rule'.
        4)  Select your device or enter the IP of your device.
        
        Rule 1:
           1)  For rule 1, enter the start and end ports as 30120
           2)  Select TCP protocol and save.
       Rule 2:
           1) Follow the same beginning steps as rule 1
           2) Select UDP protocol instead and save.
           
       5) Save and confirm all changes and exit the panel
       6) Restart your device
       
    [NOTE]: If you have any problems and you cannot find your portforwarding page on your router, head to the following link and find your router - there will be direct steps of how to port forward for your specific router. (https://portforward.com/router.htm)
