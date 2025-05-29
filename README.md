# Le0der 工具包：Json工具

​	该工具包是 Unity 项目中的一个Json功能模块，主要作用是对Json的序列化与反序列化，目的是json简易解析和全平台适用。

​	工具是基于Newtonsoft Json的工具包，在实际使用中逐渐添加用到的方法和使用习惯，Newtonsoft解决了UnityJson工具不能解析复杂结构和LitJson解析Json对象过于困难的问题。

​	还有一个小问题就是我记不住Newtonsoft Json在Unity的Package Manager中引用的地址，所以就下载了离线包拿来用了。

​	遵循 Unity Package Manager（UPM） 规范开发，可通过 Git 快速引入项目中。

---

## 📦 包信息

- **包名**：`com.le0der.json`  
- **版本**：`1.0.0`  
- **最低支持 Unity 版本**：`2020.3`  
- **作者**：[Newtonsoft](https://www.newtonsoft.com/json),[Le0der](https://github.com/le0der)

---

## 📥 安装方式（通过 Unity Package Manager）

你可以通过以下任一方式集成该工具包：

---
### ✅ 方法 1：使用 Unity 编辑器内的 Package Manager 添加 Git 地址（推荐）

1. 打开 Unity 菜单：`Window > Package Manager`

2. 点击左上角的 `+` 按钮

3. 选择 `Add package from Git URL...`

4. 输入地址：

   ```arduino
   https://github.com/le0der-tools/com.le0der.json.git
   ```

5. 点击 Add 即可完成安装。
### ✅ 方法 2：使用 Git URL 添加依赖

​	编辑你的 Unity 项目的 `Packages/manifest.json` 文件，在 `"dependencies"` 节点中添加如下行：

```json
"com.le0der.json": "https://github.com/le0der-tools/com.le0der.json.git"
```

### ✅ 方法 3：通过本地路径引入（适用于开发测试）

1. 将工具包克隆至你的项目目录下，例如：

   ```json
   cd YourUnityProject/Packages
   git clone https://github.com/le0der-tools/com.le0der.json.git
   ```

2. 在 manifest.json 中添加依赖：

   ```json
   "com.le0der.json": "file:Packages/com.le0der.json"
   ```

   