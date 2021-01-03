import java.util.*;

class Main {
  public static void main(String[] args) {
   int baris, kolom, ganjil = 0;
        Scanner input = new Scanner(System.in);
        baris = input.nextInt();
        kolom = input.nextInt();
        int nilai[][] = new int[baris][kolom];
        for (int i = 0; i < baris; i++)
        {
            for (int j = 0; j < kolom; j++)
            {
                nilai[i][j] = input.nextInt();
            }
        }
        for(int b = 0; b < baris; b++){
            ganjil = 0;
            for(int k = 0; k < kolom; k++){
                if(nilai[b][k] % 2 != 0) {
                    ganjil++ ;
                }
            }
            System.out.println(ganjil);
        }
  }
}