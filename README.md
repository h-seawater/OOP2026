# OOP2026
### Homework1
```Java
public class Main {
	public static void main(String []args){
		int i, j;
        
		for(i = 1; i <= 10; i++) {
			for(j = 1; j <= i; j++) {
				System.out.print("#");
			}
			System.out.println("");
		}
		System.out.println("");
        
        for (i = 10; i >= 1; i--) {
        	for (j = 1; j <= i; j++) {
            	System.out.print("#");
			}
            System.out.println();
		}
    	System.out.println();
        
		for(i = 1; i <= 10; i++) {
			for(j = 1; j <= 10-i; j++) {
				System.out.print(" ");
			}
			for(j = 1; j <= i; j++) {
				System.out.print("#");
			}
			System.out.println();
		}
		System.out.println();
        
        for(i = 10; i >= 1; i--) {
			for(j = 1; j <= 10 - i; j++) {
				System.out.print(" ");
			}
			for(j = 1; j <= i; j++) {
				System.out.print("#");
			}
            System.out.println();
		}
		System.out.println();
	}
}
```
<img width="1626" height="848" alt="image" src="https://github.com/user-attachments/assets/88a7dbac-691e-40da-8801-5b163be8da5e" />


### Homework2
```Java
public class Main {
  public static void main(String[] args) {
    int f1 = 0;
    int f2 = 1;
    
	System.out.print(f1 + " " + f2 + " ");

    for (int i = 3; i <= 20; i += 1) {
	    int f3 = f1 + f2;
        System.out.print(f3 + " ");
		
        f1 = f2;
        f2 = f3;
        }
	}
}
```
<img width="1627" height="398" alt="image" src="https://github.com/user-attachments/assets/bc892195-3d8b-4261-8928-0986f4c937a0" />


### Homework3
```Java
public class Main {
	public static void main(String[] args) {
		double a = 1;
		double b = 1;
        double c;
        double result;
		
		for (int i = 3; i <= 20; i ++) {
			c = a + b;
            result = c / b;
            String resultS = String.format("%.9f", result);
            
            System.out.println((int)c + "/" + (int)b + " = " + resultS);
            
            a = b;
            b = c;
		}
	}
}
```
<img width="1628" height="411" alt="image" src="https://github.com/user-attachments/assets/71026245-3b91-4c3b-959b-2ebf63b76650" />


### Homework4
```Java
public class Main {
	public static void main(String[] args) {
    
		for (int i = 1; i <= 9; i++) {
			for (int j = 1; j <= 9; j++) {
				System.out.print(i + "*" + j + "=" + i*j + " ");
			}
            System.out.println();
		}
	}
}
```
<img width="1627" height="336" alt="image" src="https://github.com/user-attachments/assets/43dca2b3-666f-43b5-aff5-dbae41517753" />


### Homework5
```Java
public class Main {
  public static void main(String[] args) {
    double sum = 0.0;
    int sign = 1;
    
    for (int i = 1; i <= 10000; i+=2) {
	    sum += sign * (4.0 / i);
	    sign = -sign;
		}
  	System.out.println(sum);
	}
}
```
<img width="1627" height="536" alt="image" src="https://github.com/user-attachments/assets/a465afc6-d12e-4c9b-9ef5-3e7e88b0ee3b" />


### Homework6
```Java
public class Main {
	public static void main(String[] args) {
    
		int binomial[][] = new int[10][10];
        
        for (int i = 0; i < 10; i++) {
        	
        	binomial[i][0] = 1;
            binomial[i][i] = 1;
            
        	for (int j = 1; j < i; j++) {
            	binomial[i][j] = binomial[i-1][j-1] + binomial[i-1][j];
            }
        }
        
        for (int i = 0; i < 10; i++) {
			for (int j = 0; j <= i; j++) {
            	System.out.print(binomial[i][j] + " ");
            }
            System.out.println();
        }
	}
}
```
<img width="1624" height="426" alt="image" src="https://github.com/user-attachments/assets/5cc28b3d-dd71-4463-a4bc-556263c75d69" />


### Homework7
```Java
public class Main {
	public static void main(String[] args) {
    
		for (int i = 1; i <= 9; i++) {
			for (int j = 1; j <= 9; j++) {
				System.out.print(i + "*" + j + "=" + i*j + " ");
			}
            System.out.println();
		}
	}
}
```
<img width="1627" height="336" alt="image" src="https://github.com/user-attachments/assets/43dca2b3-666f-43b5-aff5-dbae41517753" />


