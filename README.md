# CompareShows
comparing movies, tv serie 
Using requests to scrap information about a tv serie, movie or even to compare between 2 shows, analyse, calculate and visualize the difference between them
using some well known libraries such as numpy, pandas, matplotlib

# Results SnowFall vs BreakingBad #
![image alt](https://github.com/ousax/CompareShows/blob/238474ff37e864db4cfa3128f12ed1729415ee62/f.png)
# Results Vikings vs Game Of Thrones (CLI) #
![image alt](https://github.com/ousax/CompareShows/blob/7369b88507d3644b3d385a2b4b9a8096a224ca5b/ff.png)
# Results Dexter (CLI) #
![image alt](https://github.com/ousax/CompareShows/blob/532e425bb478a6a9931679e3c3fe347c47b3671d/dexter.png)
# Results Dexter (VIZ, PLOT)
![image alt](https://github.com/ousax/CompareShows/blob/684f9e1a706fa0528741bc883412f898b9f04339/dexter%20plot.png)

### _Install on Linux_
- git clone https://github.com/ousax/CompareShows.git
- CompareShows
- pip3 install -r requirements
- chmod +x shows_comp.py
- python3 shows_comp.py
## Requirements 
1. requests
2. bs4
3. tqdm
4. termcolor
5. numpy
6. pandas
7. matplotlib
8. matplotlib_venn
# Usage Options
### Command-Line Arguments

| Argument           | Short | Type         | Required | Description                                                                 |
|--------------------|-------|--------------|----------|-----------------------------------------------------------------------------|
| `--name`           | `-n`  | `str`        | No       | Name of the movie or TV show                                                |
| `--type`           | `-t`  | `str` (choices: `movie`, `tv`) | No       | Type of content (movie or TV)                                               |
| `--season`         | `-s`  | `int`        | No       | Specific season to scrape (for TV series)                                   |
| `--episode`        | `-e`  | `int`        | No       | Specific episode to scrape (for TV series)                                  |
| `--top-rated`      |       | `flag`       | No       | Get top-rated episodes (for TV series)                                      |
| `--top-limit`      |       | `int` (default: `10`) | No       | Number of top episodes to display                                           |
| `--progress`       |       | `flag`       | No       | Show progress indicator when scraping                                       |
| `--viz`            |       | `flag`       | No       | Create visualization of ratings (for TV series)                             |
| `--viz-path`       |       | `str`        | No       | Path to save visualization (default: display)                               |
| `--save`           |       | `flag`       | No       | Generate streaming links for each episode/movie                            |
| `--output`         |       | `str` (file path) | No    | Save results to a JSON file                                                 |
| `--compare`        |       | `tuple(str, str)` | No    | Compare two shows by name (`SHOW1` and `SHOW2`)                             |

