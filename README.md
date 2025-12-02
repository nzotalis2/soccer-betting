## 📊 Data File
Download the Excel spreadsheet [here](./out_excel.xlsx).

## Time-Window Summary

| Window | Date Range | Profit | Num Bets | ROI |
|----------------|---------------------|--------|----------|-------|
| Last 30 Days | 11/02/2025 - 12/01/2025 | -15.372 | 47 | -32.71% |
| Last 3 Months | 09/03/2025 - 12/01/2025 | -15.904 | 183 | -8.69% |
| Last 6 Months | 06/05/2025 - 12/01/2025 | -24.313 | 359 | -6.77% |
| YTD | 01/01/2025 - 12/01/2025 | +74.238 | 777 | 9.55% |
| Last 52 Weeks | 12/02/2024 - 12/01/2025 | +102.398 | 831 | 12.32% |
| All Time | 08/25/2012 - 12/01/2025 | +1299.802 | 11217 | 11.59% |

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



## Weekly Results (Last 52 Weeks)

| Date Range | Profit | Num Bets | ROI | Total Profit | Total Num Bets | Total ROI |
|---------------------|--------|----------|-------|--------------|----------------|-----------|
| 12/03/2024 - 12/09/2024 | +8.292 | 25 | 33.17% | +8.292 | 25 | 33.17% |
| 12/10/2024 - 12/16/2024 | +21.105 | 14 | 150.75% | +29.397 | 39 | 75.38% |
| 12/17/2024 - 12/23/2024 | -0.388 | 6 | -6.47% | +29.009 | 45 | 64.46% |
| 12/24/2024 - 12/30/2024 | -0.849 | 9 | -9.43% | +28.160 | 54 | 52.15% |
| 12/31/2024 - 01/06/2025 | +9.088 | 6 | 151.47% | +37.248 | 60 | 62.08% |
| 01/07/2025 - 01/13/2025 | -6.000 | 6 | -100.00% | +31.248 | 66 | 47.35% |
| 01/14/2025 - 01/20/2025 | -0.185 | 10 | -1.85% | +31.063 | 76 | 40.87% |
| 01/21/2025 - 01/27/2025 | -5.430 | 7 | -77.57% | +25.633 | 83 | 30.88% |
| 01/28/2025 - 02/03/2025 | +17.643 | 17 | 103.78% | +43.276 | 100 | 43.28% |
| 02/04/2025 - 02/10/2025 | -5.633 | 10 | -56.33% | +37.643 | 110 | 34.22% |
| 02/11/2025 - 02/17/2025 | +8.355 | 9 | 92.83% | +45.998 | 119 | 38.65% |
| 02/18/2025 - 02/24/2025 | -1.024 | 10 | -10.24% | +44.974 | 129 | 34.86% |
| 02/25/2025 - 03/03/2025 | -5.409 | 13 | -41.61% | +39.565 | 142 | 27.86% |
| 03/04/2025 - 03/10/2025 | +15.387 | 11 | 139.88% | +54.952 | 153 | 35.92% |
| 03/11/2025 - 03/17/2025 | +11.848 | 26 | 45.57% | +66.800 | 179 | 37.32% |
| 03/18/2025 - 03/24/2025 | -2.552 | 6 | -42.53% | +64.248 | 185 | 34.73% |
| 03/25/2025 - 03/31/2025 | -4.182 | 22 | -19.01% | +60.066 | 207 | 29.02% |
| 04/01/2025 - 04/07/2025 | +5.613 | 28 | 20.05% | +65.679 | 235 | 27.95% |
| 04/08/2025 - 04/14/2025 | +0.023 | 33 | 0.07% | +65.702 | 268 | 24.52% |
| 04/15/2025 - 04/21/2025 | +5.021 | 26 | 19.31% | +70.723 | 294 | 24.06% |
| 04/22/2025 - 04/28/2025 | +11.329 | 32 | 35.40% | +82.052 | 326 | 25.17% |
| 04/29/2025 - 05/05/2025 | +1.368 | 34 | 4.02% | +83.420 | 360 | 23.17% |
| 05/06/2025 - 05/12/2025 | +9.387 | 29 | 32.37% | +92.807 | 389 | 23.86% |
| 05/13/2025 - 05/19/2025 | +18.339 | 37 | 49.56% | +111.146 | 426 | 26.09% |
| 05/20/2025 - 05/26/2025 | +11.031 | 23 | 47.96% | +122.177 | 449 | 27.21% |
| 05/27/2025 - 06/02/2025 | +4.534 | 23 | 19.71% | +126.711 | 472 | 26.85% |
| 06/03/2025 - 06/09/2025 | +1.803 | 5 | 36.06% | +128.514 | 477 | 26.94% |
| 06/10/2025 - 06/16/2025 | -0.870 | 8 | -10.88% | +127.644 | 485 | 26.32% |
| 06/17/2025 - 06/23/2025 | +0.000 | 0 | 0.00% | +127.644 | 485 | 26.32% |
| 06/24/2025 - 06/30/2025 | -5.724 | 21 | -27.26% | +121.920 | 506 | 24.09% |
| 07/01/2025 - 07/07/2025 | -5.563 | 14 | -39.74% | +116.357 | 520 | 22.38% |
| 07/08/2025 - 07/14/2025 | -4.340 | 13 | -33.38% | +112.017 | 533 | 21.02% |
| 07/15/2025 - 07/21/2025 | -0.720 | 22 | -3.27% | +111.297 | 555 | 20.05% |
| 07/22/2025 - 07/28/2025 | -10.077 | 17 | -59.28% | +101.220 | 572 | 17.70% |
| 07/29/2025 - 08/04/2025 | -5.000 | 5 | -100.00% | +96.220 | 577 | 16.68% |
| 08/05/2025 - 08/11/2025 | +8.257 | 19 | 43.46% | +104.477 | 596 | 17.53% |
| 08/12/2025 - 08/18/2025 | -2.617 | 17 | -15.39% | +101.860 | 613 | 16.62% |
| 08/19/2025 - 08/25/2025 | +12.967 | 18 | 72.04% | +114.827 | 631 | 18.20% |
| 08/26/2025 - 09/01/2025 | +3.475 | 17 | 20.44% | +118.302 | 648 | 18.26% |
| 09/02/2025 - 09/08/2025 | +2.049 | 2 | 102.45% | +120.351 | 650 | 18.52% |
| 09/09/2025 - 09/15/2025 | +6.526 | 15 | 43.51% | +126.877 | 665 | 19.08% |
| 09/16/2025 - 09/22/2025 | -5.921 | 20 | -29.61% | +120.956 | 685 | 17.66% |
| 09/23/2025 - 09/29/2025 | +0.209 | 23 | 0.91% | +121.165 | 708 | 17.11% |
| 09/30/2025 - 10/06/2025 | -4.185 | 25 | -16.74% | +116.980 | 733 | 15.96% |
| 10/07/2025 - 10/13/2025 | +0.532 | 2 | 26.60% | +117.512 | 735 | 15.99% |
| 10/14/2025 - 10/20/2025 | -3.115 | 19 | -16.39% | +114.397 | 754 | 15.17% |
| 10/21/2025 - 10/27/2025 | +10.748 | 16 | 67.17% | +125.145 | 770 | 16.25% |
| 10/28/2025 - 11/03/2025 | -7.111 | 19 | -37.43% | +118.034 | 789 | 14.96% |
| 11/04/2025 - 11/10/2025 | +3.231 | 17 | 19.01% | +121.265 | 806 | 15.05% |
| 11/11/2025 - 11/17/2025 | -1.000 | 1 | -100.00% | +120.265 | 807 | 14.90% |
| 11/18/2025 - 11/24/2025 | -5.618 | 10 | -56.18% | +114.647 | 817 | 14.03% |
| 11/25/2025 - 12/01/2025 | -12.249 | 14 | -87.49% | +102.398 | 831 | 12.32% |