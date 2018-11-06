# Niveshi Data Generator
This project is for candidate who are on later stage interview process with Niveshi. Before starting on project, few housekeeping rules:
<br>a) Fork the repo into your account. If you make repo private, please add @rahulgoyal3004 and @deependersingla as collaborators.<br>
b) When you submit project, email us: Github link and you approach you took.<br>
c) We are just a call/email away if you have any guestion.
<br>


## Problem Statement:
One of the biggest problem in using Deep RL with trading is limitation of data. When you apply RL to a gaming engine you can play infinite number of episodes, in trading you just have historical data available for you to make game episodes. Niveshi Data Generator solve this problem by taking a historical data and simulate new data. It's built to keep mainly two things in mind: <br>
a) Data Sanity still remain same, don't change underlying distribution. System know about Garbage in and Garbage out<br>
b) System will simulate a lot of new data so you can just concentrate on writing best RL engine

#Input:<br>
System take file bank_future_data.csv as input. The file contains last 6 month of price, volume data for 5 Banking instrument in Indian market. The Format is this:<br>
a) DateTime: Timestamp of the price data sent at every turn of minute in format (dd/mm/yyyy HH:MM)<br>
b) Open: Open Price, Symbol of the stock . For instance: SBI,PNB etc + "_0"<br>
c) High: High Price,  Symbol of the stock . For instance: SBI,PNB etc + "_1"<br>
d) Low: Low Price,  Symbol of the stock . For instance: SBI,PNB etc + "_2"<br>
e) Close: Close price,  Symbol of the stock . For instance: SBI,PNB etc + "_3"<br>
f) Volume: Volume Traded,  Symbol of the stock . For instance: SBI,PNB,etc + "_4"<br>

This is repeated for other stocks. Hence the format is:<br><br>
DateTime,BANKBARODA_OPEN,BANKBARODA_HIGH,BANKBARODA_LOW,BANKBARODA_CLOSE,BANKBARODA_VOLUME,CANARABANK_OPEN,CANARABANK_HIGH,CANARABANK_LOW,CANARABANK_CLOSE,CANARABANK_VOLUME,AXISBANK,AXISBANK_OPEN,AXISBANK_HIGH,AXISBANK_LOW,AXISBANK_CLOSE,AXISBANK_VOLUME,SBI_OPEN,SBI_HIGH,SBI_LOW,SBI_CLOSE,SBI_VOLUME,PNB_OPEN,PNB_HIGH,PNB_LOW,PNB_CLOSE,PNB_VOLUME


Ideas:<br> You can try straight forward method like change prices by -max to + max for each stock or something like GAN. We will leave this on your imagination. 

## Random Resources <br>
a) If you want to understand financial data: https://en.wikipedia.org/wiki/Open-high-low-close_chart. <br>
b) https://arxiv.org/abs/1706.02633<br>