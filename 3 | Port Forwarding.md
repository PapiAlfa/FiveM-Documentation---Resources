3 | Portforwarding Your FiveM Server

    A step-by-step guide on your FiveM server
    
    Setting a Static IP Address
        To be able to maitain your forwarded ports you will need to set a static IP address
        to your device so the device's IP will not change - This is set through your device 
        or your router.
    
    Finding your IPv4 address & Default Gateway:
        1) Open Command Prompt as Administator
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
        

