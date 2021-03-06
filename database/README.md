### Database

This module contains the data about students' performances in contests.

It also contains functions necessary to query and update this data.

#### Description
1. contest_ranks: Each file contains rank list of students
2. db_pass.txt: Password to access the database. This version of the file is accessible only to those managing the repository.
3. db_tools.py: Variables and functions to read, write and reset database

##### Contest Ranks
Following is the list of contests that have been considered for rating so far

| S.no. | Contest Name | Rank File | Start Date | End Date |
| ----- | ----------------- | ----------- | ------------- | ---------- |
| 1. | [Google Codejam 2018 Qualification Round](https://codejam.withgoogle.com/2018/challenges/00000000000000cb/scoreboard) | codejam_qualification-2018.in | 07/04/2018(04:30) | 08/04/2018(07:30) |
| 2. | [Google Codejam 2018 Round 1A](https://codejam.withgoogle.com/2018/challenges/0000000000007883/scoreboard) | codejam-1a-2018.in | 14/04/2018(06:30) | 14/04/2018(09:00) |
| 3. | [Google Codejam 2018 Round 1B](https://codejam.withgoogle.com/2018/challenges/0000000000007764/scoreboard) | codejam-1b-2018.in | 29/04/2018(21:30) | 30/04/2018(00:00) |
| 4. | [Google Codejam 2018 Round 1C](https://codejam.withgoogle.com/2018/challenges/0000000000007765/scoreboard) | codejam-1c-2018.in | 05/05/2018(14:30) | 05/05/2018(20:00) |
| 5. | [PESU Alcoding Club April 2018](https://www.hackerearth.com/challenge/college/pes-alcoding-contest-2018-april/leaderboard/) | hackerearth-alcoding-2018.in | 18/04/2018(16:00) | 18/04/2018(20:30) |
| 6. | [Codechef June Long Challenge 2018](https://www.codechef.com/JUNE18) | codechef-june18.in | 01/06/2018(15:00) | 11/06/2018(15:00) |
| 7. | [Codechef July Long Challenge 2018](https://www.codechef.com/JULY18) | codechef-july18.in | 06/06/2018(15:00) | 16/07/2018(15:00) |
| 8. | [Codechef August Long Challenge 2018](https://www.codechef.com/AUG18) | codechef-aug18.in | 03/08/2018(15:00) | 13/08/2018(15:00) |
| 9. | [Codechef September Long Challenge 2018](https://www.codechef.com/SEPT18) | codechef-sept18.in | 07/09/2018(15:00) | 17/09/2018(15:00) |
| 10. | [Codechef October Long Challenge 2018](https://www.codechef.com/OCT18) | codechef-oct18.in | 05/10/2018 (15:00) | 17/10/2018(15:00) |
| 11. | [Codechef November Long Challenge 2018](https://www.codechef.com/NOV18) | codechef-nov18.in | 02/11/2018(15:00) | 12/11/2018(15:00) |
| 12. | [Codechef December Long Challenge 2018](https://www.codechef.com/DEC18) | codechef-dec18.in | 07/12/2018(15:00) | 17/12/2018(15:00) |
| 13. | [Hackearth January Easy 2019](https://www.hackerearth.com/challenge/competitive/january-easy-19/) | hackerearth-jan-easy-2019.in | 06/01/2019(21:00) | 07/01/2019(00:00) |
| 14. | [Codechef January Long Challenge 2019](https://www.codechef.com/JAN19) | codechef-jan19.in | 04/01/2019(15:00) | 14/01/2019(15:00) |
| 15. | [Hackearth February Easy 2019](https://www.hackerearth.com/challenges/competitive/february-easy-19/) | hackerearth-feb-easy-2019.in | 01/02/2019(21:00) | 02/02/2019(00:00) |
| 16. | [Codechef February Long Challenge 2019](https://www.codechef.com/FEB19) | codechef-feb19.in | 01/02/2019(15:00) | 11/02/2019(15:00) |
| 17. | [Codechef February Cookoff 2019](https://www.codechef.com/COOK103) | codechef-feb-cookoff19.in | 17/02/2019(21:30) | 18/02/2019(00:00) |
| 18. | [Hackerearth February Circuits 2019](https://www.hackerearth.com/challenges/competitive/february-circuits-19/) | hackerearth-feb-circuits19.in | 15/02/2019(21:00) | 24/02/2019(21:00) |
| 19. | [Codechef March Long Challenge 2019](https://www.codechef.com/MARCH19) | codechef-mar19.in | 01/03/2019(15:00) | 11/03/2019(15:00) |
| 20. | [Google Kickstart 2019 Round A](https://codingcompetitions.withgoogle.com/kickstart/round/0000000000050e01) | kickstart-a-2019.in | 24/03/2019(09:30) | 24/03/2019(12:45) |
| 21. | [Codechef March Cookoff 2019](https://www.codechef.com/COOK104) | codechef-mar-cookoff19.in | 24/03/2019(21:30) | 25/03/2019(00:00) |
| 22. | [Codechef March Lunchtime 2019](https://www.codechef.com/LTIME70) | codechef-mar-lunchtime19.in | 30/03/2019(19:30) | 30/03/2019(22:30) |
| 23. | [Hackerearth March Circuits 2019](https://www.hackerearth.com/challenges/competitive/march-circuits-19/) | hackerearth-mar-circuits-2019.in | 22/03/2019(21:00) | 31/03/2019(21:00) |
| 24. | [Hackerearth April Easy 2019](https://www.hackerearth.com/challenge/competitive/april-easy-19/) | hackerearth-april-easy-2019.in | 06/04/2019(21:30) | 07/04/2019(00:30) |
| 25. | [Google Codejam 2019 Qualification Round](https://codingcompetitions.withgoogle.com/codejam/round/0000000000051705) | codejam_qualification-2019.in | 06/04/2019(04:30) | 07/04/2019(7:30) |
| 26. | [Google Codejam 2019 Round 1A](https://codingcompetitions.withgoogle.com/codejam/round/0000000000051635) | codejam-1a-2019.in | 13/04/2019(06:30) | 13/04/2019(09:00) |
| 27. | [Hackerearth HourStorm #10 2019](https://www.hackerearth.com/challenges/competitive/hourstorm-10/) | hackerearth-hourstorm#10-2019.in | 13/04/2019(21:30) | 13/04/2019(22:30) |
| 28. | [Codechef April Long Challenge 2019](https://www.codechef.com/APRIL19) | codechef-april19.in | 05/04/2019(15:00) | 15/04/2019(15:00) |
| 29. | [Google Kickstart 2019 Round B](https://codingcompetitions.withgoogle.com/kickstart/round/0000000000050eda) | kickstart-b-2019.in | 21/04/2019(04:30) | 21/04/2019(07:30) |
| 30. | [Codechef April Cookoff 2019](https://www.codechef.com/COOK105) | codechef-april-cookoff19.in | 21/04/2019(21:30) | 22/04/2019(00:00) |
| 31. | [Codechef April Lunchtime 2019](https://www.codechef.com/LTIME71) | codechef-april-lunchtime19.in | 27/04/2019(19:30) | 27/04/2019(22:30) |
| 32. | [Google Codejam 2019 Round 1B](https://codingcompetitions.withgoogle.com/codejam/round/0000000000051706) | codejam-1b-2019.in | 28/04/2019(21:30) | 29/04/2019(00:00) |
| 33. | [Google Codejam 2019 Round 1C](https://codingcompetitions.withgoogle.com/codejam/round/00000000000516b9) | codejam-1c-2019.in | 04/05/2019(14:30) | 04/05/2019(17:00) |
| 34. | [Hackerearth April Circuits 2019](https://www.hackerearth.com/challenges/competitive/april-circuits-19/) | hackerearth-april-circuits19.in | 26/04/2019(21:00) | 05/05/2019(21:00) |
| 35. | [Codechef May Long Challenge 2019](https://www.codechef.com/MAY19) | codechef-may19.in | 03/05/2019(15:00) | 13/05/2019(15:00) |
| 36. | [Hackerearth May Easy 2019](https://www.hackerearth.com/challenge/competitive/may-easy-19/) | hackerearth-may-easy-2019.in | 13/05/2019(21:30) | 14/05/2019(00:00) |
| 37. | [Google Codejam 2019 Round 2](https://codingcompetitions.withgoogle.com/codejam/round/0000000000051679) | codejam-round2-2019.in | 18/05/2019(19:30) | 18/05/2019(22:00) |
| 38. | [Codechef May Cookoff 2019](https://www.codechef.com/COOK106) | codechef-may-cookoff19.in | 19/05/2019(21:30) | 19/05/2019(00:00) |
| 39. | [Codechef May Lunchtime 2019](https://www.codechef.com/LTIME72) | codechef-may-lunchtime19.in | 25/05/2019(19:30) | 25/05/2019(22:30) |
| 40. | [Google Kickstart 2019 Round C](https://codingcompetitions.withgoogle.com/kickstart/round/0000000000050ff2) | kickstart-c-2019.in | 26/05/2019(14:30) | 26/05/2019(17:30) |
| 41. | [Hackerearth May Circuits 2019](https://www.hackerearth.com/challenges/competitive/may-circuits-19/) | hackerearth-may-circuits19.in | 24/05/2019(21:00) | 02/06/2019(21:00) |
| 42. | [Hackerearth June Easy 2019](https://www.hackerearth.com/challenge/competitive/june-easy-19/) | hackerearth-june-easy-2019.in | 2/06/2019(21:30) | 3/06/2019(00:30) |
| 43. | [Hackerrank Alcoding Summer Week 1](https://www.hackerrank.com/contests/alcoding-summer-weekly-contest-1/challenges) | hackerrank-alcoding-summer19-1.in | 7/06/2019(21:00) | 8/06/2019(00:00) |
| 44. | [Hackerrank Alcoding Summer Week 2](https://www.hackerrank.com/contests/alcoding-summer-weekly-contest-2/challenges) | hackerrank-alcoding-summer19-2.in | 14/06/2019(21:00) | 15/06/2019(00:00) |
| 45. | [Codechef June Long Challenge 2019](https://www.codechef.com/JUNE19) | codechef-june19.in | 07/06/2019(15:00) | 17/05/2019(16:00) |
| 46. | [Hackerrank Alcoding Summer Week 3](https://www.hackerrank.com/contests/alcoding-summer-weekly-contest-3/challenges) | hackerrank-alcoding-summer19-3.in | 21/06/2019(21:00) | 22/06/2019(00:00) |
| 47. | [Codechef June Cookoff 2019](https://www.codechef.com/COOK107) | codechef-june-cookoff19.in | 23/06/2019(21:30) | 24/06/2019(00:00) |
| 48. | [Hackerrank Alcoding Summer Week 4](https://www.hackerrank.com/contests/alcoding-summer-weekly-contest-4/challenges) | hackerrank-alcoding-summer19-4.in | 28/06/2019(21:00) | 29/06/2019(00:00) |
| 49. | [Codechef June Lunchtime 2019](https://www.codechef.com/LTIME73) | codechef-june-lunchtime19.in | 29/06/2019(19:30) | 29/06/2019(22:30) |
| 50. | [Hackerearth June Circuits 2019](https://www.hackerearth.com/challenges/competitive/june-circuits-19/) | hackerearth-june-circuits19.in | 21/06/2019(21:00) | 30/06/2019(21:00) |
| 51. | [Hackerrank Alcoding Summer Week 5](https://www.hackerrank.com/contests/alcoding-summer-weekly-contest-5/challenges) | hackerrank-alcoding-summer19-5.in | 05/07/2019(21:00) | 05/07/2019(00:00) |
| 52. | [Hackerearth July Easy 2019](https://www.hackerearth.com/challenge/competitive/july-easy-19/) | hackerearth-july-easy-2019.in | 07/07/2019(09:30) | 07/07/2019(12:30) |
| 53. | [Codechef July Long Challenge 2019](https://www.codechef.com/JULY19) | codechef-july19.in | 05/07/2019(15:00) | 15/07/2019(15:00) |
| 54. | [Hackerrank Alcoding Summer Week 6](https://www.hackerrank.com/contests/alcoding-summer-weekly-contest-6/challenges) | hackerrank-alcoding-summer19-6.in | 19/07/2019(21:00) | 20/07/2019(00:00) |
| 55. | [Codechef July Cookoff 2019](https://www.codechef.com/COOK108) | codechef-july-cookoff19.in | 21/07/2019(21:30) | 22/07/2019(00:00) |
| 56. | [Hackerrank Alcoding Summer Week 7](https://www.hackerrank.com/contests/alcoding-summer-weekly-contest-7/challenges) | hackerrank-alcoding-summer19-7.in | 26/07/2019(21:00) | 27/07/2019(00:00) |
| 57. | [Codechef July Lunchtime 2019](https://www.codechef.com/LTIME74) | codechef-july-lunchtime19.in | 27/07/2019(19:30) | 29/06/2019(22:30) |
| 58. | [Google Kickstart 2019 Round D](https://codingcompetitions.withgoogle.com/kickstart/round/0000000000051061) | kickstart-d-2019.in | 28/07/2019(10:30) | 28/07/2019(13:30) |
| 59. | [Hackerearth August Easy 2019](https://www.hackerearth.com/challenge/competitive/august-easy-19/) | hackerearth-august-easy-2019.in | 04/08/2019(09:30) | 04/08/2019(12:30) |
| 60. | [Codechef August Long Challenge 2019](https://www.codechef.com/AUG19) | codechef-aug19.in | 02/08/2019(15:00) | 12/08/2019(15:00) |
| 61. | [Codechef August Cookoff 2019](https://www.codechef.com/COOK109) | codechef-aug-cookoff19.in | 18/08/2019(21:30) | 19/08/2019(00:00) |
| 62. | [Google Kickstart 2019 Round E](https://codingcompetitions.withgoogle.com/kickstart/round/0000000000050edb) | kickstart-e-2019.in | 25/08/2019(10:30) | 25/08/2019(13:30) |
| 63. | [Hackerearth August Circuits 2019](https://www.hackerearth.com/challenges/competitive/august-circuits-19/) | hackerearth-aug-circuits19.in | 24/08/2019(21:00) | 31/08/2019(21:00) |
| 64. | [Codechef August Lunchtime 2019](https://www.codechef.com/LTIME75) | codechef-aug-lunchtime19.in | 31/08/2019(20:00) | 31/08/2019(23:00) |
| 65. | [Codechef Alcoding Global Challenge](https://www.codechef.com/ALCM2019) | codechef-alcoding-global-challenge.in | 01/09/2019(21:00) | 02/09/2019(00:00) |
| 66. | [Hackerearth September Easy 2019](https://www.hackerearth.com/challenge/competitive/september-easy-19/) | hackerearth-sept-easy-2019.in | 07/09/2019(09:30) | 07/09/2019(12:30) |
| 67. | [Codechef September Long Challenge 2019](https://www.codechef.com/SEPT19) | codechef-sept19.in | 06/09/2019(15:00) | 16/09/2019(15:00) |
| 68. | [Codechef September Cookoff 2019](https://www.codechef.com/COOK110) | codechef-sept-cookoff19.in | 22/09/2019(21:30) | 23/09/2019(00:00) |
| 69. | [Hackerearth September Circuits 2019](https://www.hackerearth.com/challenges/competitive/september-circuits-19/) | hackerearth-sept-circuits19.in | 21/09/2019(21:00) | 28/08/2019(21:00) |
| 70. | [Codechef September Lunchtime 2019](https://www.codechef.com/LTIME76) | codechef-sept-lunchtime19.in | 28/09/2019(19:30) | 28/09/2019(22:30) |
| 71. | [Hackerearth October Easy 2019](https://www.hackerearth.com/challenge/competitive/october-easy-19/) | hackerearth-oct-easy-2019.in | 04/10/2019(23:00) | 05/10/2019(03:30) |
| 72. | [Codechef October Long Challenge 2019](https://www.codechef.com/OCT19) | codechef-oct19.in | 04/10/2019(15:00) | 14/10/2019(15:00) |
| 73. | [Codechef October Cookoff 2019](https://www.codechef.com/COOK111) | codechef-oct-cookoff19.in | 20/10/2019(21:30) | 21/10/2019(00:00) |
| 74. | [Hackerearth October Circuits 2019](https://www.hackerearth.com/challenges/competitive/october-circuits-19/) | hackerearth-oct-circuits19.in | 19/10/2019(21:00) | 26/10/2019(21:00) |
| 75. | [Codechef October Lunchtime 2019](https://www.codechef.com/LTIME77) | codechef-oct-lunchtime19.in | 26/10/2019(19:30) | 26/10/2019(22:30) |
| 76. | [Hackerearth November Easy 2019](https://www.hackerearth.com/challenge/competitive/november-easy-19/) | hackerearth-nov-easy-2019.in | 02/11/2019(09:30) | 02/11/2019(12:30) |
| 77. | [Codechef November Long Challenge 2019](https://www.codechef.com/NOV19) | codechef-nov19.in | 01/11/2019(15:00) | 11/11/2019(15:00) |
| 78. | [Codechef November Cookoff 2019](https://www.codechef.com/COOK112) | codechef-nov-cookoff19.in | 17/11/2019(21:30) | 18/11/2019(00:00) |
| 79. | [Hackerearth November Circuits 2019](https://www.hackerearth.com/challenges/competitive/november-circuits-19/) | hackerearth-nov-circuits19.in | 16/11/2019(21:00) | 23/11/2019(21:00) |
| 80. | [Codechef November Lunchtime 2019](https://www.codechef.com/LTIME78) | codechef-nov-lunchtime19.in | 30/11/2019(19:30) | 30/11/2019(22:30) |
| 81. | [Codechef December Long Challenge 2019](https://www.codechef.com/DEC19) | codechef-dec19.in | 06/12/2019(15:00) | 16/12/2019(15:00) |
| 82. | [Hackerearth December Easy 2019](https://www.hackerearth.com/challenge/competitive/december-easy-19/) | hackerearth-dec-easy-2019.in | 07/12/2019(09:30) | 07/12/2019(12:30) |
| 83. | [Codechef December Cookoff 2019](https://www.codechef.com/COOK113) | codechef-dec-cookoff19.in | 22/12/2019(21:30) | 23/12/2019(00:00) |
| 84. | [Hackerearth December Circuits 2019](https://www.hackerearth.com/challenges/competitive/december-circuits-19/) | hackerearth-dec-circuits19.in | 21/12/2019(21:00) | 28/12/2019(21:30) |
| 85. | [Codechef December Lunchtime 2019](https://www.codechef.com/LTIME79) | codechef-dec-lunchtime19.in | 28/12/2019(19:30) | 28/12/2019(22:30) |
| 86. | [Hackerearth January Easy 2019](https://www.hackerearth.com/challenge/competitive/january-easy-20/) | hackerearth-jan-easy-2019.in | 04/01/2020(09:30) | 04/01/2020(12:30) |
| 87. | [Codechef January Long Challenge 2020](https://www.codechef.com/JAN20) | codechef-jan20.in | 03/01/2020(15:00) | 13/01/2020(15:00) |
| 88. | [Codechef January Cookoff 2019](https://www.codechef.com/COOK114) | codechef-jan-cookoff20.in | 19/01/2020(21:30) | 20/01/2020(00:00) |
| 89. | [Hackerearth January Circuits 2020](https://www.hackerearth.com/challenges/competitive/january-circuits-20/) | hackerearth-jan-circuits20.in | 18/01/2020(21:00) | 25/01/2020(21:00) |
| 90. | [Codechef January Lunchtime 2020](https://www.codechef.com/LTIME80) | codechef-jan-lunchtime20.in | 25/01/2020(19:30) | 25/01/2020(22:30) |
| 91. | [Hackerearth February Easy 2019](https://www.hackerearth.com/challenge/competitive/february-easy-20/) | hackerearth-feb-easy-2020.in | 01/02/2020(09:30) | 01/02/2020(12:30) |
| 92. | [Codechef February Cookoff 2020](https://www.codechef.com/COOK115) | codechef-feb-cookoff20.in | 16/02/2020(21:30) | 17/02/2020(00:00) |
| 93. | [Codechef February Long Challenge 2020](https://www.codechef.com/JAN20) | codechef-feb20.in | 07/02/2020(15:00) | 17/02/2020(15:00) |
| 94. | [Hackerearth February Circuits 2020](https://www.hackerearth.com/challenges/competitive/february-circuits-20/) | hackerearth-feb-circuits20.in | 15/02/2020(21:30) | 22/02/2020(21:30) |
| 95. | [Codechef February Lunchtime 2020](https://www.codechef.com/LTIME81) | codechef-feb-lunchtime20.in | 29/02/2020(19:30) | 29/02/2020(22:30) |
| 96. | [Hackerearth March Easy 2020](https://www.hackerearth.com/challenge/competitive/march-easy-20/) | hackerearth-march-easy-2019.in | 07/03/2020(09:30) | 07/03/2020(12:30) |
| 97. | [Codechef March Long Challenge 2020](https://www.codechef.com/FEB20) | codechef-march20.in | 06/03/2020(15:00) | 16/03/2020(15:00) |
| 98. | [Google Kickstart 2020 Round A](https://codingcompetitions.withgoogle.com/kickstart/round/000000000019ffc7) | kickstart-a-2020.in | 22/03/2020(09:30) | 22/03/2019(12:30) |
| 99. | [Codechef March Cookoff 2020](https://www.codechef.com/COOK116) | codechef-march-cookoff20.in | 22/03/2020(21:30) | 23/03/2020(00:00) |
| 100. | [Hackerearth March Circuits 2020](https://www.hackerearth.com/challenges/competitive/march-circuits-20/) | hackerearth-march-circuits20.in | 21/03/2020(21:00) | 28/03/2020(21:00) |
| 101. | [Codechef March Lunchtime 2020](https://www.codechef.com/LTIME82) | codechef-march-lunchtime20.in | 28/03/2020(19:30) | 28/03/2020(22:30) |
| 102. | [Hackerearth April Easy 2020](https://www.hackerearth.com/challenge/competitive/april-easy-20/) | hackerearth-april-easy-2019.in | 04/04/2020(09:30) | 04/04/2020(12:30) |
| 103. | [Google Codejam 2020 Qualification Round](https://codingcompetitions.withgoogle.com/codejam/round/000000000019fd27) | codejam-qualification-2020.in | 04/04/2020(04:30) | 05/04/2020(07:30) |
| 104. | [Codechef April Long Challenge 2020](https://www.codechef.com/MARCH20) | codechef-mar20.in | 03/04/2020(15:00) | 13/04/2020(15:00) |
| 105. | [Google Kickstart 2020 Round B](https://codingcompetitions.withgoogle.com/kickstart/round/0000000000050e01) | kickstart-a-2020.in | 19/04/2020(04:30) | 19/04/2020(07:30) |
| 106. | [Codechef April Cookoff 2020](https://www.codechef.com/COOK117) | codechef-april-cookoff20.in | 20/04/2020(21:30) | 21/04/2020(00:00) |
| 107. | [Hackerearth April Circuits 2020](https://www.hackerearth.com/challenges/competitive/april-circuits-20/) | hackerearth-april-circuits20.in | 18/04/2020(21:00) | 25/04/2020(21:00) |
| 108. | [Codechef April Lunchtime 2020](https://www.codechef.com/LTIME83) | codechef-april-lunchtime20.in | 25/04/2020(19:30) | 25/04/2020(22:30) |
| 109. | [Hackerearth May Easy 2020](https://www.hackerearth.com/challenge/competitive/may-easy-20/) | hackerearth-may-easy-2019.in | 02/05/2020(09:30) | 02/05/2020(12:30) |