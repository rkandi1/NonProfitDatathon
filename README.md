# NonProfitDatathon
DSC Datathon. Creating Database for Non-Profits.

## Goals
The goal of this project is to find organizations that are closest in their goals to Understood.org's mission. Understood is a non-profit dedicated to serving the millions of families of kids who learn and think differently. Our programs for Families, Educators, and Young Adults focus on empowering people who learn and think differently and those who support them, offering customized, accessible resources and a compassionate community. Our Workplace program helps organizations across industries create inclusive workplaces, by developing and implementing best-in-class disability inclusion programs so they can hire, advance, and retain people with disabilities. The algorithm automates that process.


## Mining the Data
For mining the data we used the database by [ProPublica](https://projects.propublica.org/nonprofits/organizations/116037894). We accessed the data using their [API](https://projects.propublica.org/nonprofits/api) and scraping data from their original site. However we scraped data because another useful database was not available to us too much. [Guidestar](https://www.guidestar.org/) is a great database to use with regarding non-profits and will most probably work especially well with our algorihtm which uses Language processing to cluster non-profits. Their [API](https://apiportal.guidestar.org/) can retrieve data for mission statements and an organization's different stated goals. Additionally, data from Bloomberg and LinkedIn can be obtained and possibly used to find for-profit companies who might have charitable arms in their companies. However, we decided to stick with non-profits to simplify.

THe size of the dataset is also only closed on one state (NY). This can be expanded to other states and more data can be retrieved by contacting ProPublica.
