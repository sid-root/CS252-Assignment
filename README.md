# Multithreaded Sorting Application

## Description
Write a multithreaded sorting program that works as follows: A list of integers is divided into two smaller lists of equal size. Two separate threads (which we will term sorting threads) sort each sublist using a sorting algorithm of your choice. The two sublists are then merged by a third thread — a merging thread — which merges the two sublists into a single sorted list.

## Basic Idea
First divide the array into two subarrays or 2 parts, each of which is then sorted by an individual thread. Create Another thread to merge the 2 sorted parts to make one complete sorted array.

## Details
### Sorting
void* partoflist1(int arr[]){
    sleep(1);

    // bubble sort algorithm to sort an array
    for(int i=0;i<ps1;i++){
        for(int j=0;j<ps1-i-1;j++){
            if(arr[j]>arr[j+1]){
                int temp=arr[j];
                arr[j]=arr[j+1];
                arr[j+1]=temp;
            }
        }
    }

    // Print the sorted part of the list
    printf("Sorted Part 1 of the list :- ");
    for(int i=0;i<ps1;i++){
        b[i]=arr[i];
        printf("%d ",arr[i]);
    }
    printf("\n");
    pthread_exit(NULL);
}
