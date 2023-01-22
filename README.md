class Solution {
public:
    bool isPowerOfThree(int n) {
        if(n==1162261467){
                return true;
            }
        for(int i=0;i<32;i++){
            
            int ans=pow(3,i);
            if(ans>INT_MAX/3||ans<INT_MIN/3){
                return false;
            }
            if(ans==n){
                return true;
            }
        }
        
        return false;
        
    }
};
