package homework1;

public class problem1 {

	public static void main(String[] args) {
        System.out.println("     *     ");
        System.out.println("    ***    ");
        System.out.println("   *****   ");
        System.out.println("  *******  ");
        System.out.println(" ********* ");
        System.out.println("***********");
    }
}

package homework1;

	import java.util.Scanner;

	public class problem2 {
	    public static void main(String[] args) {
	        int n;
	        Scanner in = new Scanner(System.in);
	        System.out.print("정수를 입력하세요 : ");
	        n = in.nextInt();
	        System.out.println(n + "의 제곱은 " + n*n);
	    }
	}

 package homework1;

	import java.util.Scanner;

	public class problem3 {
	    public static void main(String[] args) {
	        double radius, h, area;
	        Scanner in = new Scanner(System.in);
	        System.out.print("원기둥의 밑면 반지름은? ");
	        radius = in.nextDouble();
	        System.out.print("원기둥의 높이는? ");
	        h = in.nextDouble();
	        area = radius * radius * 3.14 * h;
	        System.out.println("원기둥의 부피는 " + area);
	    }
	}

 package homework1;

	import java.util.Scanner;

	public class problem4 {
	    public static void main(String[] args) {
	        int n;
	        Scanner in = new Scanner(System.in);
	        System.out.print("초 단위 정수를 입력하세요 : ");
	        n = in.nextInt();
	        int s = n % 60;
	        int m = (n / 60) % 60;
	        int h = (n / 60) / 60;
	        System.out.println(h + "시간 " + m + "분 " + s + "초");
	    }
	}

package homework1;

	import java.util.Scanner;

	public class problem5 {
	    public static void main(String[] args) {
	        char c = 'a'; 
	        char C = 'A'; 
	        int n = (int)c - (int)C; 
	        System.out.println("소문자" + c + " -> 대문자" + (char)(c-n));

	        char a, A;
	        Scanner in = new Scanner(System.in);
	        System.out.print("소문자를 입력하세요 : ");
	        a = in.next().charAt(0); 
	        A = (char)((int)a - 32);
	        System.out.println("소문자" + a + "를 대문자로 변환하면? " + A);
	    }
	}

 package homework1;

import java.util.Scanner;

public class problem6 {
    public static void main(String[] args) 
    {
	double F;
        Scanner in = new Scanner(System.in);
        System.out.print("화씨온도를 입력하세요 : ");
        F = in.nextDouble();
        double C = 5.0 / 9.0 * (F - 32);
        System.out.println("화씨온도 " + F + "-> 섭씨온도 " + C);
    }
}

package homework1;

import java.util.Scanner;

public class problem7 {
    public static void main(String[] args) {
        int x;
        Scanner in = new Scanner(System.in);
        System.out.print("정수를 입력하세요 : ");
        x = in.nextInt();
        boolean one = (x % 4 == 0) && (x % 5 == 0);
        boolean two = (x % 4 == 0) || (x % 5 == 0);
        boolean three = (x % 4 == 0 || x % 5 == 0) && !(x % 4 == 0 && x % 5 == 0);
        System.out.println("4와 5로 나누어지는지 : " + one);
        System.out.println("4 또는 5로 나누어지는지 : " + two);
        System.out.println("4나 5 중 하나로 나누어지지만 두 수 모두로는 나누어지지 않는지 : " + three);
    }
}

package homework1;

import java.util.Scanner;

public class problem8 {
    public static void main(String[] args) {
        int n;
        Scanner in = new Scanner(System.in);
        System.out.print("0~999 사이의 숫자를 입력하세요 : ");
        n = in.nextInt();
        System.out.printf("각 자릿수의 합 = %d\n", n/100 + (n%100)/10 + (n%100)%10);
    }
}

package homework1;

import java.util.Scanner;

public class problem9 {
    public static void main(String[] args) {
        int n1, n2, n3;
        Scanner in = new Scanner(System.in);
        System.out.print("전공 이수 학점 : ");
        n1 = in.nextInt();
        System.out.print("교양 이수 학점 : ");
        n2 = in.nextInt();
        System.out.print("일반 이수 학점 : ");
        n3 = in.nextInt();

        System.out.println((n1+n2+n3 >= 140 && ((n1>=70 && ((n2>=30&&n3>=30) || (n2+n3>=80)))))?"졸업 가능":"졸업 불가능");
    }
}
