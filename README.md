# webmapping
web mapping final
Jared Dobkin
Final Web Mapping 
	This project is a current position locator in reference to my job, Share Food Program, and also shows the position on a map of the schools I serve. 
	The initial tile layer for the map is an L.tileLayer function showing the Dark All basemap from open street maps.org this is a pretty basic function so I won’t get into the meat of it. I like the dark layer base map a lot more though hand it gives the impression that your data is important or secret, and I really like that. 
	The points for the schools I serve are contained in the header as nepSitesInOrder.js are not referenced in an L.geoJson point to layer function. 
 
I then use a an on each featue event caller to change the color and display a name when the item is clicked on.  
This will display the name of the facility that I serve, and make that name go away and change the color after you put the mouse over the marker and pull it away. I used a circle marker because it showed up better than a regular marker. This also uses a varible popup and the layer.bindPopup function to populate the popups wit hthe name of the facility.
	This procress is then repeated for the other geoJSON files refered at the header. These files are schools.js which is every school in Philadelphia sans the ones we serve and fMarket.js which is farmers market locations. 
	After all the elements are created a function to get the user coordinates is implemented. This is the navigator.geolocation.getCurrentPosition function. This is a part of native javascript and api for it can be found on mozilla’s website. 
 
This returns the user’s coordinates as postion.coords.latitude and .longitude. We then calculate the distance using the Math model to Share (40.016501, -75.1437876, and convert it to miles. This then triggers an alert that tells you how far you are from the Share Food Program. For reference I commented out all the possible attributes of the getCurrentPosition function.
	I tried to play with the idea of real time data being implemented into my map and have included the code that did not function under fuction createRealtimeLayer. Also included is a link the .js file that has the added user generated module and to real time data of the wander drone. 
 
Reflection
	This class was ¬¬a great opportunity to learn a marketable and very satisfying skill for my GIS career. Web mapping is one of the most relatable and easiest to explain GIS functions, and it was really awesome to be able for once to explain to my folks what I was working on and watch them actually have a grasp on it. 
	A real struggle for me was switching between the logic of javascript and css and html all in one document. Sometimes I even confused it with python scripting and tried to add python elements into the java document. After kind of catching on to where the CSS and where the HTML and where the Java go it was a lot easier to get into the flow of scripting in this way. It seems like that kind of transition could be difficult in harder applications of webmapping. 
	Another struggle for me in this class was getting used to calling functions after I write them. The arguments and parameters seem easier to distinguish logically but can be really tricky in application in a document. I had to fight the urge to hard code more and more things because it wouldn’t have taught me very much about calling and using functions.
	The last thing I struggled with is working on aesthetics of my websites. As a not very aesthetically motivated person I found it challenging to figure out what would look good on the web and really make my site pop and stand out. This is definitely something I would need to work on in the future not only in this application but across the board.
	My real ahaaa moment came when I began to fall into the flow of references different Leaftlet functions and how to really pour into the API. The biggest transition was from mostly checking stackoverflow to going to the leaflet API and only using the stack if I really couldn’t figure it out the first time.
	This was a challenging course be defiantly gave me a firm footing into web design and digital mapping. I don’t see myself becoming much of a web designer but it would be a very appealing way to display data in the future and I look forward to implementing it. Furthermore if more projected were webhosted that data would be open to the public more and allow for less institutional exclusivity. If we really want to provide good data for everyone webmapping is the future of that. 

