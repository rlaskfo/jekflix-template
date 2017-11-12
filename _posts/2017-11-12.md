---
layout: post
title: "Python Lib 설치"
date: 2017-11-12

---

이번 포스팅 내용은 <a href=""> Python Library 설치 </a> 입니다.
현재 제가 개발하고 있는 환경은 Anaconda의 Python 3.5 입니다. 
-Anaconda 를 설치하거나 Python을 설치하는 과정은 생략합니다.

본인이 설치한 python의 version을 모른다면 CMD창을 키고 ** python --version **명령어를 치면 확인할 수 있습니다.

![Alt text](https://rlaskfo.github.io/images/python_version.PNG)

## pip install "Lib이름"

Python 에서 개발하다보면 이것저것 필요한 Library들이 많습니다. 
그래서 그런건지 모르겠지만 Python에서는 간단한 명령어로 Library를 설치할 수 있습니다.

일단 본인의 환경에서 설치가 되려면 pip가 설치되어야 합니다. 
CMD창을 키고 **pip install pip** 를 입력해봅니다. 
![Alt text](https://rlaskfo.github.io/images/pip_install_first.PNG)
저같은 경우엔 설치가 되어있어서 그림 같이 나오지만 설치가 처음인 경우라면 뭔가 설치되는 화면이 진행될 것입니다. 

이제 그 다음 과정은 Library설치 입니다. 
역시 CMD창에서 **pip install Library이름** 를 입력해봅니다.
저 같은 경우엔 지금 ==**konlpy**== 라는 library를 설치를 하는 것입니다. 
   ![Alt text](https://rlaskfo.github.io/images/pip_install.PNG)
설치가 성공적이라면 successfully installed이라는 명령어가 나오겠죠?

Python은 계속해서 Library가 update가 됩니다. 그래서 해당 Library를 업데이트 하고 싶을 때도 pip명령어를 사용하면 됩니다. 
CMD창에서 **pip install --upgrade Library이름** 를 입력해봅니다.
![Alt text](https://rlaskfo.github.io/images/pip_upgrade_install.PNG)

## 직접 Download 하는 방법
대부분이 pip 명령어로 설치가 성공적으로 되지만 
가끔 설치가 제대로 되지 않는다며 CMD창이 빨강색으로 뒤덮일 때가 있습니다. 
이런 경운에 저는 직접 Library파일을 다운받아서 설치를 하는데요, 
그 과정을 정리해보겠습니다. 

1. Library파일 다운 받기 
   
   먼저 아래 링크로 걸어둔 사이트에서 Library파일을 다운 받습니다.
   
   [Python library Download](https://www.lfd.uci.edu/~gohlke/pythonlibs/)
   
   다운받을때는 당연히 자신이 설치한 python version과 일치하는걸 다운받아야합니다.
   예를 들어 numpy library를 다운받는다 하면,
   ![Alt text](https://rlaskfo.github.io/images/lib_site.PNG)
   그림처럼 numpy 아래 여러 파일들이 있는데 각 파일마다 **"cp숫자"**가 있는걸 확인할 수 있습니다. 이 숫자는 python version을 말하고 있는겁니다.
   저의 경우엔 python이 3.5버전이었으니깐 cp35에 해당하는 파일을 다운 받으면 됩니다. 
   win32는 os환경이 32bit, 64는 64bit를 의미하는거니깐 그거에 맞춰서 다운받아주세요!
  
2. CMD창에서 Download 
   
   이제 CMD창에서 방금 다운 받은 파일이 있는 경로로 이동합니다. 
   **cd명령어 + 파일 경로** 입력하면 이동이 됩니다.
   ```js
   cd C:\\Users\\Downloads
	```
   그럼 이제 해야될 일은 pip install "다운 받은 파일 이름"을 입력합니다.
   ```js
   pip install "numpy‑1.13.3+mkl‑cp35‑cp35m‑win_amd64.whl"
	```
그럼 위의 pip install numpy를 입력해 설치하는 것처럼 설치가 진행됩니다.


## 결론

요즘 python library들을 upgrade하면서 이전 버전과 호환이 안되거나, 더이상 지원하지 않는 함수들이 생겨나는 경우들을 맞닥뜨리는 중입니다..
각자가 조심해서..? upgrade해야 될 것 같습니다. 제가 알기론 업데이트 한 버전에 대한 설명 문서들이 있어 그걸 미리 읽어보고 upgrade 여부를 판단해 설치하면 좋을 것 같습니다.






