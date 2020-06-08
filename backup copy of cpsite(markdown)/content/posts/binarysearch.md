---
title: Binary Search
date: 2020-06-03T14:21:26+08:00
#lastmod: 2020-06-03T22:02:47+08:00
author: Sabbir
#cover: /img/notready.gif
cover: https://user-images.githubusercontent.com/64752426/83613786-1a24e080-a5a6-11ea-9621-057c8b252f61.jpg
categories:
  - Algorithm
tags:
  - algo
---
# :pushpin: CODE-LIBRARY:

```c++
  //  author:  MSA
int BinarySearch(int a[],int n,int target)
{
	int low=0, high =n-1;
	while(low<=high)
	{
		int mid=low+(high-low)/2;  // best formula to ignore overflow

		if(target==a[mid]) return mid; //mid element is the ans

		else if(a[mid]<target)    low=mid+1; //moving to right side

		else   high=mid-1; // moving to left side
	}
	return -1;  //no value found
}

```

# :pushpin: VIDEO-TUTORIALS :
## 1. [mycodeschool](https://www.youtube.com/playlist?list=PL2_aWCzGMAwL3ldWlrii6YeLszojgH77j)
## 2. [Errichto](https://www.youtube.com/watch?v=GU7DpgHINWQ)
## 3. [AfterAcademy](https://www.youtube.com/watch?v=wwAnGDx2f48)   
## 4. [Nick White](https://www.youtube.com/watch?v=QdVrY3stDD4)
# :pushpin: PDF-TUTORIALS :
## 1. [**Binary Search**](https://drive.google.com/file/d/0B1yhFrxtsDsyLTdDUTZMSUV6RzA/view) >>>>>>>>>>:man_technologist: [I_Love_Equinox](https://codeforces.com/profile/I_Love_Equinox)

# :pushpin: SCREENSHOT-BREAKDOWN :
### 1. Iterative Binary Search -  [Method -01]::
#### source: [mycodeschool](https://www.youtube.com/playlist?list=PL2_aWCzGMAwL3ldWlrii6YeLszojgH77j)
-------------------------------------------
```
mid=(low+high)/2
```
![bin1](https://user-images.githubusercontent.com/64752426/83613210-4c820e00-a5a5-11ea-8ae0-6d888754679f.png)

### 2.  Iterative Binary Search -  [Method -02]::
-------------------------------------------
```
mid=low+(high-low)/2
```
#### source: [mycodeschool](https://www.youtube.com/playlist?list=PL2_aWCzGMAwL3ldWlrii6YeLszojgH77j)

![bin2](https://user-images.githubusercontent.com/64752426/83614216-b8b14180-a5a6-11ea-811e-817f0415bd88.png)

#### source: [Errichto](https://www.youtube.com/watch?v=GU7DpgHINWQ)

![bin12](https://user-images.githubusercontent.com/64752426/83642505-be238180-a5d0-11ea-9e2e-647ee71eea92.png)


### 3. (Iterative *vs*  Recursive) Binary Search::
#### source: [mycodeschool](https://www.youtube.com/playlist?list=PL2_aWCzGMAwL3ldWlrii6YeLszojgH77j)
-------------------------------------------
![bin3](https://user-images.githubusercontent.com/64752426/83614467-0d54bc80-a5a7-11ea-835f-0419a0b14fc9.png)

### 4. First occurrence of a number using  Binary Search::
#### source: [mycodeschool](https://www.youtube.com/playlist?list=PL2_aWCzGMAwL3ldWlrii6YeLszojgH77j)
-------------------------------------------
```
if(x==A[mid])
{
  result=mid;
  high=mid-1;
}
```
![bin4](https://user-images.githubusercontent.com/64752426/83621338-5b21f280-a5b0-11ea-9509-ae86fae9c0aa.png)

### 5. Last occurrence of a number using  Binary Search::
#### source: [mycodeschool](https://www.youtube.com/playlist?list=PL2_aWCzGMAwL3ldWlrii6YeLszojgH77j)
-------------------------------------------
```
if(x==A[mid])
{
  result=mid;
  low=mid+1;
}
```
![bin5](https://user-images.githubusercontent.com/64752426/83621716-dc798500-a5b0-11ea-8669-49e8c46e3ace.png)

### 6. Count occurrences of a number in a sorted array using Binary Search
#### source: [mycodeschool](https://www.youtube.com/playlist?list=PL2_aWCzGMAwL3ldWlrii6YeLszojgH77j)
-------------------------------------------
```
//array is sorted so at the beginning  find  the first and last element then
(last element-first element)+1
```
![2](https://user-images.githubusercontent.com/64752426/83625381-a5f23900-a5b5-11ea-8d81-b2fcc8b30a46.png)
![3](https://user-images.githubusercontent.com/64752426/83625417-b4d8eb80-a5b5-11ea-907d-ca10e57eb611.png)

### 7. Rotated Sorted Array
-------------------------------------------
#### source: [AfterAcademy](https://www.youtube.com/watch?v=wwAnGDx2f48)   
![bin14](https://user-images.githubusercontent.com/64752426/83667717-a52ac880-a5f0-11ea-8c5f-e8080e18d3e0.png)

#### source: [Nick White](https://www.youtube.com/watch?v=QdVrY3stDD4)   
![bin13](https://user-images.githubusercontent.com/64752426/83655132-d8189080-a5df-11ea-92c3-a7c85665fa5b.png)
<!---
#### source: [mycodeschool](https://www.youtube.com/playlist?list=PL2_aWCzGMAwL3ldWlrii6YeLszojgH77j)
```
//pivot property---- next and previous both are greater
//duplicate element is not possible in this case
```
![1](https://user-images.githubusercontent.com/64752426/83633089-346cb780-a5c2-11ea-89bc-d7871b89c550.png)
>Code:

![2](https://user-images.githubusercontent.com/64752426/83633148-49e1e180-a5c2-11ea-9db0-37683ba80e73.png)

-->

<!---

### 8. Search element in a circular sorted array
#### source: [mycodeschool](https://www.youtube.com/playlist?list=PL2_aWCzGMAwL3ldWlrii6YeLszojgH77j)
-------------------------------------------

![bin10](https://user-images.githubusercontent.com/64752426/83640293-c1693e00-a5cd-11ea-9921-c9144e830879.png)
![bin11](https://user-images.githubusercontent.com/64752426/83640215-a72f6000-a5cd-11ea-96e0-68e3473f9b92.png)
--->
