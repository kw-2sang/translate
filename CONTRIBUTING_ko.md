# Vim에 기여하기

어떤 형식이든 패치를 환영합니다.
패치에 대한 토의는 'vim-dev' 메일 주소에서 이루어집니다.
여러분이 GitHub에 Pull request를 만든다면, 'vim-dev' 메일 주소로 연동되어 전송됩니다. 또한 여러분은 패치를 직접적으로 전송하실 수 있습니다.
이러한 경우에, 첨부파일은 Unified diff 형식으로 보내주시면 감사하겠습니다.
메일 주소에 대한 정보는 [Vim 웹사이트]를 참고하세요.

[Vim 웹사이트]: http://www.vim.org/maillist.php#vim-dev

Pull request는 지속적 통합(CI)의 테스트의 계기가 되고, 여러분에게 문제를 인식하게 하는 이점이 있습니다. (Coverage 경고를 무시할 수 있습니다, 너무 시끄럽기만 하죠.)

한 번쯤 테스트 해주시기를 부탁드립니다.
새로운 기능과 버그 수정은 프로젝트의 퇴보를 막기 위해 테스트를 해야 합니다: 테스트는 수정이 있기 전에는 실패하고 수정 후에는 통과해야 합니다.
예시를 확인하려면 최근 패치를 살펴보시거나 ":help testing"을 이용하여 도움말을 찾아보세요.
테스트는 "src/testdir" 경로에 위치하고 있습니다.

기여는 Vim 라이센스에 따라 Vim과 함께 배포됩니다.
변경 사항을 제공하는 것은 여러분이 이를 동의하고, 여러분의 기여는 상표 또는 특허에 문제를 일으키지 않는다는 것을 내포합니다.
서명할 기여자 라이센스 동의(CLA)는 없습니다.


# 문제 보고하기

우리는 GitHub issues를 사용하지만, 이것이 필수는 아닙니다.
Vim 메일 주소로 보내주셔도 좋습니다.

실제로 발생한 문제점에 대해서는 GitHub issue만을 사용해주시길 바랍니다.
여러분이 제기할 문제점이 Vim의 문제인지 100% 확신할 수 없을 때에는 제일 먼저 Vim user 메일 주소를 통해 의논해주세요.
여러분의 플러그인이나 설정을 제외한 문제점을 줄이기 위해 해당 명령어를 실행해주세요:

    vim --clean

여러분이 issue를 보고하신다면, 그것을 재현하기 위한 방법을 자세하게 묘사해주시면 감사하겠습니다.
예를 들자면, "insert some text"라고 하지 마시고, 여러분이 행한 정확한 내용을 말씀해주세요: "ahere is some text&lt;Esc&gt;".
여러분이 순서대로 행하신 단계는 문제점이 고쳐졌는가에 대한 검증 테스트가 쓰이는데 사용될 수 있습니다.

아무리 작은 문제점이든, 문서의 오탈자든 마음 놓고 보고해주세요.

이미 알려준 문제점에 대해서 알고싶으시다면 todo 파일을 참고하세요: ":help todo".
또는 최신 버전을 보고 싶으시다면 GitHub에서 [todo 파일]을 열어서 확인하세요.

[todo 파일]: https://github.com/vim/vim/blob/master/runtime/doc/todo.txt


# 구문(Syntax), 들여쓰기 및 기타 런타임 파일

해당하는 최신 버전 파일은 저장소(Repository)에서 얻을 수 있습니다.
일반적으로 번호가 매겨진 패치로 업데이트되지 않거든요.

여러분이 해당 파일들 중에 문제점을 발견하셨거나, 발전을 위한 더 좋은 의견이 있으시다면 제일 먼저 유지보수 담당자에게 직접 연락해주시길 부탁드립니다.
유지보수 담당자의 이름과 이메일 주소는 해당 파일의 헤더를 참조하시면 됩니다.

유지보수 담당자가 해당 문제점을 해결하여 Vim과 함께 배포될 수 있도록 Bram에게 업데이트를 보낼 것입니다.

유지보수 담당자가 응답하지 않는다면, 'vim-dev' 메일 주소로 연락해주세요.


# 번역

한국어 번역에 수고하신 분은 다음과 같습니다.
*   cjw1359: [CONTRIBUTING_ko.md](https://github.com/cjw1359/opensource/blob/master/Vim/CONTRIBUTING_ko.md)
*   kw-2sang: 본 번역은 원본 서식에 맞추고, URL 바로가기 등을 추가하여 새로 번역한 것입니다.

CONTRIBUTING 파일의 원본은 다음에서 확인할 수 있습니다.
[English](https://github.com/vim/vim/blob/master/CONTRIBUTING.md)

메시지와 런타임 파일의 번역을 매우 환영합니다!
번역될 수 있는 파일:
*   Vim 내 메시지는 여기서 확인하세요. [src/po/README.txt][1]
    또한 바탕화면 아이콘에 사용된답니다.
*   메뉴는 여기서 확인하세요. [runtime/lang/README.txt][2]
*   Vim tutor는 여기서 확인하세요. [runtime/tutor/README.txt][3]
*   메뉴얼 페이지의 예시는 여기서 확인하세요. [runtime/doc/\*.1][4]
*   설치 프로그램의 예시는 여기서 확인하세요. [nsis/lang/\*.nsi][5]

도움말 파일은 별도로 번역하여 사용할 수 있습니다.
예시는 https://www.vim.org/translations.php 여기서 확인하세요.

[1]: https://github.com/vim/vim/blob/master/src/po/README.txt
[2]: https://github.com/vim/vim/blob/master/runtime/lang/README.txt
[3]: https://github.com/vim/vim/blob/master/runtime/tutor/README.txt
[4]: https://github.com/vim/vim/blob/master/runtime/doc/vim.1
[5]: https://github.com/vim/vim/blob/master/nsis/lang/english.nsi