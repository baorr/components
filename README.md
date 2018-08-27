# components
## 1. 任何一个组件都多个状态，并且总会出于某一状态。
## 2. 任何一个组件从一个状态转移到另一个状态，中间可以定义多个子状态。
## 3.组件的状态可以是无序的，也可以是有序的。但从一个状态转移到另个状态的子状态是有序的，但返回结果可以是无序的也可以是有序的。
## 4. 每个组件都有自己的公开状态和隐私状态。
## 5. 每个组件都可以在某种状态下唤起自己本身的下个状态或者其他组件（N>=1）的某个状态。
## 6. 具有输入的组件功能的组件，一定要有一下几种状态
### a. 进入输入（in）
### b. 输入中（typing）
### c. 暂停输入（pause）

## 7. 任何一个显示组件，一定要有一下几种状态
### a. 显示（show），
### b. 获得焦点（on）
### c.变化中（tansform）
### e. 失去焦点（leave）
### f. 只读（readonly）
### g. 不可用（disabled）

## 8.所有组件的实例对象要有一个唯一的对应的uuid ，并且把实例引用存在一个公共管理仓库中。
## 9. 所有组件的公共state，在公共仓库中都需要有一个组件的uuid和对应的state做对应。
