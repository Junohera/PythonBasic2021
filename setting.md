# Jupyter Notebook Elegant Setting(간단하지만 우아한 설정)

# 1. JT (jupyter-themes)
---
#### ex)
```
pip install jupyterthemes
jt -l # 테마 목록 조회
# jt -t ${원하는 테마와 온갖 옵션들}

# 현재 세팅중인 값
jt -t chesterish -f roboto -fs 9 -altp -tfs 11 -nfs 10 -cellw 96% -cursw 8 -T -N
```
#### reset to default
```
jt -r
```
### 더많은 옵션 목록

#### Description of Command Line options
| cl options            |   arg   |  default   |
| :-------------------- | :-----: | :--------: |
| Usage help            |   -h    |     --     |
| List Themes           |   -l    |     --     |
| Theme Name to Install |   -t    |     --     |
| Code Font             |   -f    |     --     |
| Code Font-Size        |   -fs   |     11     |
| Notebook Font         |   -nf   |     --     |
| Notebook Font Size    |  -nfs   |     13     |
| Text/MD Cell Font     |   -tf   |     --     |
| Text/MD Cell Fontsize |  -tfs   |     13     |
| Pandas DF Fontsize    |  -dfs   |     9      |
| Output Area Fontsize  |  -ofs   |    8.5     |
| Mathjax Fontsize (%)  | -mathfs |    100     |
| Intro Page Margins    |   -m    |    auto    |
| Cell Width            | -cellw  |    980     |
| Line Height           | -lineh  |    170     |
| Cursor Width          | -cursw  |     2      |
| Cursor Color          | -cursc  |     --     |
| Alt Prompt Layout     |  -altp  |     --     |
| Alt Markdown BG Color | -altmd  |     --     |
| Alt Output BG Color   | -altout |     --     |
| Style Vim NBExt*      |  -vim   |     --     |
| Toolbar Visible       |   -T    |     --     |
| Name & Logo Visible   |   -N    |     --     |
| Kernel Logo Visible   |   -kl   |     --     |
| Reset Default Theme   |   -r    |     --     |
| Force Default Fonts   | -dfonts |     --     |

> 공식문서 참조 : https://github.com/dunovank/jupyter-themes

# 2. Nbextensions
---
### add
1. Code prettify : 코드 자동 정렬
1. Codefolding : 코드접기
1. executeTime :  실행시간
1. Hide input : 선택셀 코드숨김
1. Hide input all : 전역셀 코드숨김
1. Highlight selected word : 타이핑중인 단어나 포커싱된 단어와 동일한 단어들을 하이라이트처리
1. highlighter :  기존의 마크다운을 더 강조하기 위함
1. Scratchpad : 현재의 노트북에는 포함하지않을 코딩을 하기위한 임시 편집창 제공
1. Table of Contents (2) : 마크다운 기준 목차역할 수행(실행중위치 확인도 가능)
1. Variable Inspector : 현재의 노트북의 변수들 정보 조회 type, shape, size, length 등등
1. hinterland : Tab키를 누르지않아도 항상 눌러주는것처럼
1. Runtools : Cell을 누르고 실행을 선택해야하는데 아예 외부로 빼주고, 사실 Alt + X를 누르면 위에서부터 전부실행되는 것때문에 사용