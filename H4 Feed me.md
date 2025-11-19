# x) Why would you want to use a feed reader (and RSS/Atom)? Couldn't you just browse to each website?
  - Instead of visiting each website separately, a feed reader gathers new posts from all of your favorite websites in one location. You save time and effort by receiving a single stream of new content rather than having to monitor several websites for changes. Feed readers make sure you don't miss any significant postings or announcements by automatically retrieving updates as soon as they are released. RSS/Atom feeds remove clutter, pop-ups, and advertisements so you can concentrate on the content. In contrast to manually perusing websites, several feed readers allow you to download items for offline reading and arrange feeds by topic, priority, or tags. 

- In short, a feed reader makes the process faster, cleaner, and more reliable rather than browsing each website.



a) Install a feed reader. Show that it can read a feed (RSS or Atom). Include a screenshot of this. You can use any feed reader you like, and you can install the feed reader in your host OS if you like.
 - I installed Thunderbird with the commnad - sudo apt-get -y install thunderbird
   <img width="839" height="568" alt="Screenshot From 2025-11-19 12-21-14" src="https://github.com/user-attachments/assets/118a92d7-a727-41ff-bb41-d9a56b227c6f" />


b) Add the feed for Krebs. This is the one we discussed in the class. https://krebsonsecurity.com/feed/
 - I added the feed for Krebs with the option "show the article summary instead of loading the webpage"
   <img width="1268" height="665" alt="Screenshot From 2025-11-19 12-47-52" src="https://github.com/user-attachments/assets/ac8fe314-8e5b-4f28-8e03-f2a21fc9d92f" />


c) Add a feed for Schneier on Security. Find the blog, and locate the feed.
  - Added the blog https://www.schneier.com/feed according to the instructions.
    <img width="1268" height="665" alt="Screenshot From 2025-11-19 12-31-00" src="https://github.com/user-attachments/assets/3ddc5f71-dade-44d4-a940-684ba8ede844" />

    
d) Find and add two more security related feeds. Explain how you found them, and why you chose them.
  - I googled and found this webiste https://rss.feedspot.com/cyber_security_rss_feeds/ , that lists Top 100 Cyber Security RSS Feeds (Security RSS) from where i chose https://thehackernews.com/ and https://www.darkreading.com/ because i am familiar with websites.
  
e) Follow security feeds for a while. What did you learn? What are the benefits and downsides of following feeds with a reader, compared to some other methods of following cyber security scene?
 - Following all the feeds i learned that it is so fast and precise to read and learn about the topics or the website i chose. Mostly i browse websites directly which is time consuming, feeds help me to identify the required information from the websites.
 <img width="1268" height="665" alt="Screenshot From 2025-11-19 12-40-21" src="https://github.com/user-attachments/assets/6b0641c2-af9a-464b-8b4f-3325030479e0" />

f) Port scan. How can criminals know what services your employer has? Disconnect your computer from the internet while doing the test (after you have installed the required software). Do the test inside your virtual machine.
 - Installed the nmap port scanner in the VM,after disconneting from the internet i tied to ping 8.8.8.8 which was unsuccessful.
   <img width="887" height="280" alt="Screenshot From 2025-11-19 13-57-44" src="https://github.com/user-attachments/assets/cb44da9d-d78d-4aac-a140-46e72c7f8c98" />
 - I scanned the port of my local machine with the commnad - sudo nmap -A -v localhost and got result as in screenshot
   <img width="588" height="685" alt="Screenshot From 2025-11-19 14-06-04" src="https://github.com/user-attachments/assets/3a72b21e-48f5-42f2-b3c8-c15cc7a608b3" />
 - And i installed a daemon, apache2 and again scan the port, i got the result as in screenshot
   <img width="588" height="715" alt="Screenshot From 2025-11-19 14-12-09" src="https://github.com/user-attachments/assets/ab168f05-d1ff-4e79-80f8-8655b1dbbc22" />
 - After analysing both results,
     - I found the purpose of the port scan is to performs an aggressive scan with verbose output, including OS detection, version detection, script scanning, and         traceroute and the target was localhost (127.0.0.1) which means the scan was run against the same machine.
     - Before installing apache 2, only one port 631/tcp was open but after the installation port 80/tcp was also open, other were closed.
     - The default Apache page is running, Linux kernel versions 5.4 to 6.2 is the OS detected, Network Distance: 0 hops confirms the scan was local.
