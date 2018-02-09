## IBM-WATSON-ANALYTICS CONNECTION WITH MYSQL SERVER

#### Introduction : 
So long story short, if you are one of those people who have been trying to connect there local - on premise database to IBM Watson and have been unable to connect to it then this one is to help you out.
It took me ages to figure out how to really make this connection with bluemix/mysql/database. It took me a while to figure it out myself as there wasn't any particular document specified for this connection.
The below steps should enable you to connect between IBM watson and your local on premise Database. 

Note : I have use MySQL to connect to IBM but this method should work fine for any database or cloud platform. 

#### Step 1 : Go to account settings > Secure gateway connection > which would open a page like below 

![screen shot 2018-02-09 at 4 50 04 pm](https://user-images.githubusercontent.com/30907520/36053903-567d44b4-0db9-11e8-8546-7f94d2ee496a.png)

#### Step 2 : Click on create client connection (+ Connect Client ) > Opens below page > Download sofware Installer as per OS

![screen shot 2018-02-09 at 4 54 13 pm](https://user-images.githubusercontent.com/30907520/36054187-9d0ae214-0dba-11e8-84e2-38851a305f4c.png)

Note : COPY AND PASTE YOUR GATEWAY AND SECURTIY TOKEN 

#### Step 3 : INSTALL THE DOWNLOADED FILE ON YOUR SYSTEM

#### Step 4 : Search secgw.command file and open in terminal 

<img width="583" alt="screen shot 2018-02-09 at 5 04 32 pm" src="https://user-images.githubusercontent.com/30907520/36054323-55e25d12-0dbb-11e8-89b1-ed3af3a2a0da.png">

Enter information : 
Enter the gateway IDs, separated by spaces: Gateway information that you copied previously 
Enter the gateway ID security tokens separated by spaces, enter 'none' for no security token: Enter Token as copied previously 

This will open installation and install bluemix something like below : 

<img width="865" alt="screen shot 2018-02-09 at 5 08 38 pm" src="https://user-images.githubusercontent.com/30907520/36054538-abc42764-0dbc-11e8-8a68-f92d1d8718db.png">

#### Step 5 : Visit localhost:9003/dashboard to view the UI or as in ur installation comments to acces UI 

![screen shot 2018-02-09 at 5 16 47 pm](https://user-images.githubusercontent.com/30907520/36054637-24800240-0dbd-11e8-9cea-33ece634d54d.png)

#### Step 6 : Go to Access Control List > To Add your connection host IP and Port info

![screen shot 2018-02-09 at 5 18 54 pm](https://user-images.githubusercontent.com/30907520/36054673-551a746c-0dbd-11e8-8a12-da1221446bd2.png)

Note : 1) So essentially you need to create a client connection with IBM Watsome using a secure gateway once that is done add your database connection on access control list. 
       2) Go back to your terminal where you installed client and type ' show acl ' 
       3) This will show you the newly provided host and port. 

### AWESOME !!! YOUR SET TO CONNECT YOUR ON PREMISE DATABASE NOW !!!

#### Step 7 : Go to Data Connection > (+) Button 

![screen shot 2018-02-09 at 5 27 34 pm](https://user-images.githubusercontent.com/30907520/36054903-8cbe570c-0dbe-11e8-8255-543d003cb731.png)

#### Step 8 : Select connection which is on premise

![screen shot 2018-02-09 at 5 28 23 pm](https://user-images.githubusercontent.com/30907520/36054925-a7c4d2d8-0dbe-11e8-86e1-befdb2b12a72.png)

#### Step 9 : Add your connection info > Click Create 

![screen shot 2018-02-09 at 5 30 21 pm](https://user-images.githubusercontent.com/30907520/36054993-fcf6d530-0dbe-11e8-967c-01496406bfb7.png)

#### Step 10 : You have Created your succesful connection to IBM WATSON !! ENJOY !! 

![screen shot 2018-02-09 at 5 32 01 pm](https://user-images.githubusercontent.com/30907520/36055015-2a7f1a76-0dbf-11e8-819c-2389209c4a70.png)

Note : the above is a screenshot of my test connection not of the one show in step 9

#### Step 11 : Test connection and check database tables : 

![screen shot 2018-02-09 at 5 33 48 pm](https://user-images.githubusercontent.com/30907520/36055073-7cabb46c-0dbf-11e8-94d5-4fef3b14be0e.png)

#### Step 12 : See if you can see your Database and Tables : 

![screen shot 2018-02-09 at 5 35 06 pm](https://user-images.githubusercontent.com/30907520/36055098-a9341f42-0dbf-11e8-8a06-54ef984ed33e.png)

Please write of comment if you have any new issues !! Good Luck !! 
