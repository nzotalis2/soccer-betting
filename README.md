## 📊 Data File
Download the Excel spreadsheet [here](./out.xlsx).

How to read the spreadsheet:
<table>
  <thead>
    <tr>
      <th>Date</th>
      <th>League</th>
      <th>Game</th>
      <th>Model Home</th>
      <th>Model Draw</th>
      <th>Model Away</th>
      <th>Book Home</th>
      <th>Book Draw</th>
      <th>Book Away</th>
      <th>Prediction</th>
      <th>Result</th>
      <th>Bet Size</th>
      <th>Payout</th>
      <th>Cum Sum</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>08/31/2025</td>
      <td>mls</td>
      <td>Sporting Kansas City vs Colorado Rapids</td>
      <td>0.25</td>
      <td>0.251</td>
      <td><b>0.499</b></td>
      <td>0.481</td>
      <td>0.234</td>
      <td><b>0.321</b></td>
      <td style="background-color:#ff6666; color:white"><b>Away</b></td>
      <td>4-2</td>
      <td>1</td>
      <td>-1</td>
      <td>1396.944</td>
    </tr>
    <tr>
      <td>08/31/2025</td>
      <td>mls</td>
      <td>Minnesota United vs Portland Timbers</td>
      <td>0.549</td>
      <td><b>0.347</b></td>
      <td>0.104</td>
      <td>0.559</td>
      <td><b>0.24</b></td>
      <td>0.235</td>
      <td style="background-color:#33cc33; color:white"><b>Draw</b></td>
      <td>1-1</td>
      <td>1</td>
      <td>3.167</td>
      <td>1400.111</td>
    </tr>
  </tbody>
</table>

Model Home, Model Draw, Model Away columns show the predicted odds for the given match by the betting model. Book Home, Book Draw, and Book Away columns show the odds implied by the sportsbook. All sportsbook odds imply a probability. +100 is 50%, +300 is 25%, -300 is 75%, etc. We convert the odds into probabilities to compare them with the odds given by the model. If the model odds for a match outcome are significantly higher than the implied odds ("significantly higher" according to parameters learned by the model), we make the bet.

In the first row, the model provided a 49.9% probability of Colorado beating Kansas City, while the book odds were only 32.1%, so we made the bet. In this case, the game actually ended with a Kansas City win, so we lose the bet. Therefore the payout is -1.

In the second row, the model provided a 34.7% probability of a draw between Minnesota and Portland, while the book odds were only 24%. In this case, the game indeed ended in a 1-1 draw, so we win the bet, and our payout is given by (1 / 0.24) - 1 = 3.167.

The model has been trained on historical data availble at https://www.football-data.co.uk/. Over a long time horizon, following the procedure above should yield positive returns. In testing over data starting on 8/25/12 and extending to the present day, the model achieved a profit of +1318.669 "units" after 11192 bets, a ROI of 11.78%. Extensive measures have been taken to validate the model and prevent overfitting. As of 6/26/25 I have been betting real money following the predictions. Therefore in the Excel sheet there is a tab which tracks returns since 6/26/25. Fingers crossed for a profitable season.


## Time-Window Summary

| Window | Date Range | Profit | Num Bets | ROI |
|----------------|---------------------|--------|----------|-------|
| Last 30 Days | 10/12/2025 - 11/10/2025 | +3.753 | 71 | 5.29% |
| Last 3 Months | 08/13/2025 - 11/10/2025 | +16.788 | 210 | 7.99% |
| Last 6 Months | 05/15/2025 - 11/10/2025 | +29.428 | 411 | 7.16% |
| YTD | 01/01/2025 - 11/10/2025 | +93.105 | 752 | 12.38% |
| Last 52 Weeks | 11/11/2024 - 11/10/2025 | +121.325 | 838 | 14.48% |
| All Time | 08/25/2012 - 11/10/2025 | +1318.669 | 11192 | 11.78% |

## Weekly Results (Last 52 Weeks)

