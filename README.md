# Git-Practice

### 리눅스 기본 명령어 정리 및 예제

- pwd (print working directory)  :  현재 위치의 경로 를 말해준다.

```swift
jihokim@gimjihoui-MacBookPro ~ % pwd
/Users/jihokim
```

- ls :  현재 디렉토리의 파일들을 보여준다. (숨김파일 제외)

```swift
Applications	Documents	Library		Music		Public
Desktop		Downloads	Movies		Pictures
```

- ls -al  , ls -la 둘다 같음 : 현 디렉토리의 모든파일 (숨김파일 포험) 상세보기 형태로 보여준다.

```swift
total 184
drwxr-xr-x+ 30 jihokim  staff    960  3 21 22:48 .
drwxr-xr-x   5 root     admin    160  3 16  2021 ..
drwxr-xr-x   6 jihokim  staff    192 12 17 16:13 .AnySign4PC
-r--------   1 jihokim  staff      8  3 16  2021 .CFUserTextEncoding
drwxr-xr-x@  3 jihokim  staff     96 10 21 16:04 .CrossWeb
-rw-r--r--@  1 jihokim  staff  14340  3 19 12:16 .DS_Store
drwx------  21 jihokim  staff    672  3 21 16:48 .Trash
drwxr-xr-x   3 jihokim  staff     96  7 20  2021 .cocoapods
-rw-r--r--   1 jihokim  staff    144  3  5 21:48 .delfino.conf
drwxr-xr-x  11 jihokim  staff    352  3 19 11:53 .git
-rw-r--r--   1 jihokim  staff    215  3 19 14:29 .gitconfig
-rw-r--r--@  1 jihokim  staff      0  4  1  2021 .gitignore_global
-rw-------   1 jihokim  staff   4096  3 19 12:28 .gitmessage.swp
-rw-r--r--   1 jihokim  staff      1  3 19 13:39 .gitmessage.txt
-rw-------   1 jihokim  staff     28  3  4 17:04 .lesshst
-rw-r--r--   1 jihokim  staff    222 10 14 13:27 .npki_pkcs11.cnf
drwxr-xr-x   3 jihokim  staff     96 10 14 13:27 .softforum
-rw-------   1 jihokim  staff  12288  3 19 12:24 .swp
-rw-------   1 jihokim  staff  13652  3 21 10:47 .viminfo
-rw-------   1 jihokim  staff  19419  3 21 16:54 .zsh_history
drwx------  82 jihokim  staff   2624  3 21 22:48 .zsh_sessions
drwx------@  3 jihokim  staff     96  9 13  2021 Applications
drwx------@ 16 jihokim  staff    512  3 21 10:28 Desktop
drwx------+  4 jihokim  staff    128  9 29 11:41 Documents
drwx------+ 35 jihokim  staff   1120  3 19 17:23 Downloads
drwx------@ 73 jihokim  staff   2336 10 20 11:39 Library
drwx------   4 jihokim  staff    128  3 23  2021 Movies
drwx------+  7 jihokim  staff    224  4 12  2021 Music
drwx------+  5 jihokim  staff    160  3 24  2021 Pictures
drwxr-xr-x+  5 jihokim  staff    160  5 26  2021 Public
```

- ls -l (print working directory)  :  현 디렉토리의 모든파일 ( 숨김 파일 제외) 상세보기 형태로 보여준다.

```swift
drwx------@  3 jihokim  staff    96  9 13  2021 Applications
drwx------@ 16 jihokim  staff   512  3 21 10:28 Desktop
drwx------+  4 jihokim  staff   128  9 29 11:41 Documents
drwx------+ 35 jihokim  staff  1120  3 19 17:23 Downloads
drwx------@ 73 jihokim  staff  2336 10 20 11:39 Library
drwx------   4 jihokim  staff   128  3 23  2021 Movies
drwx------+  7 jihokim  staff   224  4 12  2021 Music
drwx------+  5 jihokim  staff   160  3 24  2021 Pictures
drwxr-xr-x+  5 jihokim  staff   160  5 26  2021 Public
```

- rm -r (삭제할 이름)   :  현재 디렉토리에서 하위 디렉토리를 삭제할때 이용한다.

```swift
jihokim@gimjihoui-MacBookPro ~ % ls
Applications	Documents	Library		Music		Public
Desktop		Downloads	Movies		Pictures	test
jihokim@gimjihoui-MacBookPro ~ % **rm -r test** 
jihokim@gimjihoui-MacBookPro ~ % ls
Applications	Documents	Library		Music		Public
Desktop		Downloads	Movies		Pictures
```

- mkdir (생성할 디렉토리 이름)  :  디렉토리 생성 하는법 make directory의 약자 인 듯.

```swift
jihokim@gimjihoui-MacBookPro ~ % mkdir test 
jihokim@gimjihoui-MacBookPro ~ % ls
Applications	Documents	Library		Music		Public
Desktop		Downloads	Movies		Pictures	test
```

- cd 이동할 경로나 폴더 이름 : change directory의 약자로 하위 디렉토리 이동시  사용

```swift
jihokim@gimjihoui-MacBookPro ~ % cd test
jihokim@gimjihoui-MacBookPro test % <---- 이동됨
```

- cd ..  : 상위 디렉토리로 이동

```swift
jihokim@gimjihoui-MacBookPro ~ % pwd
/Users/jihokim
```

- cd  ~  : 최상위 디렉토리 (홈) 으로 이동

```swift
jihokim@gimjihoui-MacBookPro Downloads % cd ~
jihokim@gimjihoui-MacBookPro ~ % ls
Applications	Documents	Library		Music		Public
Desktop		Downloads	Movies		Pictures
```

[https://blog.naver.com/ehdud4520/222604365308](https://blog.naver.com/ehdud4520/222604365308)

더 많은 cd 예제는 여기서 확인해보자~

- vim 생성할 파일 이름  : 파일 생성시 사용

```swift
jihokim@gimjihoui-MacBookPro test % vim test.txt
```

- cat 읽을 파일 이름 : 아래와 같이 파일의 내용을 보여준다.

```swift
jihokim@gimjihoui-MacBookPro test % cat test.txt
asdasdasd
```

- pwd (print working directory)  :  현재 위치의 경로 를 말해준다.

```swift
jihokim@gimjihoui-MacBookPro ~ % pwd
/Users/jihokim
```
