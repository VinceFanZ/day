# 一行 JavaScript 代码

### 随机数组



```javascript
const shuffleArray = (arr) => arr.sort(() => Math.random() - 0.5);
// Testing
const arr = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10];
console.log(shuffleArray(arr));
```



### 复制到剪贴板



```javascript
const copyToClipboard = (text) => navigator.clipboard?.writeText && navigator.clipboard.writeText(text);
// Testing
copyToClipboard("Hello World!");
```



### Set 数组去重



```javascript
const getUnique = (arr) => [...new Set(arr)];
// Testing
const arr = [1, 1, 2, 3, 3, 4, 4, 4, 5, 5];
console.log(getUnique(arr));
```



### 检测黑夜模式



```javascript
const isDarkMode = () =>
  window.matchMedia &&
  window.matchMedia("(prefers-color-scheme: dark)").matches;
// Testing
console.log(isDarkMode());
```



### 滚动到顶部



```javascript
const scrollToTop = (element) => element.scrollIntoView({ behavior: "smooth", block: "start" });
```



### 滚动到底部



```javascript
const scrollToBottom = (element) => element.scrollIntoView({ behavior: "smooth", block: "end" });
```



### 生成随机颜色



```javascript
const generateRandomHexColor = () => `#${Math.floor(Math.random() * 0xffffff).toString(16)}`;
```





参考

[https://tapajyoti-bose.medium.com/7-killer-one-liners-in-javascript-33db6798f5bf](https://tapajyoti-bose.medium.com/7-killer-one-liners-in-javascript-33db6798f5bf)

