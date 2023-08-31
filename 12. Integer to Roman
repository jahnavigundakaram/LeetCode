class Solution {
public:
    int divisor[13] = {1000,900,500,400,100,90,50,40,10,9,5,4,1};
    string roman[13] = {"M","CM","D","CD","C","XC","L","XL","X","IX","V","IV","I"};
    
    string intToRoman(int num) {
        string ans;
        for(int i=0;i<13;i++){
            int numerator = 0;
            numerator = num/divisor[i];
            //cout << divisor[i] << " " << numerator <<" " << roman[i]<< endl;
            while(numerator--){
                ans += roman[i];
            }
               num%=divisor[i];
        }
        
        return ans;
    }
};
