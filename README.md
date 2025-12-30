## 📊 Data File
Download the Excel spreadsheet [here](./out_excel.xlsx).

## Time-Window Summary

| Window | Date Range | Profit | Num Bets | ROI |
|----------------|---------------------|--------|----------|-------|
| Last 30 Days | 11/30/2025 - 12/29/2025 | -5.296 | 54 | -9.81% |
| Last 3 Months | 10/01/2025 - 12/29/2025 | -13.214 | 171 | -7.73% |
| Last 6 Months | 07/03/2025 - 12/29/2025 | -19.070 | 381 | -5.01% |
| YTD | 01/01/2025 - 12/29/2025 | +72.539 | 833 | 8.71% |
| Last 52 Weeks | 12/30/2024 - 12/29/2025 | +72.539 | 833 | 8.71% |
| All Time | 03/24/2013 - 12/29/2025 | +1314.753 | 11234 | 11.70% |

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
| 12/31/2024 - 01/06/2025 | +9.088 | 6 | 151.47% | +9.088 | 6 | 151.47% |
| 01/07/2025 - 01/13/2025 | -6.000 | 6 | -100.00% | +3.088 | 12 | 25.73% |
| 01/14/2025 - 01/20/2025 | -0.185 | 10 | -1.85% | +2.903 | 22 | 13.20% |
| 01/21/2025 - 01/27/2025 | -5.430 | 7 | -77.57% | -2.527 | 29 | -8.71% |
| 01/28/2025 - 02/03/2025 | +17.643 | 17 | 103.78% | +15.116 | 46 | 32.86% |
| 02/04/2025 - 02/10/2025 | -5.633 | 10 | -56.33% | +9.483 | 56 | 16.93% |
| 02/11/2025 - 02/17/2025 | +8.355 | 9 | 92.83% | +17.838 | 65 | 27.44% |
| 02/18/2025 - 02/24/2025 | -2.175 | 9 | -24.17% | +15.663 | 74 | 21.17% |
| 02/25/2025 - 03/03/2025 | -5.409 | 13 | -41.61% | +10.254 | 87 | 11.79% |
| 03/04/2025 - 03/10/2025 | +15.387 | 11 | 139.88% | +25.641 | 98 | 26.16% |
| 03/11/2025 - 03/17/2025 | +11.848 | 26 | 45.57% | +37.489 | 124 | 30.23% |
| 03/18/2025 - 03/24/2025 | -2.552 | 6 | -42.53% | +34.937 | 130 | 26.87% |
| 03/25/2025 - 03/31/2025 | -4.182 | 22 | -19.01% | +30.755 | 152 | 20.23% |
| 04/01/2025 - 04/07/2025 | +5.613 | 28 | 20.05% | +36.368 | 180 | 20.20% |
| 04/08/2025 - 04/14/2025 | +0.023 | 33 | 0.07% | +36.391 | 213 | 17.08% |
| 04/15/2025 - 04/21/2025 | +5.021 | 26 | 19.31% | +41.412 | 239 | 17.33% |
| 04/22/2025 - 04/28/2025 | +11.329 | 32 | 35.40% | +52.741 | 271 | 19.46% |
| 04/29/2025 - 05/05/2025 | +1.368 | 34 | 4.02% | +54.109 | 305 | 17.74% |
| 05/06/2025 - 05/12/2025 | +9.387 | 29 | 32.37% | +63.496 | 334 | 19.01% |
| 05/13/2025 - 05/19/2025 | +18.339 | 37 | 49.56% | +81.835 | 371 | 22.06% |
| 05/20/2025 - 05/26/2025 | +11.031 | 23 | 47.96% | +92.866 | 394 | 23.57% |
| 05/27/2025 - 06/02/2025 | +4.534 | 23 | 19.71% | +97.400 | 417 | 23.36% |
| 06/03/2025 - 06/09/2025 | +1.803 | 5 | 36.06% | +99.203 | 422 | 23.51% |
| 06/10/2025 - 06/16/2025 | -0.870 | 8 | -10.87% | +98.333 | 430 | 22.87% |
| 06/17/2025 - 06/23/2025 | +0.000 | 0 | 0.00% | +98.333 | 430 | 22.87% |
| 06/24/2025 - 06/30/2025 | -5.724 | 21 | -27.26% | +92.609 | 451 | 20.53% |
| 07/01/2025 - 07/07/2025 | -5.563 | 14 | -39.74% | +87.046 | 465 | 18.72% |
| 07/08/2025 - 07/14/2025 | -4.340 | 13 | -33.38% | +82.706 | 478 | 17.30% |
| 07/15/2025 - 07/21/2025 | -0.720 | 22 | -3.27% | +81.986 | 500 | 16.40% |
| 07/22/2025 - 07/28/2025 | -10.077 | 17 | -59.28% | +71.909 | 517 | 13.91% |
| 07/29/2025 - 08/04/2025 | -5.000 | 5 | -100.00% | +66.909 | 522 | 12.82% |
| 08/05/2025 - 08/11/2025 | +8.257 | 19 | 43.46% | +75.166 | 541 | 13.89% |
| 08/12/2025 - 08/18/2025 | -2.617 | 17 | -15.39% | +72.549 | 558 | 13.00% |
| 08/19/2025 - 08/25/2025 | +11.866 | 22 | 53.94% | +84.415 | 580 | 14.55% |
| 08/26/2025 - 09/01/2025 | +2.475 | 18 | 13.75% | +86.890 | 598 | 14.53% |
| 09/02/2025 - 09/08/2025 | +2.049 | 2 | 102.45% | +88.939 | 600 | 14.82% |
| 09/09/2025 - 09/15/2025 | +4.526 | 17 | 26.62% | +93.465 | 617 | 15.15% |
| 09/16/2025 - 09/22/2025 | -5.921 | 20 | -29.61% | +87.544 | 637 | 13.74% |
| 09/23/2025 - 09/29/2025 | -1.791 | 25 | -7.16% | +85.753 | 662 | 12.95% |
| 09/30/2025 - 10/06/2025 | -5.185 | 26 | -19.94% | +80.568 | 688 | 11.71% |
| 10/07/2025 - 10/13/2025 | -0.468 | 3 | -15.60% | +80.100 | 691 | 11.59% |
| 10/14/2025 - 10/20/2025 | -3.115 | 19 | -16.39% | +76.985 | 710 | 10.84% |
| 10/21/2025 - 10/27/2025 | +9.748 | 17 | 57.34% | +86.733 | 727 | 11.93% |
| 10/28/2025 - 11/03/2025 | -4.811 | 20 | -24.05% | +81.922 | 747 | 10.97% |
| 11/04/2025 - 11/10/2025 | +5.531 | 18 | 30.73% | +87.453 | 765 | 11.43% |
| 11/11/2025 - 11/17/2025 | -1.000 | 1 | -100.00% | +86.453 | 766 | 11.29% |
| 11/18/2025 - 11/24/2025 | -5.618 | 10 | -56.18% | +80.835 | 776 | 10.42% |
| 11/25/2025 - 12/01/2025 | -12.249 | 14 | -87.49% | +68.586 | 790 | 8.68% |
| 12/02/2025 - 12/08/2025 | +1.198 | 19 | 6.31% | +69.784 | 809 | 8.63% |
| 12/09/2025 - 12/15/2025 | +7.852 | 10 | 78.52% | +77.636 | 819 | 9.48% |
| 12/16/2025 - 12/22/2025 | -0.097 | 9 | -1.08% | +77.539 | 828 | 9.36% |
| 12/23/2025 - 12/29/2025 | -5.000 | 5 | -100.00% | +72.539 | 833 | 8.71% |