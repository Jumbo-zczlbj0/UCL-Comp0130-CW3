# Robot-Vision-and-Navigation-CW3
COMP0130

# Reference
https://github.com/sjulier/Refactored_ORB_SLAM2

# Code Modification
For Part 2, change the YAML file. ORBextractor.nFeatures: 

For Part 3, 
1. Tracking.cc

comment line 415-418; 

2. Optimizer.cc 

line 362 and 363 

const float chi2Mono[4] = {5.991, 5.991, 5.991, 5.991};

const float chi2Stereo[4] = {7.815, 7.815, 7.815, 7.815};

Replaced by 

const float chi2Mono[4] = {13.82, 13.82, 13.82, 13.82};

const float chi2Stereo[4] = {16.27, 16.27, 16.27, 16.27};

3. LocalMapping.cc

line 346 356 370 380

replaced by 13.82 or 16.27

For Part 4,

comment line 66

# Folder explanation

gt refers to ground truth

ref refers to references

estimate contains camera trajectory estimation

fig refers to figures

# Code Understanding
程序中变量名的第一个字母如果为"m"则表示为类中的成员变量，member
第一个、第二个字母:
"p"表示指针数据类型
"n"表示int类型
"b"表示bool类型
"s"表示set类型
"v"表示vector数据类型
'l'表示list数据类型
"KF"表示KeyPoint数据类型
