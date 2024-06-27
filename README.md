# Crowdfunding_ETL

This code takes the extracts data from crowdfunding and contacts excel file to produce four csv files. campaign. csv contains crowdfunding campaign information. contacts.csv contains contact information for those that funded the campaigns. category.csv and subcategory.csv have the names and id of each category or subcategory. The csv files were then imported into a SQL database using the crowdfunding_db_schema.sql.

References:

Used following code from Xpert Learning  to convert date correctly with desired format. 
    campaign_df['launched_date'] = pd.to_datetime(campaign_df["launched_date"], unit='s').dt.strftime('%Y-%m-%d')
    campaign_df['end_date'] = pd.to_datetime(campaign_df["end_date"], unit='s').dt.strftime('%Y-%m-%d')