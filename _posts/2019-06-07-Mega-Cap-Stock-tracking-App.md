---
layout: post
title: "Stock Tracking App for NASDAQ Mega Cap Companies"
subtitle: "Price charts and relevant news for NASDAQ Mega Cap stocks in addition to some useful metrics"
nottableau: 'true'
---

Here is the **[link for the app](https://fathomless-stream-09745.herokuapp.com/)**.

I have used the following Python libraries in this project: Pandas, Matplotlib, YFinance, MPLFinance, and Requests.

The app is created using the Streamlit framework and is hosted on Heroku (it's a free service so slightly slower than commercially-deployed apps).

All of the financial data is scraped from Yahoo Finance in real time while the 'relevant news' data comes from NewsAPI.

Some screenshots below:

{:refdef: style="text-align: center;"}
![Dashboard snapshot]({{ site.baseimg }}/assets/stock1.jpg)
{: refdef}

{:refdef: style="text-align: center;"}
![Dashboard snapshot]({{ site.baseimg }}/assets/stock2.jpg)
{: refdef}
