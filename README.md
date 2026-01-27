## 📊 Data File
Download the Excel spreadsheet [here](./out_excel.xlsx).

## Time-Window Summary

| Window | Date Range | Profit | Num Bets | ROI |
|----------------|---------------------|--------|----------|-------|
| Last 30 Days | 12/28/2025 - 01/26/2026 | -16.052 | 37 | -43.38% |
| Last 3 Months | 10/29/2025 - 01/26/2026 | -26.546 | 136 | -19.52% |
| Last 6 Months | 07/31/2025 - 01/26/2026 | -11.422 | 349 | -3.27% |
| YTD | 01/01/2026 - 01/26/2026 | -12.052 | 33 | -36.52% |
| Last 52 Weeks | 01/27/2025 - 01/26/2026 | +63.014 | 837 | 7.53% |
| All Time | 03/24/2013 - 01/26/2026 | +1302.701 | 11267 | 11.56% |

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
| 01/28/2025 - 02/03/2025 | +17.643 | 17 | 103.78% | +17.643 | 17 | 103.78% |
| 02/04/2025 - 02/10/2025 | -5.633 | 10 | -56.33% | +12.010 | 27 | 44.48% |
| 02/11/2025 - 02/17/2025 | +8.355 | 9 | 92.83% | +20.365 | 36 | 56.57% |
| 02/18/2025 - 02/24/2025 | -2.175 | 9 | -24.17% | +18.190 | 45 | 40.42% |
| 02/25/2025 - 03/03/2025 | -5.409 | 13 | -41.61% | +12.781 | 58 | 22.04% |
| 03/04/2025 - 03/10/2025 | +15.387 | 11 | 139.88% | +28.168 | 69 | 40.82% |
| 03/11/2025 - 03/17/2025 | +11.848 | 26 | 45.57% | +40.016 | 95 | 42.12% |
| 03/18/2025 - 03/24/2025 | -2.552 | 6 | -42.53% | +37.464 | 101 | 37.09% |
| 03/25/2025 - 03/31/2025 | -4.182 | 22 | -19.01% | +33.282 | 123 | 27.06% |
| 04/01/2025 - 04/07/2025 | +5.613 | 28 | 20.05% | +38.895 | 151 | 25.76% |
| 04/08/2025 - 04/14/2025 | +0.023 | 33 | 0.07% | +38.918 | 184 | 21.15% |
| 04/15/2025 - 04/21/2025 | +5.021 | 26 | 19.31% | +43.939 | 210 | 20.92% |
| 04/22/2025 - 04/28/2025 | +11.329 | 32 | 35.40% | +55.268 | 242 | 22.84% |
| 04/29/2025 - 05/05/2025 | +1.368 | 34 | 4.02% | +56.636 | 276 | 20.52% |
| 05/06/2025 - 05/12/2025 | +9.387 | 29 | 32.37% | +66.023 | 305 | 21.65% |
| 05/13/2025 - 05/19/2025 | +18.339 | 37 | 49.56% | +84.362 | 342 | 24.67% |
| 05/20/2025 - 05/26/2025 | +11.031 | 23 | 47.96% | +95.393 | 365 | 26.14% |
| 05/27/2025 - 06/02/2025 | +4.534 | 23 | 19.71% | +99.927 | 388 | 25.75% |
| 06/03/2025 - 06/09/2025 | +1.803 | 5 | 36.06% | +101.730 | 393 | 25.89% |
| 06/10/2025 - 06/16/2025 | -0.870 | 8 | -10.88% | +100.860 | 401 | 25.15% |
| 06/17/2025 - 06/23/2025 | +0.000 | 0 | 0.00% | +100.860 | 401 | 25.15% |
| 06/24/2025 - 06/30/2025 | -5.724 | 21 | -27.26% | +95.136 | 422 | 22.54% |
| 07/01/2025 - 07/07/2025 | -5.563 | 14 | -39.74% | +89.573 | 436 | 20.54% |
| 07/08/2025 - 07/14/2025 | -4.340 | 13 | -33.38% | +85.233 | 449 | 18.98% |
| 07/15/2025 - 07/21/2025 | -0.720 | 22 | -3.27% | +84.513 | 471 | 17.94% |
| 07/22/2025 - 07/28/2025 | -10.077 | 17 | -59.28% | +74.436 | 488 | 15.25% |
| 07/29/2025 - 08/04/2025 | -5.000 | 5 | -100.00% | +69.436 | 493 | 14.08% |
| 08/05/2025 - 08/11/2025 | +8.257 | 19 | 43.46% | +77.693 | 512 | 15.17% |
| 08/12/2025 - 08/18/2025 | -2.617 | 17 | -15.39% | +75.076 | 529 | 14.19% |
| 08/19/2025 - 08/25/2025 | +11.866 | 22 | 53.94% | +86.942 | 551 | 15.78% |
| 08/26/2025 - 09/01/2025 | +2.475 | 18 | 13.75% | +89.417 | 569 | 15.71% |
| 09/02/2025 - 09/08/2025 | +2.049 | 2 | 102.45% | +91.466 | 571 | 16.02% |
| 09/09/2025 - 09/15/2025 | +4.526 | 17 | 26.62% | +95.992 | 588 | 16.33% |
| 09/16/2025 - 09/22/2025 | -5.921 | 20 | -29.61% | +90.071 | 608 | 14.81% |
| 09/23/2025 - 09/29/2025 | -1.791 | 25 | -7.16% | +88.280 | 633 | 13.95% |
| 09/30/2025 - 10/06/2025 | -5.185 | 26 | -19.94% | +83.095 | 659 | 12.61% |
| 10/07/2025 - 10/13/2025 | -0.468 | 3 | -15.60% | +82.627 | 662 | 12.48% |
| 10/14/2025 - 10/20/2025 | -3.115 | 19 | -16.39% | +79.512 | 681 | 11.68% |
| 10/21/2025 - 10/27/2025 | +9.748 | 17 | 57.34% | +89.260 | 698 | 12.79% |
| 10/28/2025 - 11/03/2025 | -4.811 | 20 | -24.05% | +84.449 | 718 | 11.76% |
| 11/04/2025 - 11/10/2025 | +5.531 | 18 | 30.73% | +89.980 | 736 | 12.23% |
| 11/11/2025 - 11/17/2025 | -1.000 | 1 | -100.00% | +88.980 | 737 | 12.07% |
| 11/18/2025 - 11/24/2025 | -5.618 | 10 | -56.18% | +83.362 | 747 | 11.16% |
| 11/25/2025 - 12/01/2025 | -12.249 | 14 | -87.49% | +71.113 | 761 | 9.34% |
| 12/02/2025 - 12/08/2025 | +1.198 | 19 | 6.31% | +72.311 | 780 | 9.27% |
| 12/09/2025 - 12/15/2025 | +7.852 | 10 | 78.52% | +80.163 | 790 | 10.15% |
| 12/16/2025 - 12/22/2025 | -0.097 | 9 | -1.08% | +80.066 | 799 | 10.02% |
| 12/23/2025 - 12/29/2025 | -5.000 | 5 | -100.00% | +75.066 | 804 | 9.34% |
| 12/30/2025 - 01/05/2026 | +4.827 | 5 | 96.54% | +79.893 | 809 | 9.88% |
| 01/06/2026 - 01/12/2026 | -4.097 | 8 | -51.21% | +75.796 | 817 | 9.28% |
| 01/13/2026 - 01/19/2026 | -2.942 | 6 | -49.03% | +72.854 | 823 | 8.85% |
| 01/20/2026 - 01/26/2026 | -9.840 | 14 | -70.29% | +63.014 | 837 | 7.53% |