# Linux_Master_1st
임베디드 리눅스 시스템을 중심으로 학습하고 이와 더불어 리숙스 마스터 1급 필기 및 실기 대비

### goorm ide linux kernel에서 명령어 정리

~~~
root@goorm:/workspace/linux# mkdir minwoo
root@goorm:/workspace/linux# ls
README.md  goorm.manifest  index.py  minwoo
root@goorm:/workspace/linux# cd minwoo
root@goorm:/workspace/linux/minwoo# pwd  : print working directory
/workspace/linux/minwoo
~~~


기억을 되살려서 빠르게 다양한 명령어를 쭉 복습하기

~~~
   1  cd /workspace/linux; clear
    2  mkdir minwoo
    3  ls
    4  cd minwoo
    5  pwd
    6  ls
    7  touch test.py
    8  ls
    9  ls -al
   10  ll
   11  clear
   12  log
   13  ls
   14  history
   15  vi tes.py
   16  ls
   17  vi test.py
   18  ls
   19  cat test.py
   20  echo "hello world"
   21  echo "hello world" >> test.py
   22  ls
   23  cat test.py
   24  more test.py
   25  cp test.py test2.py
   26  ls
   27  rm test.py
   28  ls
   29  ls -al > result.txt
   30  ls
   31  mv result.txt ../
   32  ls
   33  cd ..
   34  ls
   35  cd minwoo
   36  ls -al
~~~

##### touch, | (operator), grep
~~~
root@goorm:/workspace/linux/minwoo# mkdir -p one/two/three
root@goorm:/workspace/linux/minwoo# ls
one
root@goorm:/workspace/linux/minwoo# mkdir one;cd one
mkdir: `one' 디렉토리를 만들 수 없습니다: 파일이 있습니다
root@goorm:/workspace/linux/minwoo/one# touch sample.txt
root@goorm:/workspace/linux/minwoo/one# ls
sample.txt  two
root@goorm:/workspace/linux/minwoo/one# cat sample.txt
root@goorm:/workspace/linux/minwoo/one# ls
sample.txt  two
root@goorm:/workspace/linux/minwoo/one# ls
sample.txt  two
root@goorm:/workspace/linux/minwoo/one# cat sample.txt | grep "P
ython"

Python is a high-level, general-purpose programming language. Its design philosophy emphasizes code readability with the use of significant indentation.[33]

Python is dynamically typed and garbage-collected. It supports multiple programming paradigms, including structured (particularly procedural), object-oriented and functional programming. It is often described as a "batteries included" language due to its comprehensive standard library.[34][35]

Guido van Rossum began working on Python in the late 1980s as a successor to the ABC programming language and first released it in 1991 as Python 0.9.0.[36] Python 2.0 was released in 2000. Python 3.0, released in 2008, was a major revision not completely backward-compatible with earlier versions. Python 2.7.18, released in 2020, was the last release of Python 2.[37]

Python consistently ranks as one of the most popular programming languages, and has gained widespread use in the machine learning community
~~~


#### RAID  


 - 여러 개의 디스크를 하나의 디스크처럼 사용
 - 운영체제에서 sw로 구현하는 형태도 있음
 - 2개 이상의 디스크가 묶여있어야 RAID라 부를 수 있다
 - Linear RAID, RAID0 RAID1
 - RAID5, RAID6
 - 
