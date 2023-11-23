# Contents Of Table

-[API Reference](#api-reference)
-[Demo](#demo)

## API Reference

#### Create User

```http
  POST /Account/v1/User
```

| Object    | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `userName`| `string` | **Required**. User Name    |
| `password`| `string` | **Required**. User password |

#### Authorize account

```http
  POST /Account/v1/Authorized
```

| Object    | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `userName`| `string` | **Required**. User Name    |
| `password`| `string` | **Required**. User password |

#### Genetarte Token

```http
  POST /Account/v1/GenerateToken
```

| Object    | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `userName`| `string` | **Required**. User Name    |
| `password`| `string` | **Required**. User password |

#### Delete User

```http
  DELETE /Account/v1/User/{UUID}
```
| Parameters | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `UserId`    | `string` | **Required**. Valid user id to delete account |

#### Get account information

```http
  GET /Account/v1/User/{UUID}
```

| Parameters | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `UserId`    | `string` | **Required**. Valid user id to get account info |

#### Get all books information

```http
  GET /Bookstore/v1/Books
```

| Bearer Token | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `Token`    | `string` | **Required**. Valid Bearer token |

#### Add list of books to user account

```http
  POST /Bookstore/v1/Books
```

| Bearer Token | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `Token`    | `string` | **Required**. Valid Bearer token |

| Object | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `useId`   | `string` | **Required**. Valid user ID is required |
| `isbn`    | `string` | **Required**. Valid book ISBN to update book |

#### Delete books 

#### Update one book

```http 
  PUT /BookStore/v1/Books/{ISBN}
```

Authentification Bearer token

| Bearer Token | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `Token`    | `string` | **Required**. Valid Bearer token |

| Parameters | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `isbn`    | `string` | **Required**. Valid book ISBN to update book |

| Object | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `useId`   | `string` | **Required**. Valid user ID is required |
| `isbn`    | `string` | **Required**. Valid book ISBN to update book |

```http
  

## Demo 

- [Docs: BookstoreAPI](https://bookstore.toolsqa.com/swagger)

<!--Nuotraukos paemimui is local repository>
![image name](../)
