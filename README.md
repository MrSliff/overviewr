# overviewr
An advanced Servarr utility to list open requests from Overseerr and missing Movies and TV shows from Radarr and Sonarr.

## Problem
Running a full stack of Servarr stuff, the request system in overseerr got a bit full and messy and i am constantly running behind. I want to reduce the workload by listing all missing requests (with an optional filter for the age, release state and so on) on one page. It should also automatically fetch download sources from *arr and list them together with the media, so you can just get a file with one click - Some times sources are rejected by filters or settings, and to go through every single media is much work. I want to also implement some custom script to make requests on my private trackers over the Pythons Http requests library, for example: If there are no sources available, a text input is displayed to provide metadata which is mandatory for a request on my tracker. With the text filled, you can just do a request on the tracker of your choice (need to reverse engineer the get and post requests sent to the tracker in the browser).

Everything should be easily accessible through a web frontend.
