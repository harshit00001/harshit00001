- 👋 Hi, I’m @harshit00001
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
harshit00001/harshit00001 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
package Test1;

import java.util.Scanner;

public class CountRepeatWord 
{
	public static void main(String[] args) 
	{
		Scanner sc=new Scanner(System.in);
		System.out.println("Enter the String: ");
		String str=sc.nextLine();
		
		for(int i=0;i<str.length();i++)
		{
			int count=1;
			while(i+1<str.length() && str.charAt(i)==str.charAt(i+1))
			{
				i++;
				count++;
			}
			System.out.print( str.charAt(i) + "" + count +"" );
		}
	}
}

package Test1;

import java.util.Scanner;

public class SpiralMatrix {

	public static void main(String[] args) {
		Scanner sc=new Scanner(System.in);
		System.out.println("Enter the m * n matrix : " );
		int[][] arr=new int[sc.nextInt()][sc.nextInt()];
		int k,count=1,row=arr.length,colm=arr[1].length,rowindex=0,columnindex=0;
		
		for(int i=0;i<arr.length;i++)
		{
			for(int j=0;j<arr[i].length;j++)
			{
					arr[i][j]=count;
					count++;
					System.out.print(arr[i][j]+" ");
			}
			System.out.println();
		}
		
		while(rowindex<row && columnindex<colm)
		{
			
			for(k=columnindex;k<colm;++k)
			{
				System.out.print(arr[rowindex][k]+" ");
			}
			rowindex++;
			for(k=rowindex;k<row;++k)
			{
				System.out.print(arr[k][colm-1]+" ");
			}
			colm--;
			if(rowindex<row)
			{
				for(k=colm-1;k>=columnindex;--k)
				{
					System.out.print(arr[row-1][k]+" ");
				}
				row--;
			}
			if(columnindex<colm)
			{
				for(k=row-1;k>=rowindex;--k)
				{
					System.out.print(arr[k][columnindex]+" ");
				}
				columnindex++;
			}
		}	
	}
}
