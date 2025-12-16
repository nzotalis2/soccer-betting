## 📊 Data File
Download the Excel spreadsheet [here](./out_excel.xlsx).

## Time-Window Summary

| Window | Date Range | Profit | Num Bets | ROI |
|----------------|---------------------|--------|----------|-------|
| Last 30 Days | 11/16/2025 - 12/15/2025 | -9.817 | 54 | -18.18% |
| Last 3 Months | 09/17/2025 - 12/15/2025 | -14.829 | 201 | -7.38% |
| Last 6 Months | 06/19/2025 - 12/15/2025 | -20.697 | 389 | -5.32% |
| YTD | 01/01/2025 - 12/15/2025 | +77.636 | 819 | 9.48% |
| Last 52 Weeks | 12/16/2024 - 12/15/2025 | +76.500 | 836 | 9.15% |
| All Time | 03/24/2013 - 12/15/2025 | +1319.850 | 11220 | 11.76% |

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
| 02/18/2025 - 02/24/2025 | -2.175 | 9 | -24.17% | +14.426 | 89 | 16.21% |
| 02/25/2025 - 03/03/2025 | -5.409 | 13 | -41.61% | +9.017 | 102 | 8.84% |
| 03/04/2025 - 03/10/2025 | +15.387 | 11 | 139.88% | +24.404 | 113 | 21.60% |
| 03/11/2025 - 03/17/2025 | +11.848 | 26 | 45.57% | +36.252 | 139 | 26.08% |
| 03/18/2025 - 03/24/2025 | -2.552 | 6 | -42.53% | +33.700 | 145 | 23.24% |
| 03/25/2025 - 03/31/2025 | -4.182 | 22 | -19.01% | +29.518 | 167 | 17.68% |
| 04/01/2025 - 04/07/2025 | +5.613 | 28 | 20.05% | +35.131 | 195 | 18.02% |
| 04/08/2025 - 04/14/2025 | +0.023 | 33 | 0.07% | +35.154 | 228 | 15.42% |
| 04/15/2025 - 04/21/2025 | +5.021 | 26 | 19.31% | +40.175 | 254 | 15.82% |
| 04/22/2025 - 04/28/2025 | +11.329 | 32 | 35.40% | +51.504 | 286 | 18.01% |
| 04/29/2025 - 05/05/2025 | +1.368 | 34 | 4.02% | +52.872 | 320 | 16.52% |
| 05/06/2025 - 05/12/2025 | +9.387 | 29 | 32.37% | +62.259 | 349 | 17.84% |
| 05/13/2025 - 05/19/2025 | +18.339 | 37 | 49.56% | +80.598 | 386 | 20.88% |
| 05/20/2025 - 05/26/2025 | +11.031 | 23 | 47.96% | +91.629 | 409 | 22.40% |
| 05/27/2025 - 06/02/2025 | +4.534 | 23 | 19.71% | +96.163 | 432 | 22.26% |
| 06/03/2025 - 06/09/2025 | +1.803 | 5 | 36.06% | +97.966 | 437 | 22.42% |
| 06/10/2025 - 06/16/2025 | -0.870 | 8 | -10.88% | +97.096 | 445 | 21.82% |
| 06/17/2025 - 06/23/2025 | +0.000 | 0 | 0.00% | +97.096 | 445 | 21.82% |
| 06/24/2025 - 06/30/2025 | -5.724 | 21 | -27.26% | +91.372 | 466 | 19.61% |
| 07/01/2025 - 07/07/2025 | -5.563 | 14 | -39.74% | +85.809 | 480 | 17.88% |
| 07/08/2025 - 07/14/2025 | -4.340 | 13 | -33.38% | +81.469 | 493 | 16.53% |
| 07/15/2025 - 07/21/2025 | -0.720 | 22 | -3.27% | +80.749 | 515 | 15.68% |
| 07/22/2025 - 07/28/2025 | -10.077 | 17 | -59.28% | +70.672 | 532 | 13.28% |
| 07/29/2025 - 08/04/2025 | -5.000 | 5 | -100.00% | +65.672 | 537 | 12.23% |
| 08/05/2025 - 08/11/2025 | +8.257 | 19 | 43.46% | +73.929 | 556 | 13.30% |
| 08/12/2025 - 08/18/2025 | -2.617 | 17 | -15.39% | +71.312 | 573 | 12.45% |
| 08/19/2025 - 08/25/2025 | +11.866 | 22 | 53.94% | +83.178 | 595 | 13.98% |
| 08/26/2025 - 09/01/2025 | +2.475 | 18 | 13.75% | +85.653 | 613 | 13.97% |
| 09/02/2025 - 09/08/2025 | +2.049 | 2 | 102.45% | +87.702 | 615 | 14.26% |
| 09/09/2025 - 09/15/2025 | +4.526 | 17 | 26.62% | +92.228 | 632 | 14.59% |
| 09/16/2025 - 09/22/2025 | -5.921 | 20 | -29.61% | +86.307 | 652 | 13.24% |
| 09/23/2025 - 09/29/2025 | -1.791 | 25 | -7.16% | +84.516 | 677 | 12.48% |
| 09/30/2025 - 10/06/2025 | -5.185 | 26 | -19.94% | +79.331 | 703 | 11.28% |
| 10/07/2025 - 10/13/2025 | -0.468 | 3 | -15.60% | +78.863 | 706 | 11.17% |
| 10/14/2025 - 10/20/2025 | -3.115 | 19 | -16.39% | +75.748 | 725 | 10.45% |
| 10/21/2025 - 10/27/2025 | +9.748 | 17 | 57.34% | +85.496 | 742 | 11.52% |
| 10/28/2025 - 11/03/2025 | -4.811 | 20 | -24.05% | +80.685 | 762 | 10.59% |
| 11/04/2025 - 11/10/2025 | +5.531 | 18 | 30.73% | +86.216 | 780 | 11.05% |
| 11/11/2025 - 11/17/2025 | -1.000 | 1 | -100.00% | +85.216 | 781 | 10.91% |
| 11/18/2025 - 11/24/2025 | -5.618 | 10 | -56.18% | +79.598 | 791 | 10.06% |
| 11/25/2025 - 12/01/2025 | -12.249 | 14 | -87.49% | +67.349 | 805 | 8.37% |
| 12/02/2025 - 12/08/2025 | +1.198 | 19 | 6.31% | +68.547 | 824 | 8.32% |
| 12/09/2025 - 12/15/2025 | +7.852 | 10 | 78.52% | +76.399 | 834 | 9.16% |