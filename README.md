## 0427 Defining routes.
<p>route가 render 되려면 page.tsx가 있어야하고 그것은 render될 url에 해당하는 폴더 안에 있어야한다..

## 0428 gitignore.
<p>git 작업도중 push 가 안되는 이유가 용량이 100mb넘어서 였는데 gitignore로 불필요 파일을 제외하고도 계속해서 안됐다. 캐시 초기화 등등 모든걸 해봐도 안됐으나 rm -rf ./.git 로 로컬 저장소 디렉토리 삭제후 다시 했더니 잘 돌아갔다. 오늘의 교훈 git 에대한 이해도를 높이고 git 디렉토리 관리 잘하자!

## 0616 Loading State using Suspense from React.
<p>Page 단위 로딩 => loading.tsx
<p>서버 컴포넌트 단위 로딩 => Suspense

## 0623 Recap
<p>fetching data => server component : async / await
<p>loading => loading component
<p>multi fetching => Promise.all / but!! => Suspense 가 더 좋음! re/promise.all 은 모든 data fetching 다될때까지 loading 화면으로 나오지만 suspense 는 로딩상태를 분리해준다. 그럼 page 자체를 기다리지 않고 component 단위로 await 할 수 있기때문에 훨씬 효율적이다.

## 0623 Css
<p>css styling 연습 및 파일구조 경험 => 대부분 비슷한데 module 쓰는법이 조금 다른것 같다. 그래도 익숙해 지면 금방 잘 될듯? 연습 많이하자.

## 0630
<p>generateMetadata
메타데이터 객체(metadata) 및 generateMetadata 함수는 서버 컴포넌트에서만 지원됩니다.
동일한 경로에서 메타데이터 객체와 generateMetadata 함수를 모두 export 할 수는 없습니다. (둘 중 하나만 사용 가능)
<p>https://nextjs.org/docs/app/api-reference/functions/generate-metadata#generatemetadata-function

## 0630
<p>deployment and prefetch => prefetch / rendering 되는 요소의 자식 data 들을 미리 fetch 해서 자식 페이지에 들어갔을때 이미 data가 fetch 돼있게 해준다!