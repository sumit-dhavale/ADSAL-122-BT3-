// Implement the problem of moving all zeroes to the end of array. 
// Statement: Given an array of random numbers, Push all the zeroes of a 
// given array to the end of the array. 


#include<iostream>
#include<vector>
using namespace std;
void mergestep(int array[],int start,int mid,int end)
{
    vector<int>temp;
    int i=start;
    int j=mid+1;
   while(i<=mid&&j<=end)
   {
    if(array[i]>=array[j])
    {
        temp.push_back(array[i]);
        i++;
    }
    else{
        temp.push_back(array[j]);
        j++;
    }
    }
    
   while(i<=mid)
   {
    temp.push_back(array[i]);
    i++;
   }
   while(j<=end)
   {
    temp.push_back(array[j]);
    j++;

   }

   for(int i=0;i<temp.size();i++)
   {
    array[i+start]=temp[i];
   }

}
void merge(int array[],int start,int end)
{
if(start<end)
{
    int mid=(end+start)/2;
    merge(array,start,mid);
    merge(array,mid+1,end);
    mergestep(array,start,mid,end);

}

}
int main()
{
    int array[10]={1,3, 4 ,0, 5, 6};
    merge(array,0,5);
        for(int i=0;i<6;i++)
    {
        cout<<array[i]<<" ";
    }

}
