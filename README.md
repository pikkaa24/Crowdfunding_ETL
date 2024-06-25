# Crowdfunding_ETL



References:

Used following code from Xpert Learning  to convert date correctly with desired format. 
    campaign_df['launched_date'] = pd.to_datetime(campaign_df["launched_date"], unit='s').dt.strftime('%Y-%m-%d')
    campaign_df['end_date'] = pd.to_datetime(campaign_df["end_date"], unit='s').dt.strftime('%Y-%m-%d')