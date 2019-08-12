 *Assisted by and Assisted line numbers: Dr.Su lines 51-58, 80, 88, 92, 94
 
 * Matthew Young
 
 * mey5087
 
 * CMPSC122 Semester 2018
 
 * 11:59, Wednesday, 13, 2018
 
 * 10:00, Wednesday, 13, 2018
 
 * This program will find the number of northeast paths between two points using a recursive function. It will
 * also time how fast it takes to get the result.
 
 */








#include <iostream>
#include "timer.h" // Was given during project, is not included on GitHub.

using namespace std;




int path(int length, int width){
    
    if (length == 1 && width == 0) {
        return 1;
    }
    
    else if (length == 0 && width == 1){
        return 1;
    }
    
    else if (length == 0 || width == 0){
        return 1;
    }
    
    else {
        return path(length, width - 1) + path(length - 1, width);
    }
}





int main() {
    
    int northPts;
    int eastPts;
    char runProg;
    
    Timer t;

    cout << "How many points North of A is B? ";
    cin >> northPts;
    
    cout << "How many points East of A is B? ";
    cin >> eastPts;
    
    t.start();
    
    cout << "There are " << path(northPts, eastPts) << " northeast paths between A and B." <<  endl << endl;
    
    t.stop();
    
    t.show();
    
    cout << "Enter Y to continue to the next example or press any other letter to exit: ";
    cin >> runProg;
    
    while (runProg == 'Y'){
        
        cout << endl;
        
        cout << "How many points North of A is B? ";
        cin >> northPts;
        
        cout << "How many points East of A is B? ";
        cin >> eastPts;
        
        t.start();
        
        cout << "There are " << path(northPts, eastPts) << " northeast paths between A and B." <<  endl << endl;
        
        t.stop();
        
        t.show();
        
        cout << "Enter Y to continue to the next example or press any other letter to exit: ";
        cin >> runProg;
        
        if (runProg != 'Y') {
            return 0;
        }
    }
    
    if (runProg != 'Y') {
        return 0;
    }
    
}
