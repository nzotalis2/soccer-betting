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
| 06/17/2025 - 06/23/2025 | +0.000 | 0 | 0.00% | +0.000 | 0 | 0.00% |
| 06/24/2025 - 06/30/2025 | -5.724 | 21 | -27.26% | -5.724 | 21 | -27.26% |
| 07/01/2025 - 07/07/2025 | -5.563 | 14 | -39.74% | -11.287 | 35 | -32.25% |
| 07/08/2025 - 07/14/2025 | -4.340 | 13 | -33.38% | -15.627 | 48 | -32.56% |
| 07/15/2025 - 07/21/2025 | -0.720 | 22 | -3.27% | -16.347 | 70 | -23.35% |
| 07/22/2025 - 07/28/2025 | -10.077 | 17 | -59.28% | -26.424 | 87 | -30.37% |
| 07/29/2025 - 08/04/2025 | -5.000 | 5 | -100.00% | -31.424 | 92 | -34.16% |
| 08/05/2025 - 08/11/2025 | +8.257 | 19 | 43.46% | -23.167 | 111 | -20.87% |
| 08/12/2025 - 08/18/2025 | -2.617 | 17 | -15.39% | -25.784 | 128 | -20.14% |
| 08/19/2025 - 08/25/2025 | +12.967 | 18 | 72.04% | -12.817 | 146 | -8.78% |
| 08/26/2025 - 09/01/2025 | +3.475 | 17 | 20.44% | -9.342 | 163 | -5.73% |
| 09/02/2025 - 09/08/2025 | +2.049 | 2 | 102.45% | -7.293 | 165 | -4.42% |
| 09/09/2025 - 09/15/2025 | +6.526 | 15 | 43.51% | -0.767 | 180 | -0.43% |
| 09/16/2025 - 09/22/2025 | -5.921 | 20 | -29.61% | -6.688 | 200 | -3.34% |
| 09/23/2025 - 09/29/2025 | +0.209 | 23 | 0.91% | -6.479 | 223 | -2.91% |
| 09/30/2025 - 10/06/2025 | -4.185 | 25 | -16.74% | -10.664 | 248 | -4.30% |
| 10/07/2025 - 10/13/2025 | +0.532 | 2 | 26.60% | -10.132 | 250 | -4.05% |
| 10/14/2025 - 10/20/2025 | -3.115 | 19 | -16.39% | -13.247 | 269 | -4.92% |
| 10/21/2025 - 10/27/2025 | +10.748 | 16 | 67.18% | -2.499 | 285 | -0.88% |
| 10/28/2025 - 11/03/2025 | -7.111 | 19 | -37.43% | -9.610 | 304 | -3.16% |