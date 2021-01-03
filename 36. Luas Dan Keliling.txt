import java.util.*;

class Main {
  public static void main(String[] args) {
    
        Scanner userInput = new Scanner(System.in);
        
        double inputPanjang = userInput.nextDouble();
        double inputLebar = userInput.nextDouble();
        tampilkanKelilingDanLuas(inputPanjang, inputLebar);
    }
    public static void tampilkanKelilingDanLuas(double panjang, double lebar){
        System.out.println(luas(panjang, lebar));
        System.out.println(keliling(panjang, lebar));
    }

    public static double keliling(double panjang, double lebar){
        double hasil = (panjang + lebar) * 2;
        return hasil;
    }

    public static double luas(double panjang,double lebar){
        double hasil = panjang * lebar;
        return hasil;
    
  }
}