# Why Fi?!
I don’t always blog but when I do, dyslexic. 

Recently, I saw a link posted on Facebook talking about a phone app that can brute force your WiFi router. The app attempts to connect to a protected router, then tries ten thousand of the most commonly used passwords one by one. Now I can see a lot of people trying this app on their own “home” router. However, I can tell you that this app will have a low success rate, based on the built-in password list. The article reminded me of a project that I did back in 2015, when I was wondering if I could easily guess the WiFi password. At the time, I quickly came to the conclusion that using most commonly or crunched password lists for brute forcing WiFi is not a viable option. If I wanted to guess the password, I needed to understand how people create base passwords for their WiFi devices. 

Just a simple test to brute force my own router with 10 random passwords showed that it took me about 3 minutes - that’s 15 to 20 seconds per password. Now let’s assume that it takes 15 seconds per password, that’s 15 * 10.000 passwords = 41.6 hours. You can imagine why this is time consuming and not worth your time trying with a list of the most commonly used passwords. If you have network-manager installed on your linux machine then you can try the test yourself by typing the following into your command line

`for i in $(cat password.txt);do nmcli device wifi connect <SSID> password $i;done`

In my search for a list I’ve found a Russian company that has built a crowdsourced app for mobile phones to make the internet more accessible. They did this by mapping over 100 million private and public WiFi access points worldwide and included comments and passwords from the social community. The data showed that in most cases, I did not need to guess the password. The app’s community actually provided the correct password for all the places I’ve used the hotspot, including a history of some access points that date back 3 years with password changes. 

To comprise with the dataset acquired from the Russian company, the original password list that came with the brute force app,  I’ve looked at Istanbul, Iraq and New York and noticed that non latin alphabet rather use numbers for their choice of password. But numbers will also be password of choice for IoT devices for consumers. But overall if you want to have a good password list to brute force you’ve to look for patterns for the specific area where the WiFi device is in.

Base words regional
Commonly used	| Turkey Istanbul	| Iraq Baghdad	| USA New York
blue			| istanbul		| ahmed 			| marion
test				| current 			| aliali 			| password
love				| toplanzi.com	| admin			| guest
pussy			| galatasaray		| aaaa			| netgear
qwerty			| required		| mustafa		| welcome
letmein			| fenerbahce		| aaaaaaaa		| hello
fuck				| ahmet 			| current			| freewifi
soccer 			| murat			| required		| angelina
mustang 		| mehmet		| alialiali			| newyork
bubba			| mustafa		| peshmarga		| abcd

Top passwords
Commonly used	| Turkey Istanbul	| Iraq Baghdad	| USA New York
password		| 12345678		| 12345678		| Marion426
123456			| 123456789		| 123456789		| 12345678
12345678		| 1234567890	| 1122334455	| 123456
1234			| 12345			| 11223344		| 123456789
qwerty			| 123456			| 1234512345	| 12345
12345			| toplanzi.com 	| 12341234		| 1234567890
dragon			| current 			| 1234567890	| password
pussy			| required		| 20152015		| marion426
baseball			| 1234567		| 1234554321	| 1234567
football			| 1122334455	| 11111111		| 1234

Password length
Commonly used	| Turkey Istanbul	| Iraq Baghdad	| USA New York
6 = 35.48%		| 8 = 23.28%		| 8 = 42.33%		| 8 = 23.94%
7 = 20.53%		| 10 = 17.67%	| 10 = 14.14%	| 10 = 14.54%
8 = 19.31%		| 9 = 15.78%		| 9 = 14.04%		| 9 = 14.28%
5 = 11.73%		| 11 = 8.93%		| 11 = 7.44%		| 6 = 10.97%
4 = 11.4%		| 12 = 7.13%		| 12 = 5.54%		| 7 = 5.84%
9 = 1.04%		| 13 = 5.26%		| 6 = 3.38%		| 5 = 5.78%
10 = 0.3%		| 6 = 4.57%		| 5 = 3.11%		| 11 = 5.69%
11 = 0.11%		| 7 = 3.79%		| 7 = 2.68%		| 12 = 4.6%
12 = 0.07%		| 5 = 3.61%		| 13 = 2.03%		| 13 = 4.46%
13 = 0.02%		| 14 = 3.07%		| 14 = 1.5%		| 16 = 2.91%
