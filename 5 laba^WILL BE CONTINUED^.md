package com.company;
import java.util.Scanner;
public class Main
{

	public static void main(String[] args)
	{
		int MatrixSize;
		int low,high;
		Scanner scanner = new Scanner(System.in);
		System.out.println("Размер матрицы:N*N");
		System.out.println("Введите N");
		MatrixSize = scanner.nextInt();
		System.out.println("Введите диапазон, где первое поле-нижняя граница , а второе поле-верхняя");
		low = scanner.nextInt();
		high = scanner.nextInt();
		int [] nottmatrix = new int[(int) Math.pow(MatrixSize,2)];
		System.out.print("Не транспонированная матрица:");
		for (int x = 0; x < nottmatrix.length; x++)
		{
			nottmatrix[x] =(int)(Math.random()*(high-low)) + low;
			System.out.print(nottmatrix[x]+" ");
		}
int [] tmatrix = new int [(int) Math.pow(MatrixSize,2)];
System.out.println(" ");
		System.out.print("Транспонированная матрица:");
		for (int a = 0; a<tmatrix.length;a++)
		{
			{
				tmatrix[a]=nottmatrix[a];
			}
			tmatrix[a]=nottmatrix[a];
			System.out.print("!"+tmatrix[a]);
		}
