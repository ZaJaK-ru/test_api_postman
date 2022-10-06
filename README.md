# Test API

## Registration

запрос POST https://blog.kata.academy/api/users

```
{
  "user": {
    "username": "ZaJaK",
    "email": "zajak@mail.ru",
    "password": "12345"
  }
}
```

ответ

```
{
    "user": {
        "username": "zajak",
        "email": "zajak@mail.ru",
        "token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpZCI6IjYzM2ViMTU0M2NmNzA1MWIwMDgyYWFmOCIsInVzZXJuYW1lIjoiemFqYWsiLCJleHAiOjE2NzAyMzcwMTIsImlhdCI6MTY2NTA1MzAxMn0.ACyo_ASXgYVzePYcTuMmctgfvbFDmQRWF4zXDCD4rUc"
    }
}
```

## Authentication

запрос POST https://blog.kata.academy/api/users/login

```
{
  "user": {
    "email": "zajak@mail.ru",
    "password": "12345"
  }
}
```
ответ

```
{
    "user": {
        "username": "zajak",
        "email": "zajak@mail.ru",
        "token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpZCI6IjYzM2ViMTU0M2NmNzA1MWIwMDgyYWFmOCIsInVzZXJuYW1lIjoiemFqYWsiLCJleHAiOjE2NzAyMzcxNjAsImlhdCI6MTY2NTA1MzE2MH0.7oocm65aKRzW0iaEqJveNTT71_sVUOTpMGgmSS7n5Ys"
    }
}
```

## Updated user information for current user

запрос PUT https://blog.kata.academy/api/user

```
{
  "user": {
    "bio": "BioBio"
  }
}
```

ответ

```
{
    "user": {
        "username": "zajak",
        "email": "zajak@mail.ru",
        "token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpZCI6IjYzM2ViMTU0M2NmNzA1MWIwMDgyYWFmOCIsInVzZXJuYW1lIjoiemFqYWsiLCJleHAiOjE2NzAyMzc1ODcsImlhdCI6MTY2NTA1MzU4N30.w_UZo041JOAtGRZQ5uBe5-FVA8Lb24CzU1PajF0bBmI"
        "bio": "BioBio"
    }
}
```

## Gets the currently logged-in user

запрос GET https://blog.kata.academy/api/user

ответ

```
{
    "user": {
        "username": "zajak",
        "email": "zajak@mail.ru",
        "token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpZCI6IjYzM2ViMTU0M2NmNzA1MWIwMDgyYWFmOCIsInVzZXJuYW1lIjoiemFqYWsiLCJleHAiOjE2NzAyMzc1ODcsImlhdCI6MTY2NTA1MzU4N30.w_UZo041JOAtGRZQ5uBe5-FVA8Lb24CzU1PajF0bBmI"
        "bio": "BioBio"
    }
}
```
