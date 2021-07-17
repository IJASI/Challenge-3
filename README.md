
#  Crypto Arbitrage Application (CAA)

The Crypto Arbitrage application allows the end-users to analyze information from a multitude of cryptocurrency exchanges to find arbitrage opportunities. The CAA allows for the selection of the specific dates within the exchange data sets and allows the end-user to visualize the differences in pricing between exchanges via data-frames and/or graphs. 

## Installation

Download the CAA code files within the following GitHub repository [IJASI Repository](https://github.com/IJASI/Challenge-3/tree/491335d4123fae396530363cb79be7070e049796). Get to the downloaded CAA files on your machine via bash and initiate your dev as well as your Jupyter lab. 


```bash

cd crypto_arbitrage_code_files

conda activate dev

jupyter lab
 
```

Once Jupyter Lab is open proceed to open the crypto_arbitrage.ipynb file from your folder tree. 


## Technologies

As mentioned previously [Jupyter](https://jupyter.org/) is needed in order to properly open the CAA files. In order to run the CAA the pandas library must be imported. We will also need to invoke matplotlib module. 

```python

import pandas as pd
from pathlib import Path
%matplotlib inline

```
## Usage Examples 

Using the .plot and .loc functionalities we can select a specific date and show a graph for the desired dates. 
```python
import 

bitstampdf['Close'].loc['2018-1-29'].plot(
    legend=True, figsize=(15, 10), title="March 2018", color="blue", label="Bitstamp")
coinbasedf['Close'].loc['2018-1-29'].plot(
    legend=True, figsize=(15, 10), color="orange", label="Coinbase")
```

![Coinbase V Bitstamp closing prices for 1/29/18](/Images/Bitstamp_v_Coinbase_early.PNG)

![Coinbase V Bitstamp closing prices for 1/29/18](/Images/Bitstamp_v_Coinbase_middle.PNG)


or you can get a dataframe for your statical analysis in order view for instance which trades would be positive 

![Coinbase V Bitstamp closing prices for 1/29/18](/Images/Statistic_over_zero_early.PNG)
 


## Contributors(ing)
This a project designed by:

Jose Sampedro
sampedro.jose.a@gmail.com

With the contributions and assistance of:

The Columbia Fintech Bootcamp TAs and Toturs

**Pull requests are welcomed. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.

## License

[See GNU v3.0](https://github.com/IJASI/Challenge-3/blob/491335d4123fae396530363cb79be7070e049796/LICENSE)

