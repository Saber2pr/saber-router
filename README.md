# @saber2pr/router

> router.

```bash
# from npm
npm install @saber2pr/router

# from github
git clone https://github.com/Saber2pr/@saber2pr/router.git
```

# API

## Router

```ts
// config Router
Router.container = document.getElementById('#root')
Router.render = ReactDOM.render

// routes map
Router({
  '/': '/profile', // redirect
  '/profile': () => <Profile />,
  '/repo': () => <Repo />,
  '/news': () => <News />,
  '/find': () => <Find />,
  '/menu': () => <Menu />,
  '/followers': () => <Followers />,
  '/following': () => <Following />,
  '/login': () => <Login />,
  '/error': () => <Error />,
  '/usersFrom': () => <UsersFrom />
})

const cancel = Router('/usersFrom', () => <UsersFrom />)

cancel() // cancel route /usersFrom
```

## push

```ts
push('/login')

push('/login', false) // scroll not reset
```

## tsx

```ts
<Anchor href="/login">login</Anchor>
```

---

## start

```bash
npm install
```

```bash
npm start

```

> Author: saber2pr
