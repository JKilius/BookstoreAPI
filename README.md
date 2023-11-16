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


## Demo 

- [Docs: BookstoreAPI](https://bookstore.toolsqa.com/swagger)

<!--Nuotraukos paemimui is local repository>
![image name](../)
