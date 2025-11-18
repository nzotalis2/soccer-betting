## 📊 Data File
Download the Excel spreadsheet [here](./out_excel.xlsx).

## Time-Window Summary

| Window | Date Range | Profit | Num Bets | ROI |
|----------------|---------------------|--------|----------|-------|
| Last 30 Days | 10/18/2025 - 11/16/2025 | +4.753 | 70 | 6.79% |
| Last 3 Months | 08/19/2025 - 11/16/2025 | +18.405 | 194 | 9.49% |
| Last 6 Months | 05/21/2025 - 11/16/2025 | +9.119 | 381 | 2.39% |
| YTD | 01/01/2025 - 11/16/2025 | +92.105 | 753 | 12.23% |
| Last 52 Weeks | 11/17/2024 - 11/16/2025 | +114.914 | 836 | 13.75% |
| All Time | 08/25/2012 - 11/16/2025 | +1317.669 | 11193 | 11.77% |

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
| 11/19/2024 - 11/25/2024 | -3.028 | 18 | -16.82% | -3.028 | 18 | -16.82% |
| 11/26/2024 - 12/02/2024 | -2.323 | 11 | -21.12% | -5.351 | 29 | -18.45% |
| 12/03/2024 - 12/09/2024 | +8.292 | 25 | 33.17% | +2.941 | 54 | 5.45% |
| 12/10/2024 - 12/16/2024 | +21.105 | 14 | 150.75% | +24.046 | 68 | 35.36% |
| 12/17/2024 - 12/23/2024 | -0.388 | 6 | -6.47% | +23.658 | 74 | 31.97% |
| 12/24/2024 - 12/30/2024 | -0.849 | 9 | -9.43% | +22.809 | 83 | 27.48% |
| 12/31/2024 - 01/06/2025 | +9.088 | 6 | 151.47% | +31.897 | 89 | 35.84% |
| 01/07/2025 - 01/13/2025 | -6.000 | 6 | -100.00% | +25.897 | 95 | 27.26% |
| 01/14/2025 - 01/20/2025 | -0.185 | 10 | -1.85% | +25.712 | 105 | 24.49% |
| 01/21/2025 - 01/27/2025 | -5.430 | 7 | -77.57% | +20.282 | 112 | 18.11% |
| 01/28/2025 - 02/03/2025 | +17.643 | 17 | 103.78% | +37.925 | 129 | 29.40% |
| 02/04/2025 - 02/10/2025 | -5.633 | 10 | -56.33% | +32.292 | 139 | 23.23% |
| 02/11/2025 - 02/17/2025 | +8.355 | 9 | 92.83% | +40.647 | 148 | 27.46% |
| 02/18/2025 - 02/24/2025 | -1.024 | 10 | -10.24% | +39.623 | 158 | 25.08% |
| 02/25/2025 - 03/03/2025 | -5.409 | 13 | -41.61% | +34.214 | 171 | 20.01% |
| 03/04/2025 - 03/10/2025 | +15.387 | 11 | 139.88% | +49.601 | 182 | 27.25% |
| 03/11/2025 - 03/17/2025 | +11.848 | 26 | 45.57% | +61.449 | 208 | 29.54% |
| 03/18/2025 - 03/24/2025 | -2.552 | 6 | -42.53% | +58.897 | 214 | 27.52% |
| 03/25/2025 - 03/31/2025 | -4.182 | 22 | -19.01% | +54.715 | 236 | 23.18% |
| 04/01/2025 - 04/07/2025 | +5.613 | 28 | 20.05% | +60.328 | 264 | 22.85% |
| 04/08/2025 - 04/14/2025 | +0.023 | 33 | 0.07% | +60.351 | 297 | 20.32% |
| 04/15/2025 - 04/21/2025 | +5.021 | 26 | 19.31% | +65.372 | 323 | 20.24% |
| 04/22/2025 - 04/28/2025 | +11.329 | 32 | 35.40% | +76.701 | 355 | 21.61% |
| 04/29/2025 - 05/05/2025 | +1.368 | 34 | 4.02% | +78.069 | 389 | 20.07% |
| 05/06/2025 - 05/12/2025 | +9.387 | 29 | 32.37% | +87.456 | 418 | 20.92% |
| 05/13/2025 - 05/19/2025 | +18.339 | 37 | 49.56% | +105.795 | 455 | 23.25% |
| 05/20/2025 - 05/26/2025 | +11.031 | 23 | 47.96% | +116.826 | 478 | 24.44% |
| 05/27/2025 - 06/02/2025 | +4.534 | 23 | 19.71% | +121.360 | 501 | 24.22% |
| 06/03/2025 - 06/09/2025 | +1.803 | 5 | 36.06% | +123.163 | 506 | 24.34% |
| 06/10/2025 - 06/16/2025 | -0.870 | 8 | -10.88% | +122.293 | 514 | 23.79% |
| 06/17/2025 - 06/23/2025 | +0.000 | 0 | 0.00% | +122.293 | 514 | 23.79% |
| 06/24/2025 - 06/30/2025 | -5.724 | 21 | -27.26% | +116.569 | 535 | 21.79% |
| 07/01/2025 - 07/07/2025 | -5.563 | 14 | -39.74% | +111.006 | 549 | 20.22% |
| 07/08/2025 - 07/14/2025 | -4.340 | 13 | -33.38% | +106.666 | 562 | 18.98% |
| 07/15/2025 - 07/21/2025 | -0.720 | 22 | -3.27% | +105.946 | 584 | 18.14% |
| 07/22/2025 - 07/28/2025 | -10.077 | 17 | -59.28% | +95.869 | 601 | 15.95% |
| 07/29/2025 - 08/04/2025 | -5.000 | 5 | -100.00% | +90.869 | 606 | 14.99% |
| 08/05/2025 - 08/11/2025 | +8.257 | 19 | 43.46% | +99.126 | 625 | 15.86% |
| 08/12/2025 - 08/18/2025 | -2.617 | 17 | -15.39% | +96.509 | 642 | 15.03% |
| 08/19/2025 - 08/25/2025 | +12.967 | 18 | 72.04% | +109.476 | 660 | 16.59% |
| 08/26/2025 - 09/01/2025 | +3.475 | 17 | 20.44% | +112.951 | 677 | 16.68% |
| 09/02/2025 - 09/08/2025 | +2.049 | 2 | 102.45% | +115.000 | 679 | 16.94% |
| 09/09/2025 - 09/15/2025 | +6.526 | 15 | 43.51% | +121.526 | 694 | 17.51% |
| 09/16/2025 - 09/22/2025 | -5.921 | 20 | -29.61% | +115.605 | 714 | 16.19% |
| 09/23/2025 - 09/29/2025 | +0.209 | 23 | 0.91% | +115.814 | 737 | 15.71% |
| 09/30/2025 - 10/06/2025 | -4.185 | 25 | -16.74% | +111.629 | 762 | 14.65% |
| 10/07/2025 - 10/13/2025 | +0.532 | 2 | 26.60% | +112.161 | 764 | 14.68% |
| 10/14/2025 - 10/20/2025 | -3.115 | 19 | -16.39% | +109.046 | 783 | 13.93% |
| 10/21/2025 - 10/27/2025 | +10.748 | 16 | 67.18% | +119.794 | 799 | 14.99% |
| 10/28/2025 - 11/03/2025 | -7.111 | 19 | -37.43% | +112.683 | 818 | 13.78% |
| 11/04/2025 - 11/10/2025 | +3.231 | 17 | 19.01% | +115.914 | 835 | 13.88% |
| 11/11/2025 - 11/17/2025 | -1.000 | 1 | -100.00% | +114.914 | 836 | 13.75% |