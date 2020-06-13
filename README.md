# FirstDemo
public class Calculator {
	public int getSum(int a,int b){//计算两个int类型之和
		int sun =a+b;
		
		return sun;
		
	}
	public double getSum(double a, double b ){//两个double类型之和
		double sum = a+ b;
		
		return sum;
	}
	public char transform(char x){
		int a = (int ) x;
		char b =(char)( a+32);
		return b;
		
	}
	
	public static void main(String[] args) {
		
		Calculator calculator = new Calculator();
		int sum = calculator.getSum(3, 4);//调用第一个int 类型方法
		System.out.println(sum);
		
		double sum2 = calculator.getSum(3.14, 3.14);//调用第一个double 类型方法
		System.out.println(sum2);
		
		char x = calculator.transform('A');//调用大写转小写功能
		System.out.println(x);
	}

}