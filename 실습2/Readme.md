package Challenges;

	import java.util.Scanner;

	public class problem1 {
	    public static void main(String[] args) {
	        int result;
	        int n;
	        Scanner in = new Scanner(System.in);

	        System.out.print("팩토리얼 값을 구할 정수 : ");
	        n = in.nextInt();

	        result = 1;
	        while (n > 0) {
	            result *= n--;
	        }
	        System.out.println(result);
	    }
	}
 
- while(true)로 수정한 후 다시 실행

 package Challenges;

	import java.util.Scanner;

	public class problem2 {
	    public static void main(String[] args) {
	        int result;
	        int n;
	        Scanner in = new Scanner(System.in);

	        System.out.print("팩토리얼 값을 구할 정수 : ");
	        n = in.nextInt();

	        result = 1;
	        while (true) {
	            if (n > 0)
	                result *= n--;
	            else if (n <= 0)
	                break;
	        }
	        System.out.println(result);
	    }
	}

 package Programming;

	import java.util.Scanner;

	public class problem1 {
	    public static void main(String[] args) {
	        int age;
	        Scanner in = new Scanner(System.in);
	        System.out.print("나이를 입력하세요 : ");
	        age = in.nextInt();

	        if (age >= 19)
	            System.out.println("성년");
	        else
	            System.out.println("미성년");
	    }
	}

 package Programming;

	import java.util.Scanner;

    public class problem2 {
	    public static void main(String[] args) {
	        int n;
	        Scanner in = new Scanner(System.in);
	        System.out.print("등수를 입력하세요 : ");
	        n = in.nextInt();

	        switch (n)
	        {
	            case 1 :
	                System.out.println("아주 잘했습니다.");
	                break;
	            case 2, 3 :
	                System.out.println("잘했습니다.");
	                break;
	            case 4, 5, 6:
	                System.out.println("보통입니다.");
	                break;
	            default:
	                System.out.println("노력해야겠습니다.");
	        }
	    }
	}

 package Programming;

	import java.util.Scanner;

	public class problem3 {
	    public static void main(String[] args) {
	        int n;
	        int result = 0;
	        Scanner in = new Scanner(System.in);
	        do {
	            System.out.print("양의 정수를 입력하세요 : ");
	            n = in.nextInt();
	            if (n % 2 == 0)
	                result += n;
	        } while (n > 0);
	        System.out.println("입력한 양의 정수 중에서 짝수의 합은 " + result);
	    }
	}

 package Programming;

public class problem4 {

	    public static void main(String[] args) {
	        for (int i = 0; i < 5; i++) {
	            for (int j = 0; j <= i; j++)
	                System.out.print("*");
	            System.out.println();
	        }
	    }
	}
