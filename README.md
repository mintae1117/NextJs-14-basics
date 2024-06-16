## 0427 Defining routes.
<p>route가 render 되려면 page.tsx가 있어야하고 그것은 render될 url에 해당하는 폴더 안에 있어야한다..

## 0428 gitignore
<p>git 작업도중 push 가 안되는 이유가 용량이 100mb넘어서 였는데 gitignore로 불필요 파일을 제외하고도 계속해서 안됐다. 캐시 초기화 등등 모든걸 해봐도 안됐으나 rm -rf ./.git 로 로컬 저장소 디렉토리 삭제후 다시 했더니 잘 돌아갔다. 오늘의 교훈 git 에대한 이해도를 높이고 git 디렉토리 관리 잘하자!

## 0616 Suspense Loading.tsx
<p>Page 단위 로딩 => loading.tsx
<p>서버 컴포넌트 단위 로딩 => Suspense