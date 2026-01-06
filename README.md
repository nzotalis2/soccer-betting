## 📊 Data File
Download the Excel spreadsheet [here](./out_excel.xlsx).

## Time-Window Summary

| Window | Date Range | Profit | Num Bets | ROI |
|----------------|---------------------|--------|----------|-------|
| Last 30 Days | 12/06/2025 - 01/04/2026 | +10.068 | 41 | 24.56% |
| Last 3 Months | 10/07/2025 - 01/04/2026 | -3.202 | 150 | -2.13% |
| Last 6 Months | 07/09/2025 - 01/04/2026 | -9.680 | 373 | -2.60% |
| YTD | 01/01/2026 - 01/04/2026 | +4.827 | 5 | 96.54% |
| Last 52 Weeks | 01/05/2025 - 01/04/2026 | +66.278 | 834 | 7.95% |
| All Time | 03/24/2013 - 01/04/2026 | +1319.580 | 11239 | 11.74% |

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
| 01/07/2025 - 01/13/2025 | -6.000 | 6 | -100.00% | -6.000 | 6 | -100.00% |
| 01/14/2025 - 01/20/2025 | -0.185 | 10 | -1.85% | -6.185 | 16 | -38.66% |
| 01/21/2025 - 01/27/2025 | -5.430 | 7 | -77.57% | -11.615 | 23 | -50.50% |
| 01/28/2025 - 02/03/2025 | +17.643 | 17 | 103.78% | +6.028 | 40 | 15.07% |
| 02/04/2025 - 02/10/2025 | -5.633 | 10 | -56.33% | +0.395 | 50 | 0.79% |
| 02/11/2025 - 02/17/2025 | +8.355 | 9 | 92.83% | +8.750 | 59 | 14.83% |
| 02/18/2025 - 02/24/2025 | -2.175 | 9 | -24.17% | +6.575 | 68 | 9.67% |
| 02/25/2025 - 03/03/2025 | -5.409 | 13 | -41.61% | +1.166 | 81 | 1.44% |
| 03/04/2025 - 03/10/2025 | +15.387 | 11 | 139.88% | +16.553 | 92 | 17.99% |
| 03/11/2025 - 03/17/2025 | +11.848 | 26 | 45.57% | +28.401 | 118 | 24.07% |
| 03/18/2025 - 03/24/2025 | -2.552 | 6 | -42.53% | +25.849 | 124 | 20.85% |
| 03/25/2025 - 03/31/2025 | -4.182 | 22 | -19.01% | +21.667 | 146 | 14.84% |
| 04/01/2025 - 04/07/2025 | +5.613 | 28 | 20.05% | +27.280 | 174 | 15.68% |
| 04/08/2025 - 04/14/2025 | +0.023 | 33 | 0.07% | +27.303 | 207 | 13.19% |
| 04/15/2025 - 04/21/2025 | +5.021 | 26 | 19.31% | +32.324 | 233 | 13.87% |
| 04/22/2025 - 04/28/2025 | +11.329 | 32 | 35.40% | +43.653 | 265 | 16.47% |
| 04/29/2025 - 05/05/2025 | +1.368 | 34 | 4.02% | +45.021 | 299 | 15.06% |
| 05/06/2025 - 05/12/2025 | +9.387 | 29 | 32.37% | +54.408 | 328 | 16.59% |
| 05/13/2025 - 05/19/2025 | +18.339 | 37 | 49.56% | +72.747 | 365 | 19.93% |
| 05/20/2025 - 05/26/2025 | +11.031 | 23 | 47.96% | +83.778 | 388 | 21.59% |
| 05/27/2025 - 06/02/2025 | +4.534 | 23 | 19.71% | +88.312 | 411 | 21.49% |
| 06/03/2025 - 06/09/2025 | +1.803 | 5 | 36.06% | +90.115 | 416 | 21.66% |
| 06/10/2025 - 06/16/2025 | -0.870 | 8 | -10.87% | +89.245 | 424 | 21.05% |
| 06/17/2025 - 06/23/2025 | +0.000 | 0 | 0.00% | +89.245 | 424 | 21.05% |
| 06/24/2025 - 06/30/2025 | -5.724 | 21 | -27.26% | +83.521 | 445 | 18.77% |
| 07/01/2025 - 07/07/2025 | -5.563 | 14 | -39.74% | +77.958 | 459 | 16.98% |
| 07/08/2025 - 07/14/2025 | -4.340 | 13 | -33.38% | +73.618 | 472 | 15.60% |
| 07/15/2025 - 07/21/2025 | -0.720 | 22 | -3.27% | +72.898 | 494 | 14.76% |
| 07/22/2025 - 07/28/2025 | -10.077 | 17 | -59.28% | +62.821 | 511 | 12.29% |
| 07/29/2025 - 08/04/2025 | -5.000 | 5 | -100.00% | +57.821 | 516 | 11.21% |
| 08/05/2025 - 08/11/2025 | +8.257 | 19 | 43.46% | +66.078 | 535 | 12.35% |
| 08/12/2025 - 08/18/2025 | -2.617 | 17 | -15.39% | +63.461 | 552 | 11.50% |
| 08/19/2025 - 08/25/2025 | +11.866 | 22 | 53.94% | +75.327 | 574 | 13.12% |
| 08/26/2025 - 09/01/2025 | +2.475 | 18 | 13.75% | +77.802 | 592 | 13.14% |
| 09/02/2025 - 09/08/2025 | +2.049 | 2 | 102.45% | +79.851 | 594 | 13.44% |
| 09/09/2025 - 09/15/2025 | +4.526 | 17 | 26.62% | +84.377 | 611 | 13.81% |
| 09/16/2025 - 09/22/2025 | -5.921 | 20 | -29.61% | +78.456 | 631 | 12.43% |
| 09/23/2025 - 09/29/2025 | -1.791 | 25 | -7.16% | +76.665 | 656 | 11.69% |
| 09/30/2025 - 10/06/2025 | -5.185 | 26 | -19.94% | +71.480 | 682 | 10.48% |
| 10/07/2025 - 10/13/2025 | -0.468 | 3 | -15.60% | +71.012 | 685 | 10.37% |
| 10/14/2025 - 10/20/2025 | -3.115 | 19 | -16.39% | +67.897 | 704 | 9.64% |
| 10/21/2025 - 10/27/2025 | +9.748 | 17 | 57.34% | +77.645 | 721 | 10.77% |
| 10/28/2025 - 11/03/2025 | -4.811 | 20 | -24.05% | +72.834 | 741 | 9.83% |
| 11/04/2025 - 11/10/2025 | +5.531 | 18 | 30.73% | +78.365 | 759 | 10.32% |
| 11/11/2025 - 11/17/2025 | -1.000 | 1 | -100.00% | +77.365 | 760 | 10.18% |
| 11/18/2025 - 11/24/2025 | -5.618 | 10 | -56.18% | +71.747 | 770 | 9.32% |
| 11/25/2025 - 12/01/2025 | -12.249 | 14 | -87.49% | +59.498 | 784 | 7.59% |
| 12/02/2025 - 12/08/2025 | +1.198 | 19 | 6.31% | +60.696 | 803 | 7.56% |
| 12/09/2025 - 12/15/2025 | +7.852 | 10 | 78.52% | +68.548 | 813 | 8.43% |
| 12/16/2025 - 12/22/2025 | -0.097 | 9 | -1.08% | +68.451 | 822 | 8.33% |
| 12/23/2025 - 12/29/2025 | -5.000 | 5 | -100.00% | +63.451 | 827 | 7.67% |
| 12/30/2025 - 01/05/2026 | +4.827 | 5 | 96.54% | +68.278 | 832 | 8.21% |