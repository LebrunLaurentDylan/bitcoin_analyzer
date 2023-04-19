# Projet Bitcoin_Analyzer

## About this project :

These are simple algorithms that allows you to extract data about any crypto-currencies
from an API *(coinapi.io)*.
it updates itself with day to days datas each time it launches
it to draws graphs and curves from these datas and then use 
them to determine sell and buy points *(always ends up selling)* based on its own calculation 
then use a fake wallet containing 1000 USD(or EUR) to buy and sell BTC

**the very point of this algorithm is to be able to make fake profit**

So it will be using two "moving-averages" based on the closing rate of each day
to calculate and determine when is the right time to buy/sell
this program will always be based on past datas up to yesterday's date 
*(giving that the closing date will only occur when the present day is past)*
Due to the number of call limitation on the API, the algorithm saves the data it gathered in a json file
to prevent calling all the data each time you run the program but just calling the data you don't have
and have then stored in the json file, ordered by date.

lastly the algorithm possesses a function for finding and replacing inconsistencies in the data it gathered
(such as obviously false data rates) and replace then by the previous good data it has in memory with the right date.

