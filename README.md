# Node.js and MongoDB :thumbsup:

### 1. **Infomation :eyes:**

- Server: Node.js (expess)
- Database: MongoDB (mongoose)
- OpenAPI - [건강보험심사평가원\_병원정보서비스](https://www.data.go.kr/tcs/dss/selectApiDataDetailView.do?publicDataPk=15001698)

### 2. **:star2: Node.js environment**

:heavy_check_mark: To start the node server :heart_eyes:

```
npm run devStart
```

:heavy_check_mark: Needed moudules are...

```
npm install express
npm install --save-dev nodemon
npm install request
npm install request-promise-native
npm install ejs
npm install mongoose
npm install method-override
npm install http
```

- request-promise-natiave: enables to use asycn, await request
- mongoose: MongoDB itself. You have to install MongoDB Server in order to use mongoose.
- method-override: enables to use DELETE, PUT, PATCH as well as GET, POST

:no_entry_sign: slugify, marked, dompurify, and jsdom are just for the TEST

### 3. **:file_folder: Directory Structure**

:heavy_check_mark: Follow MVC (model, view, controll) model.

:no_entry_sign: Directories or files related to 'mypage' are just for the TEST

> ##### node_modules (directory)
>
> ##### models (directory)
>
> > hospitals.js
>
> ##### routes (directory)
>
> > admin.js
>
> ##### views (directory)
>
> > index.ejs
>
> > ###### admin (directory)
> >
> > > hospital.ejs
> > > hospitals.ejs
> > > index.ejs
>
> package-lock.json
> package.json
> README.md
> server.js

### 4. Functions :dart:

- [x] Mongoose install & test it
- [x] Search hospitals by name
- [x] Create **[Open API Reload]** btn in admin page
- [ ] Admin Account (DB)
- [ ] Sign in & Sign up (DB) - 로그인 세션 & 아이디 중복 문제 처리, 비밀번호 암호화(솔트) 해야 함
- [ ] Create a normal users' mypage
- [ ] ~~Calculate hospitals' points to recommend hospitals tailored to the symptoms~~
- [ ] connect to Kakao map API
- [ ] get a user's addr & search it in DB