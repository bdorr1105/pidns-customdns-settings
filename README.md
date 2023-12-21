# pidns-customdns-settings
The settings.php file modified to allow for up to 8 custom DNS servers. This probably overkill for most people, but if you want more than just two options for a real custom setup, then this will help. I don't know how often this is going to be updated as I won't have a need to do it often. This is really custom to my environment anyway. This is from version 5.17.12


![Custom DNS](https://github.com/bdorr1105/pidns-customdns-settings/assets/12386911/570a7900-f0ad-40ff-ba93-f9385eafd44d)


## How to Use This
You can view the changes you have to make which are towards the top of the script and then in the DNS section about midway down and modify your files on box. It would be wise to make a backup before implementing any of these changes. If you opt to not edit the local files on box, still make a backup so you have the original. Then you will paste these in the perspective directories. You can also git clone the repo or download direct. Whatever you prefer.

### Clone this repository to your local machine:
`git clone https://github.com/bdorr1105/pidns-customdns-settings.git`

|:exclamation:  Warning   You should make a backup of each file so if anything goes wrong you can fall back to the default configuration that is a known good. Modify at your own risk!|
|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|

## Paste the settings.php in
 ```/var/www/html/admin/settings.php```

## Paste the savedsettings.php in 
```/var/www/html/admin/scripts/pi-hole/php/savesettings.php```

## Validate it saved your custom upstream DNS servers by checking the setupVars.conf
```cat /etc/pihole/setupVars.conf```

## Here is a sneak peak of the first octet of my internal DNS, go wild lol!

![setupVars-conf](https://github.com/bdorr1105/pidns-customdns-settings/assets/12386911/5284ff36-0e24-4872-811a-0597c7b0a9fb)

## Contributions
Contributions to this project are welcome. If you find any issues or have suggestions for improvements, please feel free to create a pull request or submit an issue on the GitHub repository.

### The pihole Project is a great one and you should consider donating if you have the funds. 
https://pi-hole.net/

![Vortex-R](https://github.com/bdorr1105/pidns-customdns-settings/assets/12386911/1953a22d-c08d-4709-a70b-f45e5c928e24)
