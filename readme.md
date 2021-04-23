# 喵音译者

功能演示

https://catt-l.github.io/MeowTranslator/



采用JavaScript实现, 与兽音译者同样的算法, 不过转换字符改成了`喵呜啊~`, 兽音译者也可以自定义字符, 因此完全可以相互兼容



### 使用方法



#### 人话 -> 喵语

```javascript
import MeowTranslator from './MeowTranslator'

// 人话->喵语
var strMeow = MeowTranslator.parseToMeow("睡了睡了，再不睡要猝死惹 QAQ");
console.log(strMeow);

// ~呜喵呜~啊喵啊喵呜喵啊喵喵~~啊~呜~~喵喵喵喵~喵喵喵啊~呜啊呜呜~~喵喵喵啊~~啊呜呜啊~啊呜喵~喵呜~啊啊啊喵喵~呜喵呜喵喵喵啊喵啊啊啊啊呜喵啊~啊喵呜~呜喵~啊呜喵喵呜呜啊喵啊~呜~呜啊喵喵喵喵呜呜喵喵~呜喵呜呜啊~啊喵啊喵啊呜~啊~喵~喵~呜喵~喵喵啊
```

#### 人话 -> 自定义字典

字典为4个字符长度, 且不能重复

```javascript
import MeowTranslator from './MeowTranslator'

// 人话->自定义字典
var strMeow = MeowTranslator.parseToMeow("睡了睡了，再不睡要猝死惹 QAQ", ".:…·");
console.log(strMeow);

// ·:.:·….….:.…..··…·:··....·...…·:…::··...…··…::…·…:.·.:·………..·:.:...….…………:.…·….:·:.·…:..::….…·:·:…....::..·:.::…·….….…:·…·.·.·:.·..…
```



#### 说人话!

```javascript
import MeowTranslator from './MeowTranslator'

var strHuman = MeowTranslator.parseToHuman("·:.:·….….:.…..··…·:··....·...…·:…::··...…··…::…·…:.·.:·………..·:.:...….…………:.…·….:·:.·…:..::….…·:·:…....::..·:.::…·….….…:·…·.·.·:.·..…");

console.log(strHuman);

var strHuman = MeowTranslator.parseToHuman("~呜喵呜~啊喵啊喵呜喵啊喵喵~~啊~呜~~喵喵喵喵~喵喵喵啊~呜啊呜呜~~喵喵喵啊~~啊呜呜啊~啊呜喵~喵呜~啊啊啊喵喵~呜喵呜喵喵喵啊喵啊啊啊啊呜喵啊~啊喵呜~呜喵~啊呜喵喵呜呜啊喵啊~呜~呜啊喵喵喵喵呜呜喵喵~呜喵呜呜啊~啊喵啊喵啊呜~啊~喵~喵~呜喵~喵喵啊");

console.log(strHuman);

// 睡了睡了，再不睡要猝死惹 QAQ


```





![睡了睡了再不睡要猝死惹](assets/readme/%E7%9D%A1%E4%BA%86%E7%9D%A1%E4%BA%86%E5%86%8D%E4%B8%8D%E7%9D%A1%E8%A6%81%E7%8C%9D%E6%AD%BB%E6%83%B9.gif)

