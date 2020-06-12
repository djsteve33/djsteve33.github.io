---
layout: post
title:      "Web Scraping vs Using API"
date:       2020-06-12 22:31:49 +0000
permalink:  web_scraping_vs_using_api
---


I recently completed my first project at Flatiron School, a coding bootcamp. The project involved creating a CLI, a Command Line Interface in Ruby, the programming language that we're learning first. It was quite a learning experience for me.

I had to first set up my coding environment. I did that using GitHub. GitHub is a website that allows you to create, store, and share a repository that you write your code in.

After I got the coding environment set up, I had to next create the folder/file structure. Then, after getting the files & folders in place, it was time to start coding. For someone new to coding, it took some doing getting the code to work the way I had envisioned for my program. 

Prior to starting the project, though, we received training on the 2 main methods to extract data online. The first method is called web scraping. The second is method is called API. 

Web scraping does have some advantages, such as: 1) up-to-date data, 2) no rate limitations on data, 3) customization and well structured data, and 4) you can remain anonymous.

API, which stands for Apllication Programming Interface, allows software to talk to other software. API does have some limitations, such as: 1) availability and lack of customization, 2) rate limits, and 3) legality. 

In spite of the limitations, there are some advantages of using API. If you need to get the same data, from the same source, for the same specific objective, then API would perfectly fit all your data needs. Also, the person might have a contract with the website. This is often in the form of an API Key.

For our projects, we used API. For my project, I had to obtain an API Key, which I kept separate from the main url. Here is a code snippet from my project:

BASE_URL = 'http://developer.itsmarta.com/RealtimeTrain/RestServiceNextTrain/GetRealtimeArrivals?apikey='
KEY = ENV['API_KEY']

I had to register for the API Key. So, it was unique to me. Therefore, to protect it from being used improperly, I hid it in a private file that wasn't shared on GitHub.

I then had to write my code to basically concatenate the base URL and the API Key together. 

In the end, my program worked as intended. I look forward to learning  more about and utilizing both web scraping and API in future programming endeavors.