| Date Range | Profit | Num Bets | ROI | Total Profit | Total Num Bets | Total ROI |
|---------------------|--------|----------|-------|--------------|----------------|-----------|
| 11/12/2024 - 11/18/2024 | +6.411 | 2 | 320.55% | +6.411 | 2 | 320.55% |
| 11/19/2024 - 11/25/2024 | -3.028 | 18 | -16.82% | +3.383 | 20 | 16.91% |
| 11/26/2024 - 12/02/2024 | -2.323 | 11 | -21.12% | +1.060 | 31 | 3.42% |
| 12/03/2024 - 12/09/2024 | +8.292 | 25 | 33.17% | +9.352 | 56 | 16.70% |
| 12/10/2024 - 12/16/2024 | +21.105 | 14 | 150.75% | +30.457 | 70 | 43.51% |
| 12/17/2024 - 12/23/2024 | -0.388 | 6 | -6.47% | +30.069 | 76 | 39.56% |
| 12/24/2024 - 12/30/2024 | -0.849 | 9 | -9.43% | +29.220 | 85 | 34.38% |
| 12/31/2024 - 01/06/2025 | +9.088 | 6 | 151.47% | +38.308 | 91 | 42.10% |
| 01/07/2025 - 01/13/2025 | -6.000 | 6 | -100.00% | +32.308 | 97 | 33.31% |
| 01/14/2025 - 01/20/2025 | -0.185 | 10 | -1.85% | +32.123 | 107 | 30.02% |
| 01/21/2025 - 01/27/2025 | -5.430 | 7 | -77.57% | +26.693 | 114 | 23.41% |
| 01/28/2025 - 02/03/2025 | +17.643 | 17 | 103.78% | +44.336 | 131 | 33.84% |
| 02/04/2025 - 02/10/2025 | -5.633 | 10 | -56.33% | +38.703 | 141 | 27.45% |
| 02/11/2025 - 02/17/2025 | +8.355 | 9 | 92.83% | +47.058 | 150 | 31.37% |
| 02/18/2025 - 02/24/2025 | -1.024 | 10 | -10.24% | +46.034 | 160 | 28.77% |
| 02/25/2025 - 03/03/2025 | -5.409 | 13 | -41.61% | +40.625 | 173 | 23.48% |
| 03/04/2025 - 03/10/2025 | +15.387 | 11 | 139.88% | +56.012 | 184 | 30.44% |
| 03/11/2025 - 03/17/2025 | +11.848 | 26 | 45.57% | +67.860 | 210 | 32.31% |
| 03/18/2025 - 03/24/2025 | -2.552 | 6 | -42.53% | +65.308 | 216 | 30.24% |
| 03/25/2025 - 03/31/2025 | -4.182 | 22 | -19.01% | +61.126 | 238 | 25.68% |
| 04/01/2025 - 04/07/2025 | +5.613 | 28 | 20.05% | +66.739 | 266 | 25.09% |
| 04/08/2025 - 04/14/2025 | +0.023 | 33 | 0.07% | +66.762 | 299 | 22.33% |
| 04/15/2025 - 04/21/2025 | +5.021 | 26 | 19.31% | +71.783 | 325 | 22.09% |
| 04/22/2025 - 04/28/2025 | +11.329 | 32 | 35.40% | +83.112 | 357 | 23.28% |
| 04/29/2025 - 05/05/2025 | +1.368 | 34 | 4.02% | +84.480 | 391 | 21.61% |
| 05/06/2025 - 05/12/2025 | +9.387 | 29 | 32.37% | +93.867 | 420 | 22.35% |
| 05/13/2025 - 05/19/2025 | +18.339 | 37 | 49.56% | +112.206 | 457 | 24.55% |
| 05/20/2025 - 05/26/2025 | +11.031 | 23 | 47.96% | +123.237 | 480 | 25.67% |
| 05/27/2025 - 06/02/2025 | +4.534 | 23 | 19.71% | +127.771 | 503 | 25.40% |
| 06/03/2025 - 06/09/2025 | +1.803 | 5 | 36.06% | +129.574 | 508 | 25.51% |
| 06/10/2025 - 06/16/2025 | -0.870 | 8 | -10.88% | +128.704 | 516 | 24.94% |
| 06/17/2025 - 06/23/2025 | +0.000 | 0 | 0.00% | +128.704 | 516 | 24.94% |
| 06/24/2025 - 06/30/2025 | -5.724 | 21 | -27.26% | +122.980 | 537 | 22.90% |
| 07/01/2025 - 07/07/2025 | -5.563 | 14 | -39.74% | +117.417 | 551 | 21.31% |
| 07/08/2025 - 07/14/2025 | -4.340 | 13 | -33.38% | +113.077 | 564 | 20.05% |
| 07/15/2025 - 07/21/2025 | -0.720 | 22 | -3.27% | +112.357 | 586 | 19.17% |
| 07/22/2025 - 07/28/2025 | -10.077 | 17 | -59.28% | +102.280 | 603 | 16.96% |
| 07/29/2025 - 08/04/2025 | -5.000 | 5 | -100.00% | +97.280 | 608 | 16.00% |
| 08/05/2025 - 08/11/2025 | +8.257 | 19 | 43.46% | +105.537 | 627 | 16.83% |
| 08/12/2025 - 08/18/2025 | -2.617 | 17 | -15.39% | +102.920 | 644 | 15.98% |
| 08/19/2025 - 08/25/2025 | +12.967 | 18 | 72.04% | +115.887 | 662 | 17.51% |
| 08/26/2025 - 09/01/2025 | +3.475 | 17 | 20.44% | +119.362 | 679 | 17.58% |
| 09/02/2025 - 09/08/2025 | +2.049 | 2 | 102.45% | +121.411 | 681 | 17.83% |
| 09/09/2025 - 09/15/2025 | +6.526 | 15 | 43.51% | +127.937 | 696 | 18.38% |
| 09/16/2025 - 09/22/2025 | -5.921 | 20 | -29.61% | +122.016 | 716 | 17.04% |
| 09/23/2025 - 09/29/2025 | +0.209 | 23 | 0.91% | +122.225 | 739 | 16.54% |
| 09/30/2025 - 10/06/2025 | -4.185 | 25 | -16.74% | +118.040 | 764 | 15.45% |
| 10/07/2025 - 10/13/2025 | +0.532 | 2 | 26.60% | +118.572 | 766 | 15.48% |
| 10/14/2025 - 10/20/2025 | -3.115 | 19 | -16.39% | +115.457 | 785 | 14.71% |
| 10/21/2025 - 10/27/2025 | +10.748 | 16 | 67.18% | +126.205 | 801 | 15.76% |
| 10/28/2025 - 11/03/2025 | -7.111 | 19 | -37.43% | +119.094 | 820 | 14.52% |
| 11/04/2025 - 11/10/2025 | +3.231 | 17 | 19.01% | +122.325 | 837 | 14.61% |