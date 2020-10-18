 #  A Whale off the Port(folio)

![alt Whale image](Whale.png)

## Whale Returns

We are trying to determine which portfolio has performed best using data analysis. Here is the historic returns from "whale" investors, algorithmic portfolios, and the overall market of the S&P 500:

<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>SOROS FUND MANAGEMENT LLC</th>
      <th>PAULSON &amp; CO.INC.</th>
      <th>TIGER GLOBAL MANAGEMENT LLC</th>
      <th>BERKSHIRE HATHAWAY INC</th>
      <th>Algo 1</th>
      <th>Algo 2</th>
      <th>S&amp;P 500</th>
    </tr>
    <tr>
      <th>Date</th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>2015-03-03</th>
      <td>-0.001266</td>
      <td>-0.004981</td>
      <td>-0.000496</td>
      <td>-0.006569</td>
      <td>-0.001942</td>
      <td>-0.000949</td>
      <td>-0.004539</td>
    </tr>
    <tr>
      <th>2015-03-04</th>
      <td>0.002230</td>
      <td>0.003241</td>
      <td>-0.002534</td>
      <td>0.004213</td>
      <td>-0.008589</td>
      <td>0.002416</td>
      <td>-0.004389</td>
    </tr>
    <tr>
      <th>2015-03-05</th>
      <td>0.004016</td>
      <td>0.004076</td>
      <td>0.002355</td>
      <td>0.006726</td>
      <td>-0.000955</td>
      <td>0.004323</td>
      <td>0.001196</td>
    </tr>
    <tr>
      <th>2015-03-06</th>
      <td>-0.007905</td>
      <td>-0.003574</td>
      <td>-0.008481</td>
      <td>-0.013098</td>
      <td>-0.004957</td>
      <td>-0.011460</td>
      <td>-0.014174</td>
    </tr>
    <tr>
      <th>2015-03-09</th>
      <td>0.000582</td>
      <td>0.004225</td>
      <td>0.005843</td>
      <td>-0.001652</td>
      <td>-0.005447</td>
      <td>0.001303</td>
      <td>0.003944</td>
    </tr>
    <tr>
      <th>...</th>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
    </tr>
    <tr>
      <th>2019-04-16</th>
      <td>0.002699</td>
      <td>0.000388</td>
      <td>-0.000831</td>
      <td>0.000837</td>
      <td>-0.006945</td>
      <td>0.002899</td>
      <td>0.000509</td>
    </tr>
    <tr>
      <th>2019-04-17</th>
      <td>-0.002897</td>
      <td>-0.006467</td>
      <td>-0.004409</td>
      <td>0.003222</td>
      <td>-0.010301</td>
      <td>-0.005228</td>
      <td>-0.002274</td>
    </tr>
    <tr>
      <th>2019-04-18</th>
      <td>0.001448</td>
      <td>0.001222</td>
      <td>0.000582</td>
      <td>0.001916</td>
      <td>-0.000588</td>
      <td>-0.001229</td>
      <td>0.001579</td>
    </tr>
    <tr>
      <th>2019-04-22</th>
      <td>-0.002586</td>
      <td>-0.007333</td>
      <td>-0.003640</td>
      <td>-0.001088</td>
      <td>0.000677</td>
      <td>-0.001936</td>
      <td>0.001012</td>
    </tr>
    <tr>
      <th>2019-04-23</th>
      <td>0.007167</td>
      <td>0.003485</td>
      <td>0.006472</td>
      <td>0.013278</td>
      <td>0.004969</td>
      <td>0.009622</td>
      <td>0.008841</td>
    </tr>
  </tbody>
</table>
</div>



---

# Portfolio Analysis

In order to understand how the portfolios are performing, it helps to visually see the differencees between each one.  

## Performance

The goal for a successful portfolio is to beat the overall market. This is easier said than done. Daily returns will vary and may often lead to a large variance from the overall market:
    
![png](output_25_1.png)
  
What the graph above is showing are the daily returns as compared to the S&P 500 (pink). As you can see, nearly every portfolio, at one point or another, will see a higher volitility than the overall market. But does that mean that they are better?
    
![png](output_26_1.png)
    
