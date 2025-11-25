## 📊 Data File
Download the Excel spreadsheet [here](./out_excel.xlsx).

## Time-Window Summary

| Window | Date Range | Profit | Num Bets | ROI |
|----------------|---------------------|--------|----------|-------|
| Last 30 Days | 10/25/2025 - 11/23/2025 | -9.075 | 58 | -15.65% |
| Last 3 Months | 08/26/2025 - 11/23/2025 | -0.180 | 186 | -0.10% |
| Last 6 Months | 05/28/2025 - 11/23/2025 | -7.530 | 368 | -2.05% |
| YTD | 01/01/2025 - 11/23/2025 | +86.487 | 763 | 11.34% |
| Last 52 Weeks | 11/24/2024 - 11/23/2025 | +112.721 | 833 | 13.53% |
| All Time | 08/25/2012 - 11/23/2025 | +1312.051 | 11203 | 11.71% |

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
| 11/26/2024 - 12/02/2024 | -2.323 | 11 | -21.12% | -2.323 | 11 | -21.12% |
| 12/03/2024 - 12/09/2024 | +8.292 | 25 | 33.17% | +5.969 | 36 | 16.58% |
| 12/10/2024 - 12/16/2024 | +21.105 | 14 | 150.75% | +27.074 | 50 | 54.15% |
| 12/17/2024 - 12/23/2024 | -0.388 | 6 | -6.47% | +26.686 | 56 | 47.65% |
| 12/24/2024 - 12/30/2024 | -0.849 | 9 | -9.43% | +25.837 | 65 | 39.75% |
| 12/31/2024 - 01/06/2025 | +9.088 | 6 | 151.47% | +34.925 | 71 | 49.19% |
| 01/07/2025 - 01/13/2025 | -6.000 | 6 | -100.00% | +28.925 | 77 | 37.56% |
| 01/14/2025 - 01/20/2025 | -0.185 | 10 | -1.85% | +28.740 | 87 | 33.03% |
| 01/21/2025 - 01/27/2025 | -5.430 | 7 | -77.57% | +23.310 | 94 | 24.80% |
| 01/28/2025 - 02/03/2025 | +17.643 | 17 | 103.78% | +40.953 | 111 | 36.89% |
| 02/04/2025 - 02/10/2025 | -5.633 | 10 | -56.33% | +35.320 | 121 | 29.19% |
| 02/11/2025 - 02/17/2025 | +8.355 | 9 | 92.83% | +43.675 | 130 | 33.60% |
| 02/18/2025 - 02/24/2025 | -1.024 | 10 | -10.24% | +42.651 | 140 | 30.46% |
| 02/25/2025 - 03/03/2025 | -5.409 | 13 | -41.61% | +37.242 | 153 | 24.34% |
| 03/04/2025 - 03/10/2025 | +15.387 | 11 | 139.88% | +52.629 | 164 | 32.09% |
| 03/11/2025 - 03/17/2025 | +11.848 | 26 | 45.57% | +64.477 | 190 | 33.94% |
| 03/18/2025 - 03/24/2025 | -2.552 | 6 | -42.53% | +61.925 | 196 | 31.59% |
| 03/25/2025 - 03/31/2025 | -4.182 | 22 | -19.01% | +57.743 | 218 | 26.49% |
| 04/01/2025 - 04/07/2025 | +5.613 | 28 | 20.05% | +63.356 | 246 | 25.75% |
| 04/08/2025 - 04/14/2025 | +0.023 | 33 | 0.07% | +63.379 | 279 | 22.72% |
| 04/15/2025 - 04/21/2025 | +5.021 | 26 | 19.31% | +68.400 | 305 | 22.43% |
| 04/22/2025 - 04/28/2025 | +11.329 | 32 | 35.40% | +79.729 | 337 | 23.66% |
| 04/29/2025 - 05/05/2025 | +1.368 | 34 | 4.02% | +81.097 | 371 | 21.86% |
| 05/06/2025 - 05/12/2025 | +9.387 | 29 | 32.37% | +90.484 | 400 | 22.62% |
| 05/13/2025 - 05/19/2025 | +18.339 | 37 | 49.56% | +108.823 | 437 | 24.90% |
| 05/20/2025 - 05/26/2025 | +11.031 | 23 | 47.96% | +119.854 | 460 | 26.06% |
| 05/27/2025 - 06/02/2025 | +4.534 | 23 | 19.71% | +124.388 | 483 | 25.75% |
| 06/03/2025 - 06/09/2025 | +1.803 | 5 | 36.06% | +126.191 | 488 | 25.86% |
| 06/10/2025 - 06/16/2025 | -0.870 | 8 | -10.88% | +125.321 | 496 | 25.27% |
| 06/17/2025 - 06/23/2025 | +0.000 | 0 | 0.00% | +125.321 | 496 | 25.27% |
| 06/24/2025 - 06/30/2025 | -5.724 | 21 | -27.26% | +119.597 | 517 | 23.13% |
| 07/01/2025 - 07/07/2025 | -5.563 | 14 | -39.74% | +114.034 | 531 | 21.48% |
| 07/08/2025 - 07/14/2025 | -4.340 | 13 | -33.38% | +109.694 | 544 | 20.16% |
| 07/15/2025 - 07/21/2025 | -0.720 | 22 | -3.27% | +108.974 | 566 | 19.25% |
| 07/22/2025 - 07/28/2025 | -10.077 | 17 | -59.28% | +98.897 | 583 | 16.96% |
| 07/29/2025 - 08/04/2025 | -5.000 | 5 | -100.00% | +93.897 | 588 | 15.97% |
| 08/05/2025 - 08/11/2025 | +8.257 | 19 | 43.46% | +102.154 | 607 | 16.83% |
| 08/12/2025 - 08/18/2025 | -2.617 | 17 | -15.39% | +99.537 | 624 | 15.95% |
| 08/19/2025 - 08/25/2025 | +12.967 | 18 | 72.04% | +112.504 | 642 | 17.52% |
| 08/26/2025 - 09/01/2025 | +3.475 | 17 | 20.44% | +115.979 | 659 | 17.60% |
| 09/02/2025 - 09/08/2025 | +2.049 | 2 | 102.45% | +118.028 | 661 | 17.86% |
| 09/09/2025 - 09/15/2025 | +6.526 | 15 | 43.51% | +124.554 | 676 | 18.43% |
| 09/16/2025 - 09/22/2025 | -5.921 | 20 | -29.60% | +118.633 | 696 | 17.04% |
| 09/23/2025 - 09/29/2025 | +0.209 | 23 | 0.91% | +118.842 | 719 | 16.53% |
| 09/30/2025 - 10/06/2025 | -4.185 | 25 | -16.74% | +114.657 | 744 | 15.41% |
| 10/07/2025 - 10/13/2025 | +0.532 | 2 | 26.60% | +115.189 | 746 | 15.44% |
| 10/14/2025 - 10/20/2025 | -3.115 | 19 | -16.39% | +112.074 | 765 | 14.65% |
| 10/21/2025 - 10/27/2025 | +10.748 | 16 | 67.18% | +122.822 | 781 | 15.73% |
| 10/28/2025 - 11/03/2025 | -7.111 | 19 | -37.43% | +115.711 | 800 | 14.46% |
| 11/04/2025 - 11/10/2025 | +3.231 | 17 | 19.01% | +118.942 | 817 | 14.56% |
| 11/11/2025 - 11/17/2025 | -1.000 | 1 | -100.00% | +117.942 | 818 | 14.42% |
| 11/18/2025 - 11/24/2025 | -5.618 | 10 | -56.18% | +112.324 | 828 | 13.57% |