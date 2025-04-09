- 👋 Hi, I’m @Anusha-narra
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...

<!---
Anusha-narra/Anusha-narra is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
#include <cmath>
#include <cstdio>
#include <vector>
#include <iostream>
#include <algorithm>
using namespace std;


int findMissingNumber(vector<int>&nums){
    int n=100; 
    int totalSum=n*(n+1)/2; 
    int sum=0;

    for (int num:nums){
        sum+=num;
    }

    return totalSum-sum;
}

int main(){
    vector<int>nums(99);

    for (int i=0;i<99;i++){
        cin>>nums[i];
    }
    cout<<findMissingNumber(nums)<<endl;

    return 0;
}
