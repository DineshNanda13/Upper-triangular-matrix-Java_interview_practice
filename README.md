# Upper-triangular-matrix-Java_interview_practice
Java program to convert a given matrix into Upper triangular matrix. For matrix to be converted into Upper triangular matrix, it needs to be square matrix, i.e, rows and columns needs to be equal.

package com.Utm;

/**
 *
 * @author Dinesh Nanda
 */

public class UpperTriangularMatrix {

    public static void main(String[] args) {
        
        int arr [][] = {{1,2,3}, {8,6,4}, {4,5,6}};
        
        int row = arr.length;
        int col = arr[0].length;
        
        if(row != col){
            
            System.out.println("The given matrix is not a square matrix so can't be a Upper Triangular Matrix");
            
        }else{
            
            for(int i = 0; i < row; i++){
                for(int j = 0; j < col; j++){
                    
                    if(i > j){
                        arr[i][j] = 0;
                    }
                }
            }
            for(int i = 0; i < row; i++){
                for(int j = 0; j < col; j++){
                    System.out.print(arr[i][j]+" ");
                }
                System.out.println();
            }
        }
    }
    
}
