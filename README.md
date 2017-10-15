# TxtFiletoArray
Need to make the text file into an array
/*
 * To change this license header, choose License Headers in Project Properties.
 * To change this template file, choose Tools | Templates
 * and open the template in the editor.
 */
package pkg2dimensionalarray;
import java.io.IOException;
public class Main {

    /**
     * @param args the command line arguments
     */
    public static void main(String[] args)throws IOException{
        // TODO code application logic here
        String file_name = "C:/MyTest/test.txt";
        
        
        try {
            ReadFile file = new ReadFile(file_name);
            String[] aryLines = file.OpenFile();
            
            int i;
            for (i=0; i < aryLines.length; i++) {
                System.out.println(aryLines[i]);
            }
            
        }
        
        
        catch (IOException e) {
            System.out.println( e.getMessage () );
        }
        int [][] array = new int [20][45];
        
        for (int row = 0; row < array.length; row++) {
            for (int column = 0; column < array[row].length; column++) {
                System.out.print(array[row][column] + " ");
            }
            
            System.out.println();
            
            
        }
        
        
        
        
        
        
        
    }
    
}
