# assignment3
#include<stdio.h>

#include<stdlib.h>

#include<unistd.h>

#include<sys/types.h>

#include<string.h>
#include<sys/wait.h>

int main(){
int arr[1000],sum=0;
for(int i=0;i<1000;i++)
{
    arr[i]=i;
}
int cpid=fork();
if(cpid==0){
    for(int j=0;j<100;j++){
        sum=sum+arr[j];
    }
    exit();
}
else{
    wait();
    int cpid1=fork();
    if(cpid2==0){
        for(int k=100;k<200;k++){
            sum=sum+arr[k];
        }
        exit();
    }
    else {
        wait();
        int cpid2=fork();
        if(cpid2==0){
            for(int l=200;l<300;l++){
                sum=sum+arr[l];
            }
            exit();
        }
        else 
        {
            wait();
            int cpid3=fork();
            if(cpid3==0){
                for(int m=300;m<400;m++){
                    sum=sum+arr[m];
                }
                exit();
            }
            else{
                wait();
                int cpid4=fork();
            if(cpid4==0){
                for(int n=400;n<500;n++){
                    sum=sum+arr[n];
                }
                exit();
             }
             else{
                 wait();
                int cpid5=fork();
            if(cpid5==0){
                for(int o=500;o<600;o++){
                    sum=sum+arr[o];
                }
                exit();
             }
             else{
                 wait();
                int cpi64=fork();
            if(cpid6==0){
                for(int p=600;p<700;p++){
                    sum=sum+arr[p];
                }
                exit();
             }
             else
             {
                wait();
                int cpid7=fork();
            if(cpid7==0){
                for(int q=700;q<800;q++){
                    sum=sum+arr[q];
                }
                exit();
             }
             else{
                wait();
                int cpid8=fork();
            if(cpid8==0){
                for(int r=800;r<900;r++){
                    sum=sum+arr[r];
                }
                exit();
             }
             else
             {
                 wait();
                
                for(int s=900;s<1000;s++){
                    sum=sum+arr[s];
                }
             }
            }
           }
                 
          }
         }
        }
       }
      }
     }
    printf("Sum = %d",sum);
    return 0;
                
                
            
        
}

