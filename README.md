https://json-server-vercel1-delta.vercel.app/

https://json-server-vercel1-delta.vercel.app/users
https://json-server-vercel1-delta.vercel.app/companies
https://json-server-vercel1-delta.vercel.app/contacts
https://json-server-vercel1-delta.vercel.app/contacts/1

Filter
https://json-server-vercel1-delta.vercel.app/users?id=1&id=2

Paginate
https://json-server-vercel1-delta.vercel.app/users?_page=1&_limit=2
https://json-server-vercel1-delta.vercel.app/users?_page=2&_limit=2

Slice

Sortings
https://json-server-vercel1-delta.vercel.app/users?_sort=age
https://json-server-vercel1-delta.vercel.app/users?_sort=age&_order=desc
https://json-server-vercel1-delta.vercel.app/users?_sort=age,lastName

Operators
https://json-server-vercel1-delta.vercel.app/users?id_ne=1
https://json-server-vercel1-delta.vercel.app/users?age_gte=20&age_lte=22

Full-text search
https://json-server-vercel1-delta.vercel.app/users?q=Tys

Relationships - include children resources
https://json-server-vercel1-delta.vercel.app/companies?_embed=users

Relationships - include parent resource
https://json-server-vercel1-delta.vercel.app/users?_expand=company

## Deploy JSON Server to Vercel

A template to deploy [JSON Server](https://github.com/typicode/json-server) to [Vercel](https://vercel.com), allow you to run fake REST API online!

Demo from this repository:

1. https://json-server-in.vercel.app
2. https://json-server-in.vercel.app/api/posts

### How to use

1. Click "**Use this template**" or clone this repository.
2. Update or use the default [`db.json`](./db.json) in the repository.
3. Sign Up or login into [Vercel](https://vercel.com).
4. From the Vercel dashboard, click "**+ New Project**" then "**Import**" your repository.
5. In the "**Configure Project**" screen, leave everything default and click "**Deploy**".
6. Wait until deployment is done, and your own JSON server is ready to serve!

## Default `db.json`

```json
{
  "posts": [{ "id": 1, "title": "json-server", "author": "typicode" }],
  "comments": [{ "id": 1, "body": "some comment", "postId": 1 }],
  "profile": { "name": "typicode" }
}
```

## Reference

1. https://github.com/typicode/json-server
2. https://vercel.com
3. https://shadowsmith.com/how-to-deploy-an-express-api-to-vercel
