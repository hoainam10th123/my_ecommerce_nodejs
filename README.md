# my_ecommerce_nodejs

### Login:
>**POST** - http://localhost:5000/api/v1/users/login

```json
{
    "email": "hoainam10th@gmail.com",
    "password": "123456"
}
```

### Register:
>**POST** - http://localhost:5000/api/v1/users/register

```json
{
    "name":"Nguyễn Tấn Đạt",
    "lastName": "Nguyễn",
    "address": "AGU",
    "city": "Long Xuyên",
    "state": "An Giang",
    "country": "Việt Nam",
    "email": "datnguyen@gmail.com",
    "password": "123456"
}
```

### Categories:
>**POST** - http://localhost:5000/api/v1/categories
**body:**

```json
{
    "name":"Danh muc test",
    "userId":"63b5786bc4eb41e32002aa33"
}
```

>**GET** - http://localhost:5000/api/v1/categories?pageNumber=1&pageSize=2
**Result:**

```json
{
    "pageNumber": "1",
    "pageSize": "10",
    "total": 13,
    "totalPages": 2,
    "data": [
        {
            "_id": "63b583a871ec3944e61f13b3",
            "name": "Danh muc 01",
            "status": true,
            "imgUrl": "http://localhost:5000/upload/images/img01.jpg",
            "user": {
                "_id": "63b5786bc4eb41e32002aa33",
                "name": "Nguyễn Hoài Nam",
                "id": "63b5786bc4eb41e32002aa33"
            },
            "__v": 0,
            "id": "63b583a871ec3944e61f13b3"
        },
        {
            "_id": "63b586689196af4cc93eb910",
            "name": "Danh muc 02",
            "status": true,
            "imgUrl": "http://localhost:5000/upload/images/img01.jpg",
            "user": {
                "_id": "63b5786bc4eb41e32002aa33",
                "name": "Nguyễn Hoài Nam",
                "id": "63b5786bc4eb41e32002aa33"
            },
            "__v": 0,
            "id": "63b586689196af4cc93eb910"
        }
    ]
}
```
