### NZ SPCA Wellington Scraper

I was having issues with how to go about scraping the SPCA Wellington site and talked with <a href="https://github.com/marcus-crane">Marcus</a> who is a lot more knowledgeable than myself in these things.

The SPCA site uses lazy loading so obtaining all the data at once proved to be more challenging than we thought.

Once you scroll to the bottom of the page it makes a XMLHttpRequest to fetch more data, so we used Postman to back-trace the browser's cookie and a JSON object which returned all the requested, current animals!

He took me through roughly how he thought it should be done and I then attempted my own version, which is included in another project
https://github.com/cam-shotter/react-personal-project

The next step was to parse the data and feed it into a database so I could use it for my app.
