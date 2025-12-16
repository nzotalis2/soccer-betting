## 📊 Data File
Download the Excel spreadsheet [here](./out_excel.xlsx).

## Time-Window Summary

| Window | Date Range | Profit | Num Bets | ROI |
|----------------|---------------------|--------|----------|-------|
| Last 30 Days | 11/16/2025 - 12/15/2025 | -7.817 | 52 | -15.03% |
| Last 3 Months | 09/17/2025 - 12/15/2025 | -12.429 | 192 | -6.47% |
| Last 6 Months | 06/19/2025 - 12/15/2025 | -14.196 | 373 | -3.81% |
| YTD | 01/01/2025 - 12/15/2025 | +85.288 | 804 | 10.61% |
| Last 52 Weeks | 12/16/2024 - 12/15/2025 | +84.152 | 821 | 10.25% |
| All Time | 08/25/2012 - 12/15/2025 | +1310.852 | 11244 | 11.66% |

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
| 12/17/2024 - 12/23/2024 | -0.388 | 6 | -6.47% | -0.388 | 6 | -6.47% |
| 12/24/2024 - 12/30/2024 | -0.849 | 9 | -9.43% | -1.237 | 15 | -8.25% |
| 12/31/2024 - 01/06/2025 | +9.088 | 6 | 151.47% | +7.851 | 21 | 37.39% |
| 01/07/2025 - 01/13/2025 | -6.000 | 6 | -100.00% | +1.851 | 27 | 6.86% |
| 01/14/2025 - 01/20/2025 | -0.185 | 10 | -1.85% | +1.666 | 37 | 4.50% |
| 01/21/2025 - 01/27/2025 | -5.430 | 7 | -77.57% | -3.764 | 44 | -8.55% |
| 01/28/2025 - 02/03/2025 | +17.643 | 17 | 103.78% | +13.879 | 61 | 22.75% |
| 02/04/2025 - 02/10/2025 | -5.633 | 10 | -56.33% | +8.246 | 71 | 11.61% |
| 02/11/2025 - 02/17/2025 | +8.355 | 9 | 92.83% | +16.601 | 80 | 20.75% |
| 02/18/2025 - 02/24/2025 | -1.024 | 10 | -10.24% | +15.577 | 90 | 17.31% |
| 02/25/2025 - 03/03/2025 | -5.409 | 13 | -41.61% | +10.168 | 103 | 9.87% |
| 03/04/2025 - 03/10/2025 | +15.387 | 11 | 139.88% | +25.555 | 114 | 22.42% |
| 03/11/2025 - 03/17/2025 | +11.848 | 26 | 45.57% | +37.403 | 140 | 26.72% |
| 03/18/2025 - 03/24/2025 | -2.552 | 6 | -42.53% | +34.851 | 146 | 23.87% |
| 03/25/2025 - 03/31/2025 | -4.182 | 22 | -19.01% | +30.669 | 168 | 18.26% |
| 04/01/2025 - 04/07/2025 | +5.613 | 28 | 20.05% | +36.282 | 196 | 18.51% |
| 04/08/2025 - 04/14/2025 | +0.023 | 33 | 0.07% | +36.305 | 229 | 15.85% |
| 04/15/2025 - 04/21/2025 | +5.021 | 26 | 19.31% | +41.326 | 255 | 16.21% |
| 04/22/2025 - 04/28/2025 | +11.329 | 32 | 35.40% | +52.655 | 287 | 18.35% |
| 04/29/2025 - 05/05/2025 | +1.368 | 34 | 4.02% | +54.023 | 321 | 16.83% |
| 05/06/2025 - 05/12/2025 | +9.387 | 29 | 32.37% | +63.410 | 350 | 18.12% |
| 05/13/2025 - 05/19/2025 | +18.339 | 37 | 49.56% | +81.749 | 387 | 21.12% |
| 05/20/2025 - 05/26/2025 | +11.031 | 23 | 47.96% | +92.780 | 410 | 22.63% |
| 05/27/2025 - 06/02/2025 | +4.534 | 23 | 19.71% | +97.314 | 433 | 22.47% |
| 06/03/2025 - 06/09/2025 | +1.803 | 5 | 36.06% | +99.117 | 438 | 22.63% |
| 06/10/2025 - 06/16/2025 | -0.870 | 8 | -10.88% | +98.247 | 446 | 22.03% |
| 06/17/2025 - 06/23/2025 | +0.000 | 0 | 0.00% | +98.247 | 446 | 22.03% |
| 06/24/2025 - 06/30/2025 | -5.724 | 21 | -27.26% | +92.523 | 467 | 19.81% |
| 07/01/2025 - 07/07/2025 | -5.563 | 14 | -39.74% | +86.960 | 481 | 18.08% |
| 07/08/2025 - 07/14/2025 | -4.340 | 13 | -33.38% | +82.620 | 494 | 16.72% |
| 07/15/2025 - 07/21/2025 | -0.720 | 22 | -3.27% | +81.900 | 516 | 15.87% |
| 07/22/2025 - 07/28/2025 | -10.077 | 17 | -59.28% | +71.823 | 533 | 13.48% |
| 07/29/2025 - 08/04/2025 | -5.000 | 5 | -100.00% | +66.823 | 538 | 12.42% |
| 08/05/2025 - 08/11/2025 | +8.257 | 19 | 43.46% | +75.080 | 557 | 13.48% |
| 08/12/2025 - 08/18/2025 | -2.617 | 17 | -15.39% | +72.463 | 574 | 12.62% |
| 08/19/2025 - 08/25/2025 | +12.967 | 18 | 72.04% | +85.430 | 592 | 14.43% |
| 08/26/2025 - 09/01/2025 | +3.475 | 17 | 20.44% | +88.905 | 609 | 14.60% |
| 09/02/2025 - 09/08/2025 | +2.049 | 2 | 102.45% | +90.954 | 611 | 14.89% |
| 09/09/2025 - 09/15/2025 | +6.526 | 15 | 43.51% | +97.480 | 626 | 15.57% |
| 09/16/2025 - 09/22/2025 | -5.921 | 20 | -29.61% | +91.559 | 646 | 14.17% |
| 09/23/2025 - 09/29/2025 | +0.209 | 23 | 0.91% | +91.768 | 669 | 13.72% |
| 09/30/2025 - 10/06/2025 | -4.185 | 25 | -16.74% | +87.583 | 694 | 12.62% |
| 10/07/2025 - 10/13/2025 | +0.532 | 2 | 26.60% | +88.115 | 696 | 12.66% |
| 10/14/2025 - 10/20/2025 | -3.115 | 19 | -16.39% | +85.000 | 715 | 11.89% |
| 10/21/2025 - 10/27/2025 | +10.748 | 16 | 67.18% | +95.748 | 731 | 13.10% |
| 10/28/2025 - 11/03/2025 | -7.111 | 19 | -37.43% | +88.637 | 750 | 11.82% |
| 11/04/2025 - 11/10/2025 | +3.231 | 17 | 19.01% | +91.868 | 767 | 11.98% |
| 11/11/2025 - 11/17/2025 | -1.000 | 1 | -100.00% | +90.868 | 768 | 11.83% |
| 11/18/2025 - 11/24/2025 | -5.618 | 10 | -56.18% | +85.250 | 778 | 10.96% |
| 11/25/2025 - 12/01/2025 | -12.249 | 14 | -87.49% | +73.001 | 792 | 9.22% |
| 12/02/2025 - 12/08/2025 | +1.198 | 19 | 6.31% | +74.199 | 811 | 9.15% |
| 12/09/2025 - 12/15/2025 | +9.852 | 8 | 123.15% | +84.051 | 819 | 10.26% |