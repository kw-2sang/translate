[![Vim Logo](https://github.com/vim/vim/raw/master/runtime/vimlogo.gif)](https://www.vim.org)

[![Github Build status](https://github.com/vim/vim/workflows/GitHub%20CI/badge.svg)](https://github.com/vim/vim/actions?query=workflow%3A%22GitHub+CI%22) [![Travis Build Status](https://travis-ci.com/vim/vim.svg?branch=master)](https://travis-ci.com/github/vim/vim) [![Appveyor Build status](https://ci.appveyor.com/api/projects/status/o2qht2kjm02sgghk?svg=true)](https://ci.appveyor.com/project/chrisbra/vim) [![Cirrus Build Status](https://api.cirrus-ci.com/github/vim/vim.svg)](https://cirrus-ci.com/github/vim/vim) [![Coverage Status](https://codecov.io/gh/vim/vim/coverage.svg?branch=master)](https://codecov.io/gh/vim/vim?branch=master) [![Coverity Scan](https://scan.coverity.com/projects/241/badge.svg)](https://scan.coverity.com/projects/vim) [![Language Grade: C/C++](https://img.shields.io/lgtm/grade/cpp/g/vim/vim.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/vim/vim/context:cpp) [![Debian CI](https://badges.debian.net/badges/debian/testing/vim/version.svg)](https://buildd.debian.org/vim) [![Packages](https://repology.org/badge/tiny-repos/vim.svg)](https://repology.org/metapackage/vim) [![Fossies codespell report](https://fossies.org/linux/test/vim-master.tar.gz/codespell.svg)](https://fossies.org/linux/test/vim-master.tar.gz/codespell.html)

<sub>For translations of this README see the end.</sub>

여러분이 만약 버그를 찾으셨거나 새로운 기능을 추가할 기발한 방법을 의논하고 싶으시다면, [issue](https://github.com/vim/vim/issues)를 참고해주세요.
여러분이 만약 질문이 있거나 Vim을 위한 무언가 기발한 생각을 의논하고 싶으시다면, [StackExchange](https://vi.stackexchange.com/)를 사용하실 수 있습니다.
또는 [Maillists](https://www.vim.org/community.php)중 하나를 택하셔도 됩니다.


## Vim이란? ##

Vim은 이전 UNIX 텍스트 편집기 [Vi](https://en.wikipedia.org/wiki/Vi)의 크게 개선된 버전입니다. 새로운 기능들이 많이 추가되었습니다: multi-level undo, 구문 강조(syntax highlighting), 명령줄 히스토리, 온라인 도움말, 맞춤법 검사(spell checking), 파일 이름 자동 완성(filename completion), block operations, 스크립트 언어 등. 또한 그래픽 유저 인터페이스(GUI)를 사용할 수 있습니다. 여전히 Vi에 대한 호환성이 유지되어, Vi가 손에 익은 사람이 Vim을 사용할지라도 익숙할 것입니다.
Vi와 다른 점은 [`runtime/doc/vi_diff.txt`](runtime/doc/vi_diff.txt)에서 볼 수 있습니다.

Vim 편집기는 프로그램과 일반 텍스트 파일을 편집하는데 아주 유용합니다.
모든 명령이 일반 키보드 문자로 제공되기 때문에, 열 손가락으로 아주 빠른 작업을 수행할 수 있습니다.
또한 기능 키를 사용자가 원하는 명령으로 매핑할 수 있고, 마우스도 사용 가능합니다.

Vim은 MS Windows (XP, Vista, 7, 8, 10), macOS, Haiku, VMS, 거의 모든 UNIX 기반 운영체제에서 실행됩니다. 다른 시스템으로 이식(포팅)하는 것도 아주 어렵지 않을 겁니다.
Vim의 구 버전은 MS-DOS, MS-Windows 95/98/Me/NT/2000, Amiga DOS, Atari MiNT, BeOS, RISC OS and OS/2에서 실행됩니다. 하지만 더 이상 유지보수는 지원하지 않습니다.

Vim9 스크립트는 [README_VIM9](README_VIM9.md)에서 확인할 수 있습니다.

## 배포 ##

여러분은 자주 사용하는 패키지 관리자를 통해 Vim을 설치할 수 있습니다. Mac 및 Linux에는 Vim의 소형 버전이 이미 설치되어 있습니다만, 더 많은 기능을 원한다면 Vim을 따로 설치해야 합니다.

Unix, PC, Amiga, 기타 운영체제를 위한 별도의 배포판이 마련되어 있습니다.
원본 ['README.md'](https://github.com/vim/vim/blob/master/README.md) 파일은 런타임 아카이브와 함께 제공됩니다. 여기에는 문서와 구문 파일, 런타임을 사용하는 기타 파일이 포함됩니다.
Vim을 실행하기 위해서는 무조건 Binary 아카이브 또는 Source 아카이브 중 하나를 가져와야 합니다.
둘 중 무엇이 필요한지는 여러분의 실행 환경과 직접 컴파일 여부에 따라 나뉩니다.
현재 사용 가능한 배포판에 대한 개요는 [https://www.vim.org/download.php]에서 확인하세요.

Vim의 최신 버전을 받을 수 있는 대표적인 곳:
* [GitHub 저장소](https://github.com/vim/vim)
* [아카이브 형식의 소스 코드](https://github.com/vim/vim/releases)
* [Windows 설치 파일](https://github.com/vim/vim-win32-installer/releases)



## 컴파일 ##

