# Webcrawler Project 5

## Approach
The general approach for this webcrawler is to keep track of all the visited pages in a list and a pseudo-queue (list) of pages to be visited. The program first logins and gets cookie information, then goes to the home page (http://webcrawler-site.ccs.neu.edu/fakebook/) and add any links it finds to the queue. I used the html.parser library to parse the HTML from the body of the HTTP responses. 

## Challenges and Testing
The most difficult part of the project was logging in and improving the performance. I ended up using developer tools in the browser to see how the post requests were structured since I was having difficulty getting the correct status. In additon, each run of the program was sometimes 10 min and I had trouble improving the performance beyond this. This also made testing difficult as I couldn't run as many times as I liked since the time it took to run once was a limiting factor. I still used print statements and tried to abstract functions to make sure my code was working as intended.