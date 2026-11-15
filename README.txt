THE CANADIAN RECORD — WEBSITE STARTER

FILES
- index.html: the website.
- episodes.json: the episode list with 30 empty slots.
- covers/: put your episode cover images here (optional).

ADDING AN EPISODE
Open episodes.json in a text editor. Each of the 30 entries looks like this:

{
  "showing": false,
  "name": "",
  "description": "",
  "cover": "",
  "video": ""
}

Fill it in, for example:

{
  "showing": true,
  "name": "Why Canada Entered World War II",
  "description": "Why Canada made its own decision to enter the war in 1939, and how Canadians contributed.",
  "cover": "covers/episode-001.jpg",
  "video": "https://www.youtube.com/watch?v=YOUR_VIDEO_ID"
}

IMPORTANT
- showing: true makes the episode appear. false keeps it hidden.
- name: the episode title.
- description: a short description shown below the title.
- cover: a path to an image in the covers folder, or a full image URL.
- video: the YouTube video URL. The site currently shows a Watch episode link.

Keep the JSON commas and quotation marks. Do not add comments inside episodes.json.

PREVIEWING
Because the site loads episodes.json separately, don't just double-click index.html.
Run a local web server from this folder. If you have Python installed, open a terminal in
this folder and run:

  python -m http.server 8000

Then visit:

  http://localhost:8000

PUBLISHING
Upload index.html, episodes.json, and the covers folder together to the same website hosting
location. Any hosting service that supports static HTML files will work.

DESIGN NOTES
The site uses a restrained editorial look: warm paper background, dark ink, muted red accents,
serif headlines, simple navigation, and grayscale cover photos. Replace the hero image URL in
index.html if you want a different banner image.
