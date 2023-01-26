# CSS_Eleicoes
Aim of the project is to compare the toxicity/polarization on twitter and the elections results/abstention 


## Methodology
- Gather data from Twitter
- Compute the toxicity of each tweet
- Calculate average toxicity score for each state
- Compare score against elecions results/abstention


## File System

### Scripts
*Files used for calculations, logic and data collection*
- FinalAug/-Sep/-Oct => Gathering tweets from the respective month (**@TwitterAPI**); toxicity score calculation (**@PerspectiveAPI**); adding results to an individual dictionary with states as keys; writing said dictionary into a JSON file (see **Data**) 
- ToxicityAndElectionResults => Combining data from all months; calculating average toxicity for each state and creating graphs 
- Archive => Prototypes, testing, and scraped approaches 

### Data
*Tweets toxicity scores for respective months*
- dataAug => Tweets from August 2022
- dataSept => Tweets from September 2022
- dataOct => Tweets from October 2022
- data_elections => Election results, abstention quotas, etc. divided by state. 


## Libraries
- tweepy: Working with Twitter - https://docs.tweepy.org/en/stable/
- numpy: Calculate correlation - https://numpy.org/ 
- matplotlib: Create graphs - https://matplotlib.org/ 
- googleapiclient(discovery): Toxicity measurement - **@PerspectiveAPI**
- tqdm: Progressbar to check on tweets gathering progress
- ufbr: Dictionary with Brazilian cities in each state (used for mapping tweets into each state) - https://www.google.com/url?sa=t&rct=j&q=&esrc=s&source=web&cd=&cad=rja&uact=8&ved=2ahUKEwjrwcWZm-b8AhXFhP0HHaQzDaEQFnoECBkQAQ&url=https%3A%2F%2Fgithub.com%2FSidon%2Fpy-ufbr&usg=AOvVaw174SO-sOoypkRCvAj0Aquk
- datetime
- time 
- csv
- json

## References
- data_elections: https://sig.tse.jus.br/ords/dwapr/seai/r/sig-eleicao/estatisticas-eleicao?session=210277115010534
- PerspectiveAPI: https://developers.perspectiveapi.com
- TwitterAPI: https://developer.twitter.com/en/docs/twitter-api

