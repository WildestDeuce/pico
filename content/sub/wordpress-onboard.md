# Onboarding for Wordpress

### Download Mamp

![mampdl](/assets/src/mamp-dl-screen.png)


This is what your screen will look like when you download MAMP. 
Click the top left box under the Apple Icon for an OS download, if you're using windows click the top right box with the windows. 

You will only need MAMP as MAMP Pro is subscription tier, costs money and isn't neccessary to run wordpress locally on your machine. 

The download will appear at the bottom of your browser select it once the download is complete. 

### MAMP Settings

First, open MAMP.
Then press cmd, (command + comma) on Mac to open preferences.
In the MAMP window select the Ports tab across the top. Make your port settings like the picture below. 

![mampsettings](/assets/src/mamp-server-settings.png)

Make sure your web server tab is set to Apache. Like this 

![mampapache](/assets/src/mamp-apache-settings.png)

While we are on this screen you also need root folder for MAMP to read your Wordpress projects from. Your apache server will access this folder as the localhost of your machine. I named mine development, feel free to do the same with yours. 

### Setting the Local Directory

Open your finder to see a screen that looks similar to this

![finderscreen](/assets/src/finder-screen.png)

If it doesn't, press cmd shift H (command + shift +H)

Click and drag the house next to "charlesopia" to the left sidebar's favorite section. This will make finding your home folder much easier in the future.

From your home folder crete a folder that you will use for your Apache server in MAMP. Again my folder is called "development".

Go back to MAMP, here 

![mampapache](/assets/src/mamp-apache-settings.png)

Next to Document Root click Select and select your home folder and then your "development" folder or whatever you chose to name yours. 

Now click OK. You will see this screen

![mamphome](/assets/src/mamp-home.png)

Stop your servers with the "Stop Servers" button. Then restart by clicking the same button again. 

In your browser go to localhost/ (a second window for MAMP will open but that isn't needed at this time)

All directories inside the development directory will be listed as hyperlinks.

![localhostscreen](/assets/src/localhost-screen.png)

Once you add directories to the development folder they will show up here. For now I'm going to click in to my wordpress directory. 

Doing so gives me this screen

![wordpress-setup1](/assets/src/wordpress-setup1.png)

Select your language and click Continue.

The information entered on the next screen is used to set up the database for your wordpress website

![worpress-setup2](/assets/src/wordpress-setup2.png)

Ok, let's stop here and setup the database first to make sure things run as smooth as possible. 

In your browser got to localhost/phpmyadmin. This will take you to your Apache server's MySQL databse where we can configure everything needed ahead of time. 

![phpmyadmin](/assets/src/phpmyadmin-screen.png)

From here click New in your left sidebar.

Make a database name (I used the name wordpress_test for mine). Click create.

Go back to your other wordpress tab in your browser and click Let's Go to continue. 

![database-setup-screen](/assets/src/database-setup-screen.png)

If you forget what you type into these fields to setup your database you can always check the wp_config.php file that gets created after this screen. 

Default settings should be "root" for Username and "root" for password. 

Database host means to find the website on wordpress_test database you would enter localhost/wordpress_test into your browser.

Don't change your table prefix. Go ahead and click Submit.

![finished-setup](/assets/src/installation-complete.png)

When you see this screen you are almost finished.

![website-setup](/assets/src/website-setup.png)

Fill in the required forms and click Install Wordpress.