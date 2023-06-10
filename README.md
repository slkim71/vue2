# vue2

## Followed Youtube video
https://youtu.be/1GNsWa_EZdw

## Project setup
```
yarn install
```

### Compiles and hot-reloads for development
```
yarn serve
```

### Compiles and minifies for production
```
yarn build
```

### Lints and fixes files
```
yarn lint
```

### Customize configuration
See [Configuration Reference](https://cli.vuejs.org/config/).

## 20230610
- `</form>     </ul> 사이`
```
v-on 대신에 @ 도 가능 => @click

activePage == index ? 'active'" 로도 쓸 수 있어. 아니면 v-bind 로 쓰거나 더 줄여서 :class 로 사용 가능(v-bind directive on class, not html) 
active for what? -> nav에서 메뉴를 누르면 클릭한게 highlighted 되는데 이걸 active 됐다고 함 

<li class="nav-item">
    <a class="nav-link" aria-current="page" href="#">{{ links[1] }}</a>
</li>
<li class="nav-item">
    <a class="nav-link" aria-current="page" href="#">{{ links[2] }}</a>
</li>
```
- nav 안에
```
:class="{'navbar-light bg-light': !useDarkNavbar, 'navbar-dark bg-dark': useDarkNavbar}"

If while loop works, this kind of expression is difficult to read and understand what is going on here.
So, instead of using combined css class with elements in nav, extract this line out into an object and just reference :class="" with navbarClasses.
And define the navbarClasses object in our data.
```
