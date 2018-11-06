# niveshi_interview_problem
This project if you are applying for Niveshi ML Engineer role. Before starting on project, few housekeeping rules:
a) Fork the project into your account and work on clone. If you make repo private, please add @rahulgoyal3004 and @deependersingla as collaborators.
b) When you submit project, email us: Github link or any feedback you have about entire process.
c) We are just a call/email away if you have questions anywhere. Feel free to ask.

#Problem Statement:
The file bank_future_data.csv contains last 6 month of price, volume data for 14 Banking instrument in Indian market. The Format is this:
a) DateTime: Timestamp of the price data sent at every turn of minute in format (dd/mm/yyyy HH:MM)
b) Open: Open Price, Symbol of the stock . For instance: SBI,PNB, NIFTY etc + "_0"
c) High: High Price,  Symbol of the stock . For instance: SBI,PNB, NIFTY etc + "_1"
d) Low: Low Price,  Symbol of the stock . For instance: SBI,PNB, NIFTY etc + "_2"
e) Close: Close price,  Symbol of the stock . For instance: SBI,PNB, NIFTY etc + "_3"
f) Volume: Volume Traded,  Symbol of the stock . For instance: SBI,PNB, NIFTY etc + "_4"

This is repeated for other stocks. Hence the format is:
DateTime,BANKBARODA_OPEN,BANKBARODA_HIGH,BANKBARODA_LOW,BANKBARODA_CLOSE,BANKBARODA_VOLUME,CANARABANK_OPEN,CANARABANK_HIGH,CANARABANK_LOW,CANARABANK_CLOSE,CANARABANK_VOLUME,AXISBANK,AXISBANK_OPEN,AXISBANK_HIGH,AXISBANK_LOW,AXISBANK_CLOSE,AXISBANK_VOLUME,SBI_OPEN,SBI_HIGH,SBI_LOW,SBI_CLOSE,SBI_VOLUME,PNB_OPEN,PNB_HIGH,PNB_LOW,PNB_CLOSE,PNB_VOLUME,ICICIBANK_OPEN,ICICIBANK_HIGH,ICICIBANK_LOW,ICICIBANK_CLOSE,ICICIBANK_VOLUME,HDFC_OPEN,PNB_VOLUME,HDFC_HIGH,HDFC_LOW,HDFC_CLOSE,HDFC_VOLUME,FEDERALBANK_OPEN,FEDERALBANK_HIGH,FEDERALBANK_LOW,FEDERALBANK_CLOSE,FEDERALBANK_VOLUME,HDFCBANK_OPEN,HDFCBANK_HIGH,HDFCBANK_LOW,HDFCBANK_CLOSE,HDFCBANK_VOLUME,INDUSINDBANK_OPEN,INDUSINDBANK_HIGH,INDUSINDBANK_LOW,INDUSINDBANK_CLOSE,INDUSINDBANK_VOLUME,KOTAKBANK_OPEN,KOTAKBANK_HIGH,KOTAKBANK_LOW,KOTAKBANK_CLOSE,KOTAKBANK_VOLUME,NIFTY_OPEN,NIFTY_HIGH,NIFTY_LOW,NIFTY_CLOSE,NIFTY_VOLUME,YESBANK_OPEN,YESBANK_HIGH,YESBANK_LOW,YESBANK_CLOSE,YESBANK_VOLUME,BANKNIFTY_OPEN,BANKNIFTY_HIGH,BANKNIFTY_LOW,BANKNIFTY_CLOSE,BANKNIFTY_VOLUME

#If you want to understand financial data: https://en.wikipedia.org/wiki/Open-high-low-close_chart. 

We want you to take this data and expand this data. For e.g the way people uses GAN to expand data without changing the distribution of the data. Ideas like:
a) Change the distribution of each stock price by some 1%. This will generate a lot of data, as you can keep one stock constant and change others.

We are happy even if you try smaller ideas because idea is to check your approach.