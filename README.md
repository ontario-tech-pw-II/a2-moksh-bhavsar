## Copy File programs

Leaning outcomes highlights: 
- using command line arguments
- file operations

**Problem:** Write a program to get the two file name as command-line arguments and create/copy the first file contents to the second file. The name of the program is mycp.cpp, so the execution should be like:

./mycp file1 file2 (create file 2 and copy file1 contents to the file 2)

your program should check if a user provided enough arguments and print an appropriate message.

```C++
int main(int argc, char const *argv[])
{
 	ifstream fin;
 	ofstream fout;
	
	// check if there are enough arguments
	
	
	// open the first file
 	
	char c;

 	if (fin.fail()) // check if it is successful 
 	{
 		cerr << " Cannot open the input file!" << endl;
 		return 1;
 	}
 	

	// open the second file
	
 	if (fout.fail())
 	{
 		cerr << " Cannot open the output file!" << endl;
 		return 1;
 	}
 	
 	while(fin.get(c)) 
	{
		fout << c;
	}
 	
 	fin.close(); 

 	fout.close();

 	 return 0;

 } 
```
