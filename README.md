## 📊 Data File
Download the Excel spreadsheet [here](./out.xlsx).

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

The model has been trained on historical data availble at https://www.football-data.co.uk/. Over a long time horizon, following the procedure above should yield positive returns. In testing over data starting on 8/25/12 and extending to the present day, the model achieved a profit of +1,320 "units" after 11,076 bets, a ROI of 11.9%. Extensive measures have been taken to validate the model and prevent overfitting. As of 6/26/25 I have been betting real money following the predictions. Therefore in the Excel sheet there is a tab which tracks returns since 6/26/25. Fingers crossed for a profitable season.


# Performance over last 20 weeks

| Date Range | Profit | Num Bets | ROI | Total Profit | Total Num Bets | Total ROI |
|---------------------|--------|----------|-------|--------------|----------------|-----------|
| 05/20/2025 - 05/26/2025 | +11.031 | 23 | 47.96% | +11.031 | 23 | 47.96% |
| 05/27/2025 - 06/02/2025 | +4.534 | 23 | 19.71% | +15.565 | 46 | 33.84% |
| 06/03/2025 - 06/09/2025 | +1.803 | 5 | 36.06% | +17.368 | 51 | 34.05% |
| 06/10/2025 - 06/16/2025 | -0.870 | 8 | -10.88% | +16.498 | 59 | 27.96% |
| 06/17/2025 - 06/23/2025 | +0.000 | 0 | 0.00% | +16.498 | 59 | 27.96% |
| 06/24/2025 - 06/30/2025 | -5.724 | 21 | -27.26% | +10.774 | 80 | 13.47% |
| 07/01/2025 - 07/07/2025 | -5.563 | 14 | -39.74% | +5.211 | 94 | 5.54% |
| 07/08/2025 - 07/14/2025 | -4.340 | 13 | -33.38% | +0.871 | 107 | 0.81% |
| 07/15/2025 - 07/21/2025 | -0.720 | 22 | -3.27% | +0.151 | 129 | 0.12% |
| 07/22/2025 - 07/28/2025 | -10.077 | 17 | -59.28% | -9.926 | 146 | -6.80% |
| 07/29/2025 - 08/04/2025 | -5.000 | 5 | -100.00% | -14.926 | 151 | -9.88% |
| 08/05/2025 - 08/11/2025 | +8.257 | 19 | 43.46% | -6.669 | 170 | -3.92% |
| 08/12/2025 - 08/18/2025 | -2.617 | 17 | -15.39% | -9.286 | 187 | -4.97% |
| 08/19/2025 - 08/25/2025 | +12.967 | 18 | 72.04% | +3.681 | 205 | 1.80% |
| 08/26/2025 - 09/01/2025 | +3.475 | 17 | 20.44% | +7.156 | 222 | 3.22% |
| 09/02/2025 - 09/08/2025 | +2.049 | 2 | 102.45% | +9.205 | 224 | 4.11% |
| 09/09/2025 - 09/15/2025 | +6.526 | 15 | 43.51% | +15.731 | 239 | 6.58% |
| 09/16/2025 - 09/22/2025 | -5.921 | 20 | -29.60% | +9.810 | 259 | 3.79% |
| 09/23/2025 - 09/29/2025 | +0.209 | 23 | 0.91% | +10.019 | 282 | 3.55% |
| 09/30/2025 - 10/06/2025 | -4.185 | 25 | -16.74% | +5.834 | 307 | 1.90% |