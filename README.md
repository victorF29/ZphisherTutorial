# Zphisher Tutorial
<h2>What is Zphisher?</h2>
Zphisher is a phishing tool that runs on your host machine and can create clones of website login pages, which can then be sent to a target to try and take their login credentials. Zphisher can also create different fake websites that can entice the target to input their login credentials for other specific websites (i.e. a  website that promises free Instagram followers by just inputting your Instagram password and username, or a website that promises free PayPal cash using your PayPal login, etc.) This tool is very easy to use and customizable as well.
<hr>

<h2>Features:</h2>
<br><em>-List of 30+ popular websites to generate phishing attacks</em></br>
<br><em>-Auto Generated URL to send to target</em></br>
<br><em>-Open Source</em></br>
<br><em>-Customize the port the host computer runs the fake website</em></br>
<br><em>-CloudFlare Tunneling</em></br>
<br><em>-IP Grabber</em></br>
<br><em>-Various Login stealing templates that match their respective sites</em></br>
<br><em>-Written in BASH</em></br>
<hr>
<h2>Installing and Using Zphisher on Kali Linux</h2>
To install Zphisher on Kali you must first open up the terminal and run the <strong>git clone</strong> command.

<pre><strong>git clone --depth=1 https://github.com/htr-tech/zphisher.git</strong></pre>

Once zphisher is installed, cd into the newly created 'zphisher' directory.

![01](https://github.com/victorF29/ZphisherTutorial/assets/145622790/725ed56c-97df-4d8b-8edb-efd3926fe4b7)

Since the zphisher script is written in bash, we will have to run the script using the bash command.

<pre><strong>bash zphisher.sh</strong></pre>

![1](https://github.com/victorF29/ZphisherTutorial/assets/145622790/2ef894e4-041b-470c-9277-b663b8232c44)

Once the script is running select the website you would like to clone by inputting its corresponding number. In this example we will be cloning Instagrams login page.

![2](https://github.com/victorF29/ZphisherTutorial/assets/145622790/9926b080-8cd5-4cf0-8980-abde84038beb)

After you choose the site you would like to clone, a menu appears asking you what template you would like to use. You have many options from choosing to simply clone the website login page, to creating fake websites that promise targets with something they may want (in this case website templates for automatic followers, 1000 instants followers, and a blue badge verification.) These templates vary for each different site. In this example we will just be cloning the regular Instagram login page.

![3](https://github.com/victorF29/ZphisherTutorial/assets/145622790/b9f3bd95-fe04-4d26-93e0-23819e1c0fd3)

Next you can choose how you want to host the fake website. From what I have tested out LocalXpose does not seem to work so the only option are localhost and CloudFlare. If you want to test it out you can use localhost, but in this example we will be using CloudFlare. 

![4](https://github.com/victorF29/ZphisherTutorial/assets/145622790/1d974480-aaf4-4be8-a2c2-da5357eef4d1)

I recommend choosing a different port everytime you run the script. From what I've tested this will help to avoid getting detected by CloudFlare some times.

![5](https://github.com/victorF29/ZphisherTutorial/assets/145622790/a5e960b6-ed22-4307-ada8-c686ff0d8fad)

The next menu will ask if you want to use a custom URL but that has never worked when I test it. Just choose no when it asks you. After that it will give you a URL link to the fake website, copy that and paste in a seperate browser to see the credential harvester in action!

![6](https://github.com/victorF29/ZphisherTutorial/assets/145622790/f3fc7f5d-e7ab-4781-97dd-46d1cd34ae6f)

Once you have the URL pasted you will be met with the login screen of the fake website that you have just created. This is the website that will be used to harvest any information typed into it. 

![8](https://github.com/victorF29/ZphisherTutorial/assets/145622790/8d975c75-79b7-462c-ba68-1c2887800322)

After the target has put in their login and password, you can see it on your terminal along with the IP that they connected on! 

![9](https://github.com/victorF29/ZphisherTutorial/assets/145622790/cafebf9f-7bdc-4ef2-95c3-3d6b50c261ab)

Once you have finished you can exit out of the script and the login info and IP will be saved in their respective .txt documents in the zphisher directory! The URL zphisher provides doesn't look very trustworthy so one thing you can do to make the URL look less fishy is by using a URL converter like Grabify or Zamzar.
