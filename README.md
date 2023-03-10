## ๐ป PJH's Blog ๐ก

<strong>์ต๊ทผ ๋ค์ด ๊ด์ฌ ๊ฐ๊ณ , ์ง์  ํ๋ก์ ํธ๋ฅผ ์งํํ๋ฉฐ ๊ตฌํํด๋ณด๊ณ  ์ถ์๋ ๊ธฐ์ ๋ค์ ํ์ตํ๋ ๋ชฉ์ ์ผ๋ก ์ ์ํ ๊ฐ๋จํ CRUD ๊ธฐ๋ฅ์ ์ ๊ณตํ๋ ํ ์ด ํ๋ก์ ํธ์๋๋ค. </strong>

- GraphQL
- React Qeury
- Next.js
- Apollo server
- twin.macro

<br>

## ๐ ํ๋ก์ ํธ ๊ธฐ๊ฐ

2023.01.13 ~ 2023.01.28

<br>

## ๐ Link

**Notion**
๐ [Notion Portfolio](https://www.notion.so/API-Practice-33a84c2d694947f68872ba74341911b5)

<br>

## ๐ ๋์ ๊ฐ๋ฐ์ผ์ง

โ๏ธ ํ๋ก์ ํธ๋ฅผ ๊ฐ๋ฐํ๋ฉฐ ์์ฑํ ๊ฐ๋ฐ๋ธ๋ก๊ทธ์๋๋ค.

- [REST API vs GraphQL](https://velog.io/@pjh1011409/REST-API-vs-GraphQL)
- [REST API ํต์ ](https://velog.io/@pjh1011409/REST-API-%ED%86%B5%EC%8B%A0)
- [GraphQL ํต์ ](https://velog.io/@pjh1011409/GraphQL-%ED%86%B5%EC%8B%A0)
- [RestAPI + ๋ฌดํ์คํฌ๋กค](https://velog.io/@pjh1011409/RestAPI-%EB%AC%B4%ED%95%9C%EC%8A%A4%ED%81%AC%EB%A1%A4)
- [GraphQL + ๋ฌดํ์คํฌ๋กค](https://velog.io/@pjh1011409/GraphQL-%EB%AC%B4%ED%95%9C%EC%8A%A4%ED%81%AC%EB%A1%A4)
- [GraphQL - Resolver / Schema](https://velog.io/@pjh1011409/GraphQL-Resolver)
- [Emotion + Tailwind CSS](https://velog.io/@pjh1011409/Emotion-Tailwind-CSS)
- [React Query - Hydration(SSR)](https://velog.io/@pjh1011409/React-Query-HydrationSSR)
- [React Query - ์ฌ์ฉ์ ๊ฒฝํ ๊ฐ์  UI](https://velog.io/@pjh1011409/React-Query-Global-Setting)


 
  
<br>

## โ๏ธ ์ฃผ์ ๊ณต๋ถ ๋ฐ ๊ตฌํ ์ฌํญ

- **API**
  - GraphQL, REST ๊ฐ๊ฐ ๋ค๋ฅธ API ์์ฒญ ๋ฐฉ๋ฒ๊ณผ ๊ทธ์ ๋ํ ์๋ต ๋ฐฉ๋ฒ์ ๋ํด ํ์ต

<br>

- **twin.macro** ๐จ

  - ๋น ๋ฅด๊ณ  ์ฝ๊ณ  ์ผ๊ด๋๊ฒ ๋์์ธํ  ์ ์๋ Utility CSS, Tailwind CSS์ JS ํ์ผ ๋ด์์ ํ๊ทธ ์์ ์คํ์ผ์ ์ ์ฉํ๋ CSS-in-JS, Emotion์ ํจ๊ป ์ฌ์ฉํ์ฌ flexibleํ ์ฝ๋ ์์ฑ ๊ฐ๋ฅ

<br>

- **Error, Loading**
  - React Query์ ์์ฑ๋ค์ ์ฌ์ฉํ์ฌ ์ฝ๊ณ  ํจ์จ์ ์ด๊ณ  ๊น๋ํ UI ์ ๊ณต
  - useIsFetching, useMutating, onSuccess, onError ...

<br>

- **Infinite Scroll**

  - ํจ์จ์ ์ธ ๋ฐ์ดํฐ ํจ์นญ ๊ตฌํ.
    - ๋ฐฉ๋ฒ 1. useInfiniteScroll + Intersection Observer API
    - ๋ฐฉ๋ฒ 2. useInfiniteScroll + React Infinite Scroller

  <br>

- **hydration**
  - React Query๋ฅผ ํตํ SSR๋ฐฉ์(Next.js) ๊ตฌํ์ ์ํ Hydration ๋ฐฉ๋ฒ ์ฌ์ฉ

<br>

## ๐ป Service Architecture

<img width="1022" alt="แแณแแณแแตแซแแฃแบ 2023-01-28 แแฉแแฎ 7 20 41" src="https://user-images.githubusercontent.com/81337674/215261387-07b2377d-eaad-48a9-9ee6-55c91ed0f95b.png">

<br>

## ๐ Project Architecture

#### Client

```
โญ๏ธ client
|
โโโ ๐ components
โ    โโโ ๐ MsgInput.tsx
โ    โโโ ๐ MsgItem.tsx
โ    โโโ ๐ MsgList.tsx
โ    โโโ ๐ common
โ           โโโ ๐ Button.tsx
โ           โโโ ๐ Input.tsx
โ           โโโ ๐ Card.tsx
โ
โโโ ๐ graphql
โ    โโโ ๐ messages.ts
โ    โโโ ๐ user.ts
โ
โโโ ๐ hooks
โ     โโโ ๐ userGetMessage.ts
โ     โโโ ๐ useCreateMessage.ts
โ     โโโ ๐ useUpdateMessage.ts
โ     โโโ ๐ useDeleteMessage.ts
โ     โโโ ๐ useInfiniteScroll.ts
โ     โโโ ๐ useQueryError.ts
โ     โโโ ๐ useCustomToast.ts
โ
โโโ ๐ pages
     โโโ ๐ _app.js
     โโโ ๐ index.tsx

```

#### Server

```
โญ๏ธ src
|
โโโ ๐ index.ts
โโโ ๐ firebase.js
โโโ ๐ types.ts
|
โโโ ๐ resolvers
โ    โโโ ๐ message.ts
โ    โโโ ๐ index.ts
โ    โโโ ๐ user.ts
โ
โโโ ๐ schema
     โโโ ๐ message.ts
     โโโ ๐ index.ts
     โโโ ๐ user.ts

```

<br>

## Query & Mutation

<img width="569" alt="แแณแแณแแตแซแแฃแบ 2023-01-28 แแฉแแฎ 7 42 37" src="https://user-images.githubusercontent.com/81337674/215262297-f6d837f4-9a05-49cc-8dac-f7cd47534b63.png">

<br>

## ๐  Tools

<p>
  <img src="https://img.shields.io/badge/Next.js-000000?style=for-the-badge&logo=Next.js&logoColor=white">
  <img src="https://img.shields.io/badge/Typescript-3178C6?style=for-the-badge&logo=Typescript&logoColor=white"> 
  <img src="https://img.shields.io/badge/GraphQL-E10098?style=for-the-badge&logo=GraphQL&logoColor=white">
 
<br>
  <img src="https://img.shields.io/badge/React Query-FF4154?style=for-the-badge&logo=React Query&logoColor=white">
     <img src="https://img.shields.io/badge/Apollo GraphQL-311C87?style=for-the-badge&logo=Apollo GraphQL&logoColor=white">
      <img src="https://img.shields.io/badge/Firebase-FFCA28?style=for-the-badge&logo=Firebase&logoColor=white">

  <br>
     <img src="https://img.shields.io/badge/Chakra UI-319795?style=for-the-badge&&logo=Chakra UI&logoColor=orange">
         <img src="https://img.shields.io/badge/Tailwind CSS-06B6D4?style=for-the-badge&logo=Tailwind CSS&logoColor=white">
             <img src="https://img.shields.io/badge/Emotion-F16521?style=for-the-badge&logo=Etsy&logoColor=white">
     <br>
  <img src="https://img.shields.io/badge/Visual%20Studio%20Code-0078d7.svg?style=for-the-badge&logo=visual-studio-code&logoColor=white">
  <img src="https://img.shields.io/badge/git-%23F05033.svg?style=for-the-badge&logo=git&logoColor=white">
  <img src="https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white">

<br>

## ๐ ์ฌ์ฉ ์ด์ 

### Next.js + React Query

- Redux์ ๋นํด ๊ตฌ์กฐ์ ์ผ๋ก ๊ฐ๊ฒฐ์ฑ์ ๊ฐ์ง๋ฉฐ, ๋ฐ์ดํฐ ํจ์นญ, ์บ์ฑ, ์๋ฒ ์ชฝ ๋ฐ์ดํฐ๋ฅผ ๊ด๋ฆฌํ๊ธฐ ์ฉ์ดํ๋ค.
- React.js๋ฅผ ์๋ฒ์ธก์์ pre-renderingํ์ฌ html์ ์์ฑํ๊ณ , ๋ธ๋ผ์ฐ์ ์๊ฒ ๋ณด๋ด์ฃผ๋ SSR๋ฐฉ์์ ๊ฐ๋ฐ์ ์งํํด๋ณด๊ณ  ์ถ์๋ค. </li>

### GraphQL + Apollo Server

- ํ๋์ EndPoint์ ์ฌ๋ฌ API ์์ฒญ์ด ๊ฐ๋ฅํ๋ฉฐ, ํ์ํ ์ ๋ณด๋ง ์์ฒญํ  ์ ์์ด HTTP ์์ฒญ ํ์์ ์๋ต ์ฌ์ด์ฆ๊ฐ ์ค์ด๋ ๋ค.
- GraphQL์ด ์ ์ฉ๋ ์๋ฒ๋ฅผ ์ฝ๊ฒ ์์ฑํ๊ฒ ๋์์ฃผ๋ ๋ผ์ด๋ธ๋ฌ๋ฆฌ๋ก, ๊ฐ๋จํ ์ฝ๋ ๋ช์ค๋ก GraphQL ์๋ฒ ๊ตฌ์ฑ์ด ๊ฐ๋ฅํ๋ค.

### Tailwind CSS + Emotion = Twin.macro

- Utiliy FirstCSS ์ CSS in JS์ ์ฅ์ ์ ๋ชจ๋ ์ด๋ ค ๋์ฑ ์ ์ฐํ CSS ๊ตฌํ ๊ฐ๋ฅ.

<br>

## ๐ฅ GIF

|                                                                                    **InfiniteScroll**                                                                                     |                                                                                        **Create**                                                                                         |
| :---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: | :---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: |
| <img width="300" height="400" alt="แแณแแณแแตแซแแฃแบ 2023-01-28 แแฉแแฎ 7 42 37" src="https://user-images.githubusercontent.com/81337674/215267483-88532d2b-1696-44a5-905b-4ee3212fd933.gif"> | <img width="300" height="400" alt="แแณแแณแแตแซแแฃแบ 2023-01-28 แแฉแแฎ 7 42 37" src="https://user-images.githubusercontent.com/81337674/215267628-d377ea72-bf3c-4b03-a1a8-d13b3303a3d8.gif"> |
|                                                                                        **Update**                                                                                         |                                                                                        **Delete**                                                                                         |
| <img width="300" height="400" alt="แแณแแณแแตแซแแฃแบ 2023-01-28 แแฉแแฎ 7 42 37" src="https://user-images.githubusercontent.com/81337674/215267659-c233243c-0b3a-4aaa-9ec3-7386f3972e58.gif"> | <img width="300" height="400" alt="แแณแแณแแตแซแแฃแบ 2023-01-28 แแฉแแฎ 7 42 37" src="https://user-images.githubusercontent.com/81337674/215267527-a5a65d7a-fe73-4934-9285-036ea70c5835.gif"> |
