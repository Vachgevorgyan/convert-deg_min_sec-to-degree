# convert-deg_min_sec-to-degree
converting
#include <iostream>

int main(void)
{
    using namespace std;
 const float deg_per_min = 60;
 const float min_per_sec = 3600;
 int deg;
 int min;
 int sec;
 cout << "Enter a latitute in degrees, minutes and secundes." << endl;
 cout << "First enter the degrees:" << endl;
 cin >> deg;
 cout <<"Next enter the minutes of arc:"<< endl;
 cin >> min;
 cout <<"Finally, enter the secundes of arc:" << endl;
 cin >> sec;
 auto result = min / deg_per_min;
 auto result1 = sec / min_per_sec;
 auto result2 = deg + result + result1;
 
 cout << deg << " degrees," << min << "minuts," << sec << " seconds =" << result2 << " degrees";
 return 0;
 
}
