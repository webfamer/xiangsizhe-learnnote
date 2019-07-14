# DOM事件
事件源.事件 = 事件处理函数  
- **获取事件源的形式：**
1. document.getElementById  
2. document.getElementsByClassName  
3. document.getElementsByTagName  
- **节点间关系获取**  
1. parentNode //父亲节点  
    // nextElementSibling：非标准属性   
    // 火狐、谷歌、IE9+版本：都指的是下一个元素节点（标签)。  
    // ie678中没有这个属性  
2. 兼容写法：li3.nextElementSibling || li3.nextSibling  
3. firstChild和firstElementChild  lastChild和lastElemetChild  兼容写法同上  
4. childNodes 获取所有字节点   children 获取所有元素节点  
// children 获取 所有元素子节点(不包括空格换行符)  
// 在 IE6/7/8 中包含注释节点（在 IE678 中，注释节点不要写在里面）。  