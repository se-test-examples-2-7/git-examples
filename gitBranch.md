# git branch ....

Git 分支（Branch）是用來管理不同開發線路的核心工具。常見的使用情境與指令如下：

### 1. 檢視分支

* **查看本地所有分支：**
```bash
git branch

```


*(前方有 `*` 號且顏色不同的為當前所在分支)*
* **查看本地與遠端（Remote）的所有分支：**
```bash
git branch -a

```



---

### 2. 建立與切換分支

* **建立新分支：**
```bash
git branch <branch-name>

```


* **切換到指定分支：**
```bash
git checkout <branch-name>

```


*（較新的 Git 版本亦可使用：`git switch <branch-name>`）*
* **建立並直接切換到新分支（最常用）：**
```bash
git checkout -b <branch-name>

```


*（較新的 Git 版本亦可使用：`git switch -c <branch-name>`）*

---

### 3. 合併與刪除分支

* **合併分支：**
先切換回目標分支（例如 `main`），再執行合併指令：
```bash
git checkout main
git merge <branch-name>

```


* **刪除已合併的分支：**
```bash
git branch -d <branch-name>

```


* **強制刪除分支（不管是否已合併）：**
```bash
git branch -D <branch-name>

```



---

### 4. 重新命名分支

* **修改當前所在分支的名稱：**
```bash
git branch -m <new-branch-name>

```



---