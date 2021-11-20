[![Vim Logo](https://github.com/vim/vim/raw/master/runtime/vimlogo.gif)](https://www.vim.org)

[![Github Build status](https://github.com/vim/vim/workflows/GitHub%20CI/badge.svg)](https://github.com/vim/vim/actions?query=workflow%3A%22GitHub+CI%22) [![Travis Build Status](https://travis-ci.com/vim/vim.svg?branch=master)](https://travis-ci.com/github/vim/vim) [![Appveyor Build status](https://ci.appveyor.com/api/projects/status/o2qht2kjm02sgghk?svg=true)](https://ci.appveyor.com/project/chrisbra/vim) [![Cirrus Build Status](https://api.cirrus-ci.com/github/vim/vim.svg)](https://cirrus-ci.com/github/vim/vim) [![Coverage Status](https://codecov.io/gh/vim/vim/coverage.svg?branch=master)](https://codecov.io/gh/vim/vim?branch=master) [![Coverity Scan](https://scan.coverity.com/projects/241/badge.svg)](https://scan.coverity.com/projects/vim) [![Language Grade: C/C++](https://img.shields.io/lgtm/grade/cpp/g/vim/vim.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/vim/vim/context:cpp) [![Debian CI](https://badges.debian.net/badges/debian/testing/vim/version.svg)](https://buildd.debian.org/vim) [![Packages](https://repology.org/badge/tiny-repos/vim.svg)](https://repology.org/metapackage/vim) [![Fossies codespell report](https://fossies.org/linux/test/vim-master.tar.gz/codespell.svg)](https://fossies.org/linux/test/vim-master.tar.gz/codespell.html)

<sub>For translations of this README see the end.</sub>

여러분이 만약 버그를 찾으셨거나 새로운 기능을 추가할 기발한 방법을 의논하고 싶으시다면, [issue](https://github.com/vim/vim/issues)를 참고해주세요.
여러분이 만약 질문이 있거나 Vim을 위한 무언가 기발한 생각을 의논하고 싶으시다면, [StackExchange](https://vi.stackexchange.com/)를 사용하실 수 있습니다.
또는 [Maillists](https://www.vim.org/community.php)중 하나를 택하셔도 됩니다.


## Vim이란? ##

Vim은 이전 UNIX 텍스트 편집기 [Vi](https://en.wikipedia.org/wiki/Vi)의 크게 개선된 버전입니다. 새로운 기능들이 많이 추가되었습니다: multi-level undo, 구문 강조(syntax highlighting), 명령줄 히스토리, 온라인 도움말, 맞춤법 검사(spell checking), 파일 이름 자동 완성(filename completion), block operations, 스크립트 언어 등. 또한 그래픽 유저 인터페이스(GUI)를 사용할 수 있습니다. 여전히 Vi에 대한 호환성이 유지되어, Vi가 손에 익은 사람이 Vim을 사용할지라도 익숙할 것입니다.
Vi와 다른 점은 [`runtime/doc/vi_diff.txt`](runtime/doc/vi_diff.txt)에서 볼 수 있습니다.