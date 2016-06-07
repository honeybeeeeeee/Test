# Test
class Solution {
public:
    double Power(double base, int exponent) {
    	if(0.0==base&&0==exponent){
            return 1.0;
        }
        if(0.0!=base&&0==exponent){
            return 1.0;
        }
        double result=base;
        if(exponent<0){
            for(int i=-exponent;i>1;--i){
                result*=base;
            }
            result=1.0/result;
        }
        else{
            for(int i=exponent;i>1;--i){
                result*=base;
            }
        }
        return result;
    }
};