Based on the data given, the first algorithmic portfolio and Berkshire Hathaway were the only two that were able to outperform.

## Risk

"The higher the risk, the higher the reward". This may be true in some cases, but does not always guarantee profit. For those that tend to be more risk averse, some portfolios will yield a safer bounty:
    
![png](output_28_1.png)
    
Based on each portfolio's standard deviation, we can see that Berkshire Hathaway was the riskest portfolio to be in. In this case, the elevated risk was worth it.

<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>STD</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>SOROS FUND MANAGEMENT LLC</th>
      <td>0.125335</td>
    </tr>
    <tr>
      <th>PAULSON &amp; CO.INC.</th>
      <td>0.111488</td>
    </tr>
    <tr>
      <th>TIGER GLOBAL MANAGEMENT LLC</th>
      <td>0.172936</td>
    </tr>
    <tr>
      <th>BERKSHIRE HATHAWAY INC</th>
      <td>0.205077</td>
    </tr>
    <tr>
      <th>Algo 1</th>
      <td>0.120967</td>
    </tr>
    <tr>
      <th>Algo 2</th>
      <td>0.132430</td>
    </tr>
    <tr>
      <th>S&amp;P 500</th>
      <td>0.135786</td>
    </tr>
  </tbody>
</table>
</div>



---

## Rolling Statistics

Risk changes over time. As shown on the graph below, there are actually periods of time (such as April 2018) where the S&P 500 has actually yielded the highest standard deviation of the group.
    
![png](output_34_1.png)

It is hard to tell from this graph how closely related some portfolios are to the S&P 500. If we compare each one and look at the data, it appears that the second algorithmic portfolio most closely mimics the S&P.
    
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>SOROS FUND MANAGEMENT LLC</th>
      <th>PAULSON &amp; CO.INC.</th>
      <th>TIGER GLOBAL MANAGEMENT LLC</th>
      <th>BERKSHIRE HATHAWAY INC</th>
      <th>Algo 1</th>
      <th>Algo 2</th>
      <th>S&amp;P 500</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>SOROS FUND MANAGEMENT LLC</th>
      <td>1.000000</td>
      <td>0.699914</td>
      <td>0.561243</td>
      <td>0.754360</td>
      <td>0.321211</td>
      <td>0.826873</td>
      <td>0.837864</td>
    </tr>
    <tr>
      <th>PAULSON &amp; CO.INC.</th>
      <td>0.699914</td>
      <td>1.000000</td>
      <td>0.434479</td>
      <td>0.545623</td>
      <td>0.268840</td>
      <td>0.678152</td>
      <td>0.669732</td>
    </tr>
    <tr>
      <th>TIGER GLOBAL MANAGEMENT LLC</th>
      <td>0.561243</td>
      <td>0.434479</td>
      <td>1.000000</td>
      <td>0.424423</td>
      <td>0.164387</td>
      <td>0.507414</td>
      <td>0.623946</td>
    </tr>
    <tr>
      <th>BERKSHIRE HATHAWAY INC</th>
      <td>0.754360</td>
      <td>0.545623</td>
      <td>0.424423</td>
      <td>1.000000</td>
      <td>0.292033</td>
      <td>0.688082</td>
      <td>0.751371</td>
    </tr>
    <tr>
      <th>Algo 1</th>
      <td>0.321211</td>
      <td>0.268840</td>
      <td>0.164387</td>
      <td>0.292033</td>
      <td>1.000000</td>
      <td>0.288243</td>
      <td>0.279494</td>
    </tr>
    <tr>
      <th>Algo 2</th>
      <td>0.826873</td>
      <td>0.678152</td>
      <td>0.507414</td>
      <td>0.688082</td>
      <td>0.288243</td>
      <td>1.000000</td>
      <td>0.858764</td>
    </tr>
    <tr>
      <th>S&amp;P 500</th>
      <td>0.837864</td>
      <td>0.669732</td>
      <td>0.623946</td>
      <td>0.751371</td>
      <td>0.279494</td>
      <td>0.858764</td>
      <td>1.000000</td>
    </tr>
  </tbody>
</table>
</div>

