# secondlargestnum

package com.company;

import java.util.Arrays;

public class Main {
    public static void main(String[] args){
        int[] arr ={1,2,13,462,52};
        max(arr);
        System.out.print("The second largest number is:");
        System.out.println(man(arr));

    }
    public static int max(int[] arr){
        int a =0,b=0;
        for (int i=0;i<arr.length;i++) {
            if (arr[i] > a) {
                a = arr[i];
                b = i;
            }
        }
    return sec(arr,b);
    }
    public static int sec(int[] arr,int b){
        arr[b] = 0;
        //System.out.println(Arrays.toString(arr));
        return arr[b];
    }
    public static int man(int[] arr){
        int a=0;
        for(int i=0;i< arr.length;i++){
            if(arr[i]>a)
                a=arr[i];
        }
        return a;
    }
}
