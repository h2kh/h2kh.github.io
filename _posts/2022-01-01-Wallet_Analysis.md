---
layout: post
title: "Wallet analysis app for ETH"
subtitle: "Plug in your wallet address and get some interesting metrics"
nottableau: 'true'
---

Here is the **[link for the app](https://share.streamlit.io/h2kh/wallet_analysis/main/app.py)**. 
*took down the app for cost reasons but you can enjoy a GIF of the app functionality below* 

This app is created with Streamlit which is a Python-based web framework.

Wallet transactions are collected from the EtherScan API. ETH/USD rates are collected from the CoinGecko API.

Data as shown on a wallet's home page on EtherScan is not available from a single API endpoint. All of the data that is extracted from the different APIs is stored in a PostgreSQL database on AWS.

The different API endpoints used, in addition to my mental model of an ETH wallet transaction, influenced my design of the database. The unified view of the transactions data displayed above comes from joining and filtering the different tables in the database.

![Database schema](/assets/db_schema.png)

This database is always checked first whenever a new query is submitted by the app user in order to avoid unnecessary requests to the API endpoints.

If the desired data isn't available in the database, then the API endpoints are used.

In case I :

![app_gif](https://user-images.githubusercontent.com/21020474/163201889-9b3dae70-1eba-486c-aa33-23250b3a2801.gif)



