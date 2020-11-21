# NonProfitDatathon
DSC Datathon. Creating Database for Non-Profits.

## Goals
The goal of this project is to find organizations that are closest in their goals to Understood.org's mission. Understood is a non-profit dedicated to serving the millions of families of kids who learn and think differently. Understood is looking for potential partners and wants an updated set of partners with whom they can work closely. The algorithm needs to update regularly (semi-yearly) and quickly provide results.


## Data Mining
For mining the data we used the database by [ProPublica](https://projects.propublica.org/nonprofits/organizations/116037894). We accessed the data using their [API](https://projects.propublica.org/nonprofits/api) and scraping data from their original site. However we scraped data because another useful database was not available to us too much. [Guidestar](https://www.guidestar.org/) is a great database to use with regarding non-profits and will most probably work especially well with our algorihtm which uses unsupervised machine learning techniques (discussed in the next section). Guidestar [API](https://apiportal.guidestar.org/) can retrieve mission statements and program descriptions from the non-profits.

## Data Filtering
Because we aim to find non-profit entities similar to Understood mostly based on the organization's mission statements and/or program descriptions, we decide to use Latent Dirichlet Allocation model, a topic modeling algorithm, to process our data. In particular, we use LDA to cluster the organization descriptions into k groups and compare the extracted topics with Understood's mission statement and program descriptions. The group closest to Understood will be used to formulate the table of potential partners. 

## Future Work (Nov 21, 2020)
Even though our program is not yet finished, we would like to do the following work to fully implement our solution for Understood: 
1. Use better web scraping tools and techniques to extract real-time data instead of relying on existing third party database
2. Collect data from for-profit entities to complement the non-profit data
3. Use similarity matrix to find the cluster(s) that fits Understood's goal.
4. Come up with a testing dataset to evaluate the accuracy of unsupervised ML results. 
5. Implement a rating system based on arbitrary weights of the features input by the user(s) to tailor to Understood's specific, evolving demand
