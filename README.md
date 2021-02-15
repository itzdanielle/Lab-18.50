# Lab-18.50
#include <iostream>
#include <iomanip>
using namespace std;

int getWins () {
  int wins;
  cout << "Please input the number of wins" << endl;
  cin >> wins;
  return wins;
}
int getLosses() {
  int losses;
  cout << "Please input the number of losses" << endl;
  cin >> losses;
  return losses;
}
double calcWinPercent(int wins, int losses) {
  double result;
  result = (wins)/(wins + losses);
  return result;
  
}
void displayWinPercent (double calcWinPercent ) {
  double result;
  result = calcWinPercent;
  cout << "The percentage of wins is " << result << endl;
  
}

int main() {
  cout << setprecision(2) << fixed;
  int wins, losses;
  wins = getWins();
  losses = getLosses();
  double result;
  result = calcWinPercent(wins,losses);
  displayWinPercent(result);
  
}
