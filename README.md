## 📊 Data File
Download the Excel spreadsheet [here](./out_excel.xlsx).

## Time-Window Summary

| Window | Date Range | Profit | Num Bets | ROI |
|----------------|---------------------|--------|----------|-------|
| Last 30 Days | 11/09/2025 - 12/08/2025 | -18.274 | 50 | -36.55% |
| Last 3 Months | 09/10/2025 - 12/08/2025 | -16.755 | 200 | -8.38% |
| Last 6 Months | 06/12/2025 - 12/08/2025 | -24.918 | 373 | -6.68% |
| YTD | 01/01/2025 - 12/08/2025 | +75.436 | 796 | 9.48% |
| Last 52 Weeks | 12/09/2024 - 12/08/2025 | +98.506 | 826 | 11.93% |
| All Time | 08/25/2012 - 12/08/2025 | +1301.000 | 11236 | 11.58% |

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
| 12/10/2024 - 12/16/2024 | +21.105 | 14 | 150.75% | +21.105 | 14 | 150.75% |
| 12/17/2024 - 12/23/2024 | -0.388 | 6 | -6.47% | +20.717 | 20 | 103.58% |
| 12/24/2024 - 12/30/2024 | -0.849 | 9 | -9.43% | +19.868 | 29 | 68.51% |
| 12/31/2024 - 01/06/2025 | +9.088 | 6 | 151.47% | +28.956 | 35 | 82.73% |
| 01/07/2025 - 01/13/2025 | -6.000 | 6 | -100.00% | +22.956 | 41 | 55.99% |
| 01/14/2025 - 01/20/2025 | -0.185 | 10 | -1.85% | +22.771 | 51 | 44.65% |
| 01/21/2025 - 01/27/2025 | -5.430 | 7 | -77.57% | +17.341 | 58 | 29.90% |
| 01/28/2025 - 02/03/2025 | +17.643 | 17 | 103.78% | +34.984 | 75 | 46.65% |
| 02/04/2025 - 02/10/2025 | -5.633 | 10 | -56.33% | +29.351 | 85 | 34.53% |
| 02/11/2025 - 02/17/2025 | +8.355 | 9 | 92.83% | +37.706 | 94 | 40.11% |
| 02/18/2025 - 02/24/2025 | -1.024 | 10 | -10.24% | +36.682 | 104 | 35.27% |
| 02/25/2025 - 03/03/2025 | -5.409 | 13 | -41.61% | +31.273 | 117 | 26.73% |
| 03/04/2025 - 03/10/2025 | +15.387 | 11 | 139.88% | +46.660 | 128 | 36.45% |
| 03/11/2025 - 03/17/2025 | +11.848 | 26 | 45.57% | +58.508 | 154 | 37.99% |
| 03/18/2025 - 03/24/2025 | -2.552 | 6 | -42.53% | +55.956 | 160 | 34.97% |
| 03/25/2025 - 03/31/2025 | -4.182 | 22 | -19.01% | +51.774 | 182 | 28.45% |
| 04/01/2025 - 04/07/2025 | +5.613 | 28 | 20.05% | +57.387 | 210 | 27.33% |
| 04/08/2025 - 04/14/2025 | +0.023 | 33 | 0.07% | +57.410 | 243 | 23.63% |
| 04/15/2025 - 04/21/2025 | +5.021 | 26 | 19.31% | +62.431 | 269 | 23.21% |
| 04/22/2025 - 04/28/2025 | +11.329 | 32 | 35.40% | +73.760 | 301 | 24.50% |
| 04/29/2025 - 05/05/2025 | +1.368 | 34 | 4.02% | +75.128 | 335 | 22.43% |
| 05/06/2025 - 05/12/2025 | +9.387 | 29 | 32.37% | +84.515 | 364 | 23.22% |
| 05/13/2025 - 05/19/2025 | +18.339 | 37 | 49.56% | +102.854 | 401 | 25.65% |
| 05/20/2025 - 05/26/2025 | +11.031 | 23 | 47.96% | +113.885 | 424 | 26.86% |
| 05/27/2025 - 06/02/2025 | +4.534 | 23 | 19.71% | +118.419 | 447 | 26.49% |
| 06/03/2025 - 06/09/2025 | +1.803 | 5 | 36.06% | +120.222 | 452 | 26.60% |
| 06/10/2025 - 06/16/2025 | -0.870 | 8 | -10.87% | +119.352 | 460 | 25.95% |
| 06/17/2025 - 06/23/2025 | +0.000 | 0 | 0.00% | +119.352 | 460 | 25.95% |
| 06/24/2025 - 06/30/2025 | -5.724 | 21 | -27.26% | +113.628 | 481 | 23.62% |
| 07/01/2025 - 07/07/2025 | -5.563 | 14 | -39.74% | +108.065 | 495 | 21.83% |
| 07/08/2025 - 07/14/2025 | -4.340 | 13 | -33.38% | +103.725 | 508 | 20.42% |
| 07/15/2025 - 07/21/2025 | -0.720 | 22 | -3.27% | +103.005 | 530 | 19.43% |
| 07/22/2025 - 07/28/2025 | -10.077 | 17 | -59.28% | +92.928 | 547 | 16.99% |
| 07/29/2025 - 08/04/2025 | -5.000 | 5 | -100.00% | +87.928 | 552 | 15.93% |
| 08/05/2025 - 08/11/2025 | +8.257 | 19 | 43.46% | +96.185 | 571 | 16.85% |
| 08/12/2025 - 08/18/2025 | -2.617 | 17 | -15.39% | +93.568 | 588 | 15.91% |
| 08/19/2025 - 08/25/2025 | +12.967 | 18 | 72.04% | +106.535 | 606 | 17.58% |
| 08/26/2025 - 09/01/2025 | +3.475 | 17 | 20.44% | +110.010 | 623 | 17.66% |
| 09/02/2025 - 09/08/2025 | +2.049 | 2 | 102.45% | +112.059 | 625 | 17.93% |
| 09/09/2025 - 09/15/2025 | +6.526 | 15 | 43.51% | +118.585 | 640 | 18.53% |
| 09/16/2025 - 09/22/2025 | -5.921 | 20 | -29.61% | +112.664 | 660 | 17.07% |
| 09/23/2025 - 09/29/2025 | +0.209 | 23 | 0.91% | +112.873 | 683 | 16.53% |
| 09/30/2025 - 10/06/2025 | -4.185 | 25 | -16.74% | +108.688 | 708 | 15.35% |
| 10/07/2025 - 10/13/2025 | +0.532 | 2 | 26.60% | +109.220 | 710 | 15.38% |
| 10/14/2025 - 10/20/2025 | -3.115 | 19 | -16.39% | +106.105 | 729 | 14.55% |
| 10/21/2025 - 10/27/2025 | +10.748 | 16 | 67.17% | +116.853 | 745 | 15.68% |
| 10/28/2025 - 11/03/2025 | -7.111 | 19 | -37.43% | +109.742 | 764 | 14.36% |
| 11/04/2025 - 11/10/2025 | +3.231 | 17 | 19.01% | +112.973 | 781 | 14.47% |
| 11/11/2025 - 11/17/2025 | -1.000 | 1 | -100.00% | +111.973 | 782 | 14.32% |
| 11/18/2025 - 11/24/2025 | -5.618 | 10 | -56.18% | +106.355 | 792 | 13.43% |
| 11/25/2025 - 12/01/2025 | -12.249 | 14 | -87.49% | +94.106 | 806 | 11.68% |
| 12/02/2025 - 12/08/2025 | +1.198 | 19 | 6.31% | +95.304 | 825 | 11.55% |