No matter how independent these other portfolios might seem, the S&P does affect each one. Some more than others. Take a look at the "riskiest" portfolio of Berkshire Hathaway when compared to the S&P:

    
![png](output_36_1.png)
    
From this we see two things:
1. Berkshire Hathaway always had a higher standard deviation than the S&P 500.
2. The low points in this graph indicate that Berkshire is occasionally sensitive to the movements in the S&P 500.


An alternative way to demonstrate a rolling window is to take the exponentially weighted moving average. Here are the portfolios when compared to the S&P:
    
![png](output_37_1.png)
    


---

## Sharpe Ratios
In reality, investment managers and thier institutional investors look at the ratio of return-to-risk, and not just returns alone. (After all, if you could invest in one of two portfolios, each offered the same 10% return, yet one offered lower risk, you'd take that one, right?).

This is where the Sharpe Ratio comes in. The Sharpe Ratio helps investors understand the Return on Investment (ROI) when compared to the risk of that portfolio.
    
![png](output_41_1.png)
    

On the basis of this performance metric, our first algo strategy outperforms both 'the market' and the whales.

---

# Personal Portfolio Returns

To demonstrate how well this algo strategy works, I wanted to see if I could put together a winning portfolio that would outperform the algo. My portfolio consists of 5 stocks: AMD, BA, NVDA, V, and WMT.

<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>AMD</th>
      <th>BA</th>
      <th>NVDA</th>
      <th>V</th>
      <th>WMT</th>
    </tr>
    <tr>
      <th>Date</th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>2017-10-17</th>
      <td>14.160000</td>
      <td>258.619995</td>
      <td>197.750000</td>
      <td>107.540001</td>
      <td>85.980003</td>
    </tr>
    <tr>
      <th>2017-10-18</th>
      <td>14.070000</td>
      <td>260.040009</td>
      <td>197.580002</td>
      <td>107.800003</td>
      <td>86.220001</td>
    </tr>
    <tr>
      <th>2017-10-19</th>
      <td>13.950000</td>
      <td>259.040009</td>
      <td>197.800003</td>
      <td>107.019997</td>
      <td>86.400002</td>
    </tr>
    <tr>
      <th>2017-10-20</th>
      <td>13.810000</td>
      <td>264.750000</td>
      <td>196.899994</td>
      <td>107.550003</td>
      <td>87.440002</td>
    </tr>
    <tr>
      <th>2017-10-23</th>
      <td>14.100000</td>
      <td>262.320007</td>
      <td>196.619995</td>
      <td>107.529999</td>
      <td>88.650002</td>
    </tr>
    <tr>
      <th>...</th>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
    </tr>
    <tr>
      <th>2020-10-12</th>
      <td>84.290001</td>
      <td>167.350006</td>
      <td>569.039978</td>
      <td>206.399994</td>
      <td>144.250000</td>
    </tr>
    <tr>
      <th>2020-10-13</th>
      <td>85.279999</td>
      <td>162.139999</td>
      <td>569.929993</td>
      <td>204.320007</td>
      <td>146.229996</td>
    </tr>
    <tr>
      <th>2020-10-14</th>
      <td>84.209999</td>
      <td>163.240005</td>
      <td>563.809998</td>
      <td>202.199997</td>
      <td>143.940002</td>
    </tr>
    <tr>
      <th>2020-10-15</th>
      <td>83.129997</td>
      <td>164.240005</td>
      <td>558.799988</td>
      <td>199.550003</td>
      <td>144.529999</td>
    </tr>
    <tr>
      <th>2020-10-16</th>
      <td>83.169998</td>
      <td>167.350006</td>
      <td>552.460022</td>
      <td>200.259995</td>
      <td>144.710007</td>
    </tr>
  </tbody>
</table>
</div>

I then went through and repeated the steps to find out how my portfolio's performance stood up against the competition.

<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>My Portfolio</th>
      <th>SOROS FUND MANAGEMENT LLC</th>
      <th>PAULSON &amp; CO.INC.</th>
      <th>TIGER GLOBAL MANAGEMENT LLC</th>
      <th>BERKSHIRE HATHAWAY INC</th>
      <th>Algo 1</th>
      <th>Algo 2</th>
      <th>S&amp;P 500</th>
    </tr>
    <tr>
      <th>Date</th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>2017-10-18</th>
      <td>0.002500</td>
      <td>-0.001167</td>
      <td>-0.007151</td>
      <td>-0.002460</td>
      <td>0.004949</td>
      <td>-0.001652</td>
      <td>-0.000138</td>
      <td>0.000742</td>
    </tr>
    <tr>
      <th>2017-10-19</th>
      <td>-0.002253</td>
      <td>-0.002063</td>
      <td>0.005359</td>
      <td>-0.006275</td>
      <td>-0.010606</td>
      <td>0.000585</td>
      <td>-0.001053</td>
      <td>0.000328</td>
    </tr>
    <tr>
      <th>2017-10-20</th>
      <td>0.009395</td>
      <td>0.002271</td>
      <td>-0.000603</td>
      <td>0.004499</td>
      <td>0.002820</td>
      <td>-0.002531</td>
      <td>0.003606</td>
      <td>0.005117</td>
    </tr>
    <tr>
      <th>2017-10-23</th>
      <td>-0.001835</td>
      <td>-0.004255</td>
      <td>-0.004292</td>
      <td>0.002513</td>
      <td>-0.008789</td>
      <td>-0.004601</td>
      <td>-0.005884</td>
      <td>-0.003972</td>
    </tr>
    <tr>
      <th>2017-10-24</th>
      <td>0.009115</td>
      <td>-0.004026</td>
      <td>-0.001726</td>
      <td>0.003547</td>
      <td>0.002099</td>
      <td>-0.004328</td>
      <td>-0.000893</td>
      <td>0.001618</td>
    </tr>
    <tr>
      <th>...</th>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
    </tr>
    <tr>
      <th>2019-04-16</th>
      <td>0.012536</td>
      <td>0.002699</td>
      <td>0.000388</td>
      <td>-0.000831</td>
      <td>0.000837</td>
      <td>-0.006945</td>
      <td>0.002899</td>
      <td>0.000509</td>
    </tr>
    <tr>
      <th>2019-04-17</th>
      <td>-0.005946</td>
      <td>-0.002897</td>
      <td>-0.006467</td>
      <td>-0.004409</td>
      <td>0.003222</td>
      <td>-0.010301</td>
      <td>-0.005228</td>
      <td>-0.002274</td>
    </tr>
    <tr>
      <th>2019-04-18</th>
      <td>0.001741</td>
      <td>0.001448</td>
      <td>0.001222</td>
      <td>0.000582</td>
      <td>0.001916</td>
      <td>-0.000588</td>
      <td>-0.001229</td>
      <td>0.001579</td>
    </tr>
    <tr>
      <th>2019-04-22</th>
      <td>-0.003266</td>
      <td>-0.002586</td>
      <td>-0.007333</td>
      <td>-0.003640</td>
      <td>-0.001088</td>
      <td>0.000677</td>
      <td>-0.001936</td>
      <td>0.001012</td>
    </tr>
    <tr>
      <th>2019-04-23</th>
      <td>0.003276</td>
      <td>0.007167</td>
      <td>0.003485</td>
      <td>0.006472</td>
      <td>0.013278</td>
      <td>0.004969</td>
      <td>0.009622</td>
      <td>0.008841</td>
    </tr>
  </tbody>
</table>
</div>



## Performance and Risk Analysis when compared to the others

# Risk

When I was deciding on which stocks to include in my portfolio, I chose 5 stocks that have been popular choices amoungst investors lately. I did diversify a little, it may not have been enough:

<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>STD</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>My Portfolio</th>
      <td>0.256996</td>
    </tr>
    <tr>
      <th>SOROS FUND MANAGEMENT LLC</th>
      <td>0.143917</td>
    </tr>
    <tr>
      <th>PAULSON &amp; CO.INC.</th>
      <td>0.116172</td>
    </tr>
    <tr>
      <th>TIGER GLOBAL MANAGEMENT LLC</th>
      <td>0.211266</td>
    </tr>
    <tr>
      <th>BERKSHIRE HATHAWAY INC</th>
      <td>0.223649</td>
    </tr>
    <tr>
      <th>Algo 1</th>
      <td>0.117606</td>
    </tr>
    <tr>
      <th>Algo 2</th>
      <td>0.133711</td>
    </tr>
    <tr>
      <th>S&amp;P 500</th>
      <td>0.151731</td>
    </tr>
  </tbody>
</table>
</div>

No surprise, my portfolio had the highest standard deviation (a.k.a. the highest risk) of any portfolio. as the rolling standard deviation will also show, my portfolio spends the most time above all other standard deviations. 
    
![png](output_62_1.png)
    
In my defense, Tiger Global Management spent about a month with a higher standard deviation than my portfolio ever had.

# Annualized Sharpe Ratios

I knew the risk factor was there, but I wanted to see if the risk was worth it. 
    
![png](output_64_1.png)
    
According to the Sharpe Ratio, our algo portfolio still reigns. Although I didn't manage to be the highest outperformer, my portfolio did manage to have a greater ROI based on risk than the S&P!

# Beta

As far as correlation to the market, the second algo portfolio is still the closest related to the S&P 500. 

<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>My Portfolio</th>
      <th>SOROS FUND MANAGEMENT LLC</th>
      <th>PAULSON &amp; CO.INC.</th>
      <th>TIGER GLOBAL MANAGEMENT LLC</th>
      <th>BERKSHIRE HATHAWAY INC</th>
      <th>Algo 1</th>
      <th>Algo 2</th>
      <th>S&amp;P 500</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>My Portfolio</th>
      <td>1.000000</td>
      <td>0.679664</td>
      <td>0.579324</td>
      <td>0.403140</td>
      <td>0.763582</td>
      <td>0.243830</td>
      <td>0.723187</td>
      <td>0.829311</td>
    </tr>
    <tr>
      <th>SOROS FUND MANAGEMENT LLC</th>
      <td>0.679664</td>
      <td>1.000000</td>
      <td>0.751071</td>
      <td>0.511691</td>
      <td>0.780257</td>
      <td>0.326331</td>
      <td>0.828155</td>
      <td>0.831343</td>
    </tr>
    <tr>
      <th>PAULSON &amp; CO.INC.</th>
      <td>0.579324</td>
      <td>0.751071</td>
      <td>1.000000</td>
      <td>0.492073</td>
      <td>0.626057</td>
      <td>0.337278</td>
      <td>0.772946</td>
      <td>0.748047</td>
    </tr>
    <tr>
      <th>TIGER GLOBAL MANAGEMENT LLC</th>
      <td>0.403140</td>
      <td>0.511691</td>
      <td>0.492073</td>
      <td>1.000000</td>
      <td>0.372517</td>
      <td>0.134633</td>
      <td>0.479858</td>
      <td>0.557858</td>
    </tr>
    <tr>
      <th>BERKSHIRE HATHAWAY INC</th>
      <td>0.763582</td>
      <td>0.780257</td>
      <td>0.626057</td>
      <td>0.372517</td>
      <td>1.000000</td>
      <td>0.310652</td>
      <td>0.779185</td>
      <td>0.830721</td>
    </tr>
    <tr>
      <th>Algo 1</th>
      <td>0.243830</td>
      <td>0.326331</td>
      <td>0.337278</td>
      <td>0.134633</td>
      <td>0.310652</td>
      <td>1.000000</td>
      <td>0.317405</td>
      <td>0.269803</td>
    </tr>
    <tr>
      <th>Algo 2</th>
      <td>0.723187</td>
      <td>0.828155</td>
      <td>0.772946</td>
      <td>0.479858</td>
      <td>0.779185</td>
      <td>0.317405</td>
      <td>1.000000</td>
      <td>0.878185</td>
    </tr>
    <tr>
      <th>S&amp;P 500</th>
      <td>0.829311</td>
      <td>0.831343</td>
      <td>0.748047</td>
      <td>0.557858</td>
      <td>0.830721</td>
      <td>0.269803</td>
      <td>0.878185</td>
      <td>1.000000</td>
    </tr>
  </tbody>
</table>
</div>

However, just like with the Berkshire Hathaway portfolio, we can see that my portfolio still has the occasional day where it near mimics the movement of the market:
    
![png](output_66_1.png)
    
I may not be considered a whale, but I have shown that it is possible to compete with one.
