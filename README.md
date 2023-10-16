# CSE330: Operating Systems 

Please follow the below steps to test your Project-2. 

- Download the zip of this git repository.
- Unzip the repository.
- Implement your kernel module code in the memory\_manager.c (i.e. all //TODO part, DO NOT change any other part).
- Run the test.sh script with the test arguments. 

## Test Cases:

| Test Case #   | Test Command  | Test Criteria  | Total Points |
| ------------- |:-------------:| :-----:|:-----:|
| 0 | free -h | The available memory size of your VM is **larger than 500MB, and smaller than 1 GB** (5 pts), your VM has enough swap spaces (e.g. Swap = 2 GB. available + Swap > 1.5 GB). (5pts) | 10 |
| 1 | sudo ./test.sh 1 | The RSS result from your kernel module output should be 100 MB (5 pts), 200 MB (5 pts), and 300 MB (5 pts), and all WSS results should be 100 MB (5 pts) | 20 |
| 2 | sudo ./test.sh 2 | The WSS result from your kernel module output should be 300 MB (5 pts), 200 MB (5 pts), and 100 MB (5 pts), and all RSS results should be 300 MB (5 pts) | 20 |
| 3 | sudo ./test.sh 3 | The RSS + SWAP results from your kernel module output should match memory pressure of 0.5 GB (5 pts), 1 GB (5 pts), and 1.5 GB (5 pts) |15|

## Note: 
- Please do not make any changes in provided test code to pass the test cases.
- You can use print statements in case you want to debug and understand the logic of the test code.
- Please get in touch with the TAs if you face issues in using the test scripts.

## Sample Output Screenshots:

### Test Case 0
![test_case_0](sample_output/test0.png)

### Test Case 1
![test_case_1](sample_output/test1.png)

### Test Case 2
![test_case_2](sample_output/test2.png)

### Test Case 3
![test_case_3](sample_output/test3.png)

