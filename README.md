# OOP2026

## 목차
1. [1주차 - 1~4](#homework1)
2. [2주차 - 5~12](#homework5)

---

https://drive.google.com/open?id=1Axmj5sCgHwMKalN_4J5sSMNLaU7z30y2y-uXn6oQTjQ
https://www.programiz.com/java-programming/online-compiler/

<details>
<summary>1주차 - 1~4</summary>
	
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
</details>

<details>
<summary>2주차 - 5~12</summary>
	
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
<img width="1624" height="426" alt="스크린샷 2026-09-08 155352" src="https://github.com/user-attachments/assets/e7975215-33c5-4b80-9c51-ff0742290b8b" />


### Homework7
```Java
public class Main {
	public static void main(String[] args) {
    
		int data[] = new int[20];
        
        for(int i=0; i<20; i++) {
            data[i]=(int)(Math.random()*100);
        }
        for(int i=0; i<20; i++) {
            System.out.print(data[i] + " ");
        }
        System.out.println();
        
        
        for (int i = 0; i < 19; i++) {
            int min = i;
            
			for (int j = i+1; j < 20; j++) {
            	if (data[j] < data[min]) {
                    min = j;
                }
            }
            
            int temp = data[i];
            data[i] = data[min];
            data[min] = temp;
        }
        
        for (int i = 0; i < 20; i++) {
            System.out.print(data[i] + " ");
        }
        System.out.println();
	}
}
```
<img width="1534" height="606" alt="image" src="https://github.com/user-attachments/assets/056c1a1e-6299-47ed-b7ee-31797583bfe7" />

### Homework7
```Java
public class Main {
	public static void main(String[] args) {
	    
		int score[][] = new int[30][6];
        
        for (int i = 0; i <= 29; i++) {
        	for (int j = 0; j < 5; j++) {
        		score[i][j] = (int)(Math.random() * 101);
        	}
        	score[i][0] = i+1;
        	
        	score[i][5] = score[i][1] + score[i][2] +score[i][3] +score[i][4];
        }
        for (int i = 0; i < 30; i++) {
        	for (int j = 0; j < 5; j++) {
        		System.out.print(score[i][j] + "\t");
        	}
        	System.out.println();
        }
	}
}
```
<img width="1047" height="488" alt="image" src="https://github.com/user-attachments/assets/14f4bb6c-afcd-45c1-9872-1430dbb1e541" />

</details>
