# DSA210-Term-Project

## Project Proposal
The goal of this project is to explore the entirety of my Youtube data, which includes search history, watch history, subscriptions etc. Since I've been using the same account for most of my life, I will be able to visualize how my usage evolved over time, how my interests changed, what type of content I keep coming back to, how my watchtime changes during the year and more! Youtube is most probably the site I have spent the most time on in my life so I am genuinely curious about what I will uncover about my usage. I expect to see my usage drop significantly during school semesters, and content switch to school related topics, and during holidays, increase significantly with hobby related content consumption.

## Data and Data Collection
I will be using Google Takeout to collect my Youtube data. The downloaded data includes the following: channels, clips, comments, creator-demographics, history, kids,live chats, music (library and uploads), playlists, shopping, subscriptions, support issues ,video metadata ,videos. I will not be using all of this data, but having them will be useful if there arises a need for that data. The downloaded data will be in .csv and .json formats.

--

## Hypotheses

### Daytime Usage vs Nighttime Usage
$H_{0}$: Daytime usage is less than or equal to nighttime usage.  
$H_{1}$: Daytime usage is significantly higher than nighttime usage.  

Daytime Mean (videos/day):   15.76  
Nighttime Mean (videos/day): 10.10  
p-value: 2.5113185059602055e-14  
Reject H0, p-value is significant  

### Exam Period Usage CHange
$H_{0}$: YouTube usage does not change during exam periods.  
$H_{1}$: There is a significant change in YouTube usage during exam periods.  

Exam Daily Mean: 7.70, Non-Exam Mean: 18.15  
p-value: 0.000000000000000000000000000024  
Result: Significant Change (Reject H0)  

### Channel Diversity Change
$H_{0}$: Channel diversity doesn't change over the years.  
$H_{1}$: Channel diversity changes from 2021 to 2025.  

Mean Unique Channels (2021): 246.7  
Mean Unique Channels (2025): 373.5  
p-value: 0.1577  
Result: No Change  

### Music at Night
$H_{0}$: Music related content is not more frequently watched at night.  
$H_{1}$: Music related content is more frequently watched at night.  

Night Music Mean: 1.32, Day Music Mean: 2.09  
p-value: 1.0000  
p-value not significant  


### Attention-Span Decrease
$H_{0}$: Short-form content consumption does not change over time.  
$H_{1}$: Short-form content consumption increases over time.  

Correlation: 0.5324  
p-value: 0.0000341465  
My attention span has decreased :( (increase in rapid-switching) (Reject H0)  

### Changing Interests
$H_{0}$: The most dominant category in 2021 is the same in 2025.  
$H_{1}$: The most dominant category has changed from 2021 to 2025.  

Top Category 2021: Gaming  
Top Category 2025: Gaming  
Most dominant category has NOT changed from 2021 to 2025  
Fail to reject H0  

--

## Data Processing and Feature Engineering
1. Used DataFrame from Pandas to store the raw data that came in the JSON format.
2. Extracted hour, day_name, year and month from the timestamp.
3. Titles of the vides were cleaned
4. Channel names were extracted from the 'Subtitles' field
## Exploratory Data Analysis (EDA)

![](/assets/perhour.png)

![](/assets/perday.png)

![](/assets/heatmap.png)

![](/assets/mostcommonwords.png)

![](/assets/mostwatcedchannels.png)

![](/assets/categories.png)


## Tools
Python, Pandas, NumPy, Matplotlib, Seaborn, SciPy, Jupyter, Git
