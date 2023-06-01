# practiceJava
Реализуйте метод, принимающий в качестве аргумента целочисленный массив. 
Если длина массива меньше некоторого заданного минимума, метод возвращает -1, в качестве кода ошибки, иначе - длину массива

//ch
public class ArrayLengthChecker {
    public static int checkArrayLength(int[] array, int minimumLength) {
        if (array.length < minimumLength) {
            return -1;
        } else {
            return array.length;
        }
    }
    public static void main(String[] args) {
        int[] myArray = {1, 2, 3, 4, 5};

        int minimumLength = 5;
        int result = checkArrayLength(myArray, minimumLength);

        if (result == -1) {
            System.out.println("Ошибка: длина массива меньше заданного минимума.");
        } else {
            System.out.println("Длина массива: " + result);
        }
    }
}
//семинар 1 задача 1 

package Praktika;
public class Main {
    public static void main(String[] args) {
        int[] massiv = new int[2];
        for (int i = 0; i < massiv.length; i++) {
            massiv[i] = i +2;
        }
        System.out.println(f1(massiv));
    }
    public static int f1(int[] massiv){
        if (massiv.length < 5){
            return -1;
        }
        return massiv.length;
    }
}
