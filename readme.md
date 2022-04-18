# USDRUB altdata

Get alternative USDRUB exchange rate values from Telegram chats and Binance exchange (USDTRUB). 

First you need to install the necessary libraries:  
`pip install -r requirements.txt`

All structured data is located in the `reports` folder, notebooks - in `src`
     
### Telegram

* Get API from https://my.telegram.org/auth, fill the values into `config.ini`
* Launch `Data_load.ipynb` to get latest raw messages data ("ticks")
* Run `Parse_messages.ipynb` for each chat to get structured data (daily bid/ask quantiles)
  * change `chat` name (right after paths chunk)

### Binance

* `Get_binance.ipynb`
* Update the `START_DATE` and `END_DATE`
* Run the notebook to get hourly open-high-low-close data and daily quantiles

Some more info in `methodology.docx`