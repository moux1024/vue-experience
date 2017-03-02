## vue项目收获

### 踩坑记录
1 使用对象属性值作为组件的属性，导致无法检测到属性改变
  ```js
  data() {
    return {
      accounts: [
        [],[]
      ]
    }
  },
  ```
  ```html
  <ul>
    <li v-for="item in accounts[0]" class="order_info">
      <account-one :item=item></account-one>
    </li>
  </ul>
  ```
