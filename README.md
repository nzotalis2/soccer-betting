## 📊 Data File
Download the Excel spreadsheet [here](./out_excel.xlsx).

## Time-Window Summary

| Window | Date Range | Profit | Num Bets | ROI |
|----------------|---------------------|--------|----------|-------|
| Last 30 Days | 12/14/2025 - 01/12/2026 | +5.985 | 32 | 18.70% |
| Last 3 Months | 10/15/2025 - 01/12/2026 | -6.831 | 155 | -4.41% |
| Last 6 Months | 07/17/2025 - 01/12/2026 | -11.294 | 367 | -3.08% |
| YTD | 01/01/2026 - 01/12/2026 | +0.730 | 13 | 5.62% |
| Last 52 Weeks | 01/13/2025 - 01/12/2026 | +70.181 | 834 | 8.41% |
| All Time | 03/24/2013 - 01/12/2026 | +1315.483 | 11247 | 11.70% |

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
| 01/14/2025 - 01/20/2025 | -0.185 | 10 | -1.85% | -0.185 | 10 | -1.85% |
| 01/21/2025 - 01/27/2025 | -5.430 | 7 | -77.57% | -5.615 | 17 | -33.03% |
| 01/28/2025 - 02/03/2025 | +17.643 | 17 | 103.78% | +12.028 | 34 | 35.38% |
| 02/04/2025 - 02/10/2025 | -5.633 | 10 | -56.33% | +6.395 | 44 | 14.53% |
| 02/11/2025 - 02/17/2025 | +8.355 | 9 | 92.83% | +14.750 | 53 | 27.83% |
| 02/18/2025 - 02/24/2025 | -2.175 | 9 | -24.17% | +12.575 | 62 | 20.28% |
| 02/25/2025 - 03/03/2025 | -5.409 | 13 | -41.61% | +7.166 | 75 | 9.55% |
| 03/04/2025 - 03/10/2025 | +15.387 | 11 | 139.88% | +22.553 | 86 | 26.22% |
| 03/11/2025 - 03/17/2025 | +11.848 | 26 | 45.57% | +34.401 | 112 | 30.72% |
| 03/18/2025 - 03/24/2025 | -2.552 | 6 | -42.53% | +31.849 | 118 | 26.99% |
| 03/25/2025 - 03/31/2025 | -4.182 | 22 | -19.01% | +27.667 | 140 | 19.76% |
| 04/01/2025 - 04/07/2025 | +5.613 | 28 | 20.05% | +33.280 | 168 | 19.81% |
| 04/08/2025 - 04/14/2025 | +0.023 | 33 | 0.07% | +33.303 | 201 | 16.57% |
| 04/15/2025 - 04/21/2025 | +5.021 | 26 | 19.31% | +38.324 | 227 | 16.88% |
| 04/22/2025 - 04/28/2025 | +11.329 | 32 | 35.40% | +49.653 | 259 | 19.17% |
| 04/29/2025 - 05/05/2025 | +1.368 | 34 | 4.02% | +51.021 | 293 | 17.41% |
| 05/06/2025 - 05/12/2025 | +9.387 | 29 | 32.37% | +60.408 | 322 | 18.76% |
| 05/13/2025 - 05/19/2025 | +18.339 | 37 | 49.56% | +78.747 | 359 | 21.94% |
| 05/20/2025 - 05/26/2025 | +11.031 | 23 | 47.96% | +89.778 | 382 | 23.50% |
| 05/27/2025 - 06/02/2025 | +4.534 | 23 | 19.71% | +94.312 | 405 | 23.29% |
| 06/03/2025 - 06/09/2025 | +1.803 | 5 | 36.06% | +96.115 | 410 | 23.44% |
| 06/10/2025 - 06/16/2025 | -0.870 | 8 | -10.88% | +95.245 | 418 | 22.79% |
| 06/17/2025 - 06/23/2025 | +0.000 | 0 | 0.00% | +95.245 | 418 | 22.79% |
| 06/24/2025 - 06/30/2025 | -5.724 | 21 | -27.26% | +89.521 | 439 | 20.39% |
| 07/01/2025 - 07/07/2025 | -5.563 | 14 | -39.74% | +83.958 | 453 | 18.53% |
| 07/08/2025 - 07/14/2025 | -4.340 | 13 | -33.38% | +79.618 | 466 | 17.09% |
| 07/15/2025 - 07/21/2025 | -0.720 | 22 | -3.27% | +78.898 | 488 | 16.17% |
| 07/22/2025 - 07/28/2025 | -10.077 | 17 | -59.28% | +68.821 | 505 | 13.63% |
| 07/29/2025 - 08/04/2025 | -5.000 | 5 | -100.00% | +63.821 | 510 | 12.51% |
| 08/05/2025 - 08/11/2025 | +8.257 | 19 | 43.46% | +72.078 | 529 | 13.63% |
| 08/12/2025 - 08/18/2025 | -2.617 | 17 | -15.39% | +69.461 | 546 | 12.72% |
| 08/19/2025 - 08/25/2025 | +11.866 | 22 | 53.94% | +81.327 | 568 | 14.32% |
| 08/26/2025 - 09/01/2025 | +2.475 | 18 | 13.75% | +83.802 | 586 | 14.30% |
| 09/02/2025 - 09/08/2025 | +2.049 | 2 | 102.45% | +85.851 | 588 | 14.60% |
| 09/09/2025 - 09/15/2025 | +4.526 | 17 | 26.62% | +90.377 | 605 | 14.94% |
| 09/16/2025 - 09/22/2025 | -5.921 | 20 | -29.61% | +84.456 | 625 | 13.51% |
| 09/23/2025 - 09/29/2025 | -1.791 | 25 | -7.16% | +82.665 | 650 | 12.72% |
| 09/30/2025 - 10/06/2025 | -5.185 | 26 | -19.94% | +77.480 | 676 | 11.46% |
| 10/07/2025 - 10/13/2025 | -0.468 | 3 | -15.60% | +77.012 | 679 | 11.34% |
| 10/14/2025 - 10/20/2025 | -3.115 | 19 | -16.39% | +73.897 | 698 | 10.59% |
| 10/21/2025 - 10/27/2025 | +9.748 | 17 | 57.34% | +83.645 | 715 | 11.70% |
| 10/28/2025 - 11/03/2025 | -4.811 | 20 | -24.05% | +78.834 | 735 | 10.73% |
| 11/04/2025 - 11/10/2025 | +5.531 | 18 | 30.73% | +84.365 | 753 | 11.20% |
| 11/11/2025 - 11/17/2025 | -1.000 | 1 | -100.00% | +83.365 | 754 | 11.06% |
| 11/18/2025 - 11/24/2025 | -5.618 | 10 | -56.18% | +77.747 | 764 | 10.18% |
| 11/25/2025 - 12/01/2025 | -12.249 | 14 | -87.49% | +65.498 | 778 | 8.42% |
| 12/02/2025 - 12/08/2025 | +1.198 | 19 | 6.31% | +66.696 | 797 | 8.37% |
| 12/09/2025 - 12/15/2025 | +7.852 | 10 | 78.52% | +74.548 | 807 | 9.24% |
| 12/16/2025 - 12/22/2025 | -0.097 | 9 | -1.08% | +74.451 | 816 | 9.12% |
| 12/23/2025 - 12/29/2025 | -5.000 | 5 | -100.00% | +69.451 | 821 | 8.46% |
| 12/30/2025 - 01/05/2026 | +4.827 | 5 | 96.54% | +74.278 | 826 | 8.99% |
| 01/06/2026 - 01/12/2026 | -4.097 | 8 | -51.21% | +70.181 | 834 | 8.41% |