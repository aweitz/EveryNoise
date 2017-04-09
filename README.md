# Every Noise at Once - Artist Query

In early 2016, I came across the the website [Every Noise at Once](http://everynoise.com/engenremap.html). In the creator's own words, it is "an ongoing attempt at an algorithmically-generated, readability-adjusted scatter-plot of the musical genre-space, based on data tracked and analyzed for 1523 genres by Spotify."

As a music lover, it was both dizzying and exciting to browse the never-ending canvas of niche genres. It was also fun to discover that many of the artists I listened to were being tagged under obscure genres I had never heard of before: things like "indie fuzzpop" and "stomp and holler." I quickly wanted to look up my favorite artists and find all the strange genre names they were categorized under. Unfortunately, the website's interface does not permit this.

The scripts provided here cirumvent that issue by scrapping each genre page on the Every Noise site and reformatting the data to make browsing by artist more user-friendly. Admittedly, the result is a bit inelegant, relying on individual HTML pages rather than a database. There is also no way to directly search for an arist. They must first be found by going to one of the artist's more obvious genres. It would be fun to add these features in the future.

The resulting HTML can be found [here](https://web.stanford.edu/~aweitz/EveryNoise/). My hope is that others can use the scrapped data for similar interesting projects.

### Use
1. `scrapGenres.ipynb` saves a dictionary listing all artists for each genre.
2. `makeArtistList.ipynb` cycles through each genre and saves a dictionary listing all genres for each artist.
3. `writeHTML.ipynb` writes the HTML pages for browsing.

### Dependencies
The specific HTML files written by this code assume you have the following tools added to your HTML directory. Versions can be easily updated within `writeHTML.ipynb`.

* [Font Awesome](https://github.com/FortAwesome/Font-Awesome/)
* [jQuery](https://jquery.com/download/)
