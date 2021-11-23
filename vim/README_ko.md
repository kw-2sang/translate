[![Vim Logo](https://github.com/vim/vim/raw/master/runtime/vimlogo.gif)](https://www.vim.org)

[![Github Build status](https://github.com/vim/vim/workflows/GitHub%20CI/badge.svg)](https://github.com/vim/vim/actions?query=workflow%3A%22GitHub+CI%22) [![Travis Build Status](https://travis-ci.com/vim/vim.svg?branch=master)](https://travis-ci.com/github/vim/vim) [![Appveyor Build status](https://ci.appveyor.com/api/projects/status/o2qht2kjm02sgghk?svg=true)](https://ci.appveyor.com/project/chrisbra/vim) [![Cirrus Build Status](https://api.cirrus-ci.com/github/vim/vim.svg)](https://cirrus-ci.com/github/vim/vim) [![Coverage Status](https://codecov.io/gh/vim/vim/coverage.svg?branch=master)](https://codecov.io/gh/vim/vim?branch=master) [![Coverity Scan](https://scan.coverity.com/projects/241/badge.svg)](https://scan.coverity.com/projects/vim) [![Language Grade: C/C++](https://img.shields.io/lgtm/grade/cpp/g/vim/vim.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/vim/vim/context:cpp) [![Debian CI](https://badges.debian.net/badges/debian/testing/vim/version.svg)](https://buildd.debian.org/vim) [![Packages](https://repology.org/badge/tiny-repos/vim.svg)](https://repology.org/metapackage/vim) [![Fossies codespell report](https://fossies.org/linux/test/vim-master.tar.gz/codespell.svg)](https://fossies.org/linux/test/vim-master.tar.gz/codespell.html)

<sub>For translations of this README see the end.</sub>

여러분이 만약 버그를 찾으셨거나 새로운 기능을 추가할 기발한 방법을 의논하고 싶으시다면, [issue](https://github.com/vim/vim/issues)를 참고해주세요.
여러분이 만약 질문이 있거나 Vim을 위한 무언가 기발한 생각을 의논하고 싶으시다면, [StackExchange](https://vi.stackexchange.com/)를 사용하실 수 있습니다.
또는 [Maillists](https://www.vim.org/community.php)중 하나를 택하셔도 됩니다.


## Vim이란? ##

Vim은 이전 UNIX 텍스트 편집기 [Vi](https://en.wikipedia.org/wiki/Vi)의 크게 개선된 버전입니다. 새로운 기능들이 많이 추가되었습니다: multi-level undo, 구문 강조(syntax highlighting), 명령줄 히스토리, 온라인 도움말, 맞춤법 검사(spell checking), 파일 이름 자동 완성(filename completion), block operations, 스크립트 언어 등. 또한 그래픽 유저 인터페이스(GUI)를 사용할 수 있습니다. 여전히 Vi에 대한 호환성이 유지되어, Vi가 손에 익은 사람이 Vim을 사용할지라도 익숙할 것입니다.
Vi와 다른 점은 [`runtime/doc/vi_diff.txt`](https://github.com/vim/vim/blob/master/runtime/doc/vi_diff.txt)에서 볼 수 있습니다.

Vim 편집기는 프로그램과 일반 텍스트 파일을 편집하는데 아주 유용합니다.
모든 명령이 일반 키보드 문자로 제공되기 때문에, 열 손가락으로 아주 빠른 작업을 수행할 수 있습니다.
또한 기능 키를 사용자가 원하는 명령으로 매핑할 수 있고, 마우스도 사용 가능합니다.

Vim은 MS Windows (XP, Vista, 7, 8, 10), macOS, Haiku, VMS, 거의 모든 UNIX 기반 운영체제에서 실행됩니다. 다른 시스템으로 이식(포팅)하는 것도 아주 어렵지 않을 겁니다.
Vim의 구 버전은 MS-DOS, MS-Windows 95/98/Me/NT/2000, Amiga DOS, Atari MiNT, BeOS, RISC OS and OS/2에서 실행됩니다. 하지만 더 이상 유지보수는 지원하지 않습니다.

Vim9 스크립트는 [README_VIM9](https://github.com/vim/vim/blob/master/README_VIM9.md)에서 확인할 수 있습니다.

## 배포 ##

여러분은 자주 사용하는 패키지 관리자를 통해 Vim을 설치할 수 있습니다. Mac 및 Linux에는 Vim의 소형 버전이 이미 설치되어 있습니다만, 더 많은 기능을 원한다면 Vim을 따로 설치해야 합니다.

Unix, PC, Amiga, 기타 운영체제를 위한 별도의 배포판이 마련되어 있습니다.
원본 [`README.md`](https://github.com/vim/vim/blob/master/README.md) 파일은 런타임 아카이브와 함께 제공됩니다. 여기에는 문서와 구문 파일, 런타임을 사용하는 기타 파일이 포함됩니다.
Vim을 실행하기 위해서는 무조건 Binary 아카이브 또는 소스 아카이브 중 하나를 가져와야 합니다.
둘 중 무엇이 필요한지는 여러분의 실행 환경과 직접 컴파일 여부에 따라 나뉩니다.
현재 사용 가능한 배포판에 대한 개요는 https://www.vim.org/download.php 에서 확인하세요.

Vim의 최신 버전을 받을 수 있는 대표적인 곳:
* [GitHub 저장소](https://github.com/vim/vim)
* [아카이브 형식의 소스 코드](https://github.com/vim/vim/releases)
* [Windows 설치 파일](https://github.com/vim/vim-win32-installer/releases)



## 컴파일 ##

여러분이 Binary 배포판을 얻은 경우에는 Vim을 따로 컴파일하실 필요는 없습니다. 하지만 소스 배포판을 얻은 경우, 컴파일을 위한 모든 파일은 ['src'](https://github.com/vim/vim/blob/master/src) 디렉터리에 있습니다.
자세한 내용은 ['src/INSTALL'](https://github.com/vim/vim/blob/master/src/INSTALL)을 확인하세요.


## 설치 ##

특정 시스템 별 자세한 사항은 아래 파일을 참조하세요.
[READMEdir 디렉터리](https://github.com/vim/vim/blob/master/READMEdir) (저장소 내부) 또는 최상위 디렉터리 (아카이브를 풀었을 경우):

    README_ami.txt		Amiga
	README_unix.txt		Unix
	README_dos.txt		MS-DOS and MS-Windows
	README_mac.txt		Macintosh
	README_haiku.txt	Haiku
	README_vms.txt		VMS

여러분이 사용하는 시스템에 따라 기타 `README_*.txt` 파일이 마련되어 있습니다.


## 문서 ##

Vim tutor는 초심자를 위한 1시간 짜리 교육 코스입니다.
`vimtutor`로 시작할 수 있곤 합니다. 자세한 정보는 `:help tutor`를 확인하세요.

가장 좋은 방법은 Vim 내에서 `:help`를 사용하는 것입니다. 아직 Vim을 설치하지 않았다면, [`runtime/doc/help.txt`](https://github.com/vim/vim/blob/master/runtime/doc/help.txt)를 확인하세요.
여기에는 다른 문서 파일에 대한 포인터가 포함되어 있습니다.
사용 설명서는 책처럼 읽히니, Vim을 배우는 용도로 추천드립니다. `:help user-manual`을 참고하세요.


## 복사(Copying) ##

Vim은 Charityware입니다. 여러분은 얼마든지 Vim을 사용하고, 복사할 수 있습니다. 하지만 우간다 고아들을 위한 기부를 여러분께 권하고 싶습니다.
[`runtime/doc/uganda.txt`](https://github.com/vim/vim/blob/master/runtime/doc/uganda.txt) 이 파일을 읽어주세요(자세한 사항은 Vim 내에서 `:help uganda`를 입력하여 확인하세요).

라이센스 핵심 정리: 수정되지 않은 Vim 복사본에 대한 사용과 배포에는 제한이 없습니다. Vim의 일부도 마찬가지로 배포될 수 있지만, 라이센스 내용은 항상 포함되어야 합니다. 수정된 버전은 몇 가지의 제한이 적용됩니다.
라이센스는 GPL 호환(compatible)이므로 여러분은 Vim을 GPL 라이브러리와 함께 컴파일할 수 있고, 배포할 수 있습니다.


## 협찬(Sponsoring) ##

버그 수정과 새로운 기능을 추가하는 것은 많은 시간과 노력이 소요됩니다. 이러한 노고에 대한 감사를 표하고, Bram과 다른 이들에게 일을 계속 할 수 있게 동기를 부여하기 위해 Vim에 기부를 바랍니다.

Bram이 유급 직장으로 돌아갔기 때문에 그 돈은 우간다의 어린이들을 돕는데에 사용될 것입니다.
[`runtime/doc/uganda.txt`](https://github.com/vim/vim/blob/master/runtime/doc/uganda.txt)를 확인해주세요.
하지만 동시에 기부는 Bram에게 Vim을 계속 작업하려는 동기를 부여합니다.

협찬에 대한 최신 정보는 Vim 웹사이트를 참조하세요:
	https://www.vim.org/sponsor/



## 기여(Contributing) ##

여러분이 Vim을 더 나은 방향으로 발전하도록 도와주시려면, [CONTRIBUTING_ko.md](./CONTRIBUTING_ko.md)를 확인해주세요.


## 정보 ##

Vim에 대한 최신 뉴스는 Vim 홈페이지에서 찾으실 수 있습니다:
	https://www.vim.org/

문제가 생겼다면, Vim 문서나 팁을 확인하세요:
	https://www.vim.org/docs.php
	https://vim.fandom.com/wiki/Vim_Tips_Wiki

문제가 해결되지 않거나 또 다른 질문이 있으시다면, Vim 사용자들과 개발자들이 토의하기 위해 아래 메일 주소 목록 중 하나를 통해 연락해주세요:
	https://www.vim.org/maillist.php

다른 방법이 없다면 버그를 직접 알려주세요:
	Bram Moolenaar <Bram@vim.org>


## 메인 작성자(Main author) ##

기타 의견이나 패치, 꽃과 의견은 이곳으로 보내주세요:
	Bram Moolenaar <Bram@vim.org>


This is KOREAN translation of [`README.md`](https://github.com/vim/vim/blob/master/README.md) for version 8.2 of Vim: Vi IMproved.
`README_ko.md` 파일은 `vim/vim` 프로젝트의 `README.md`를 한국어로 번역한 것입니다.