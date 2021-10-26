---
description: >-
  Import variables label table and value-labels table, then generate Stata code
  of the labelling operations.
---

# Label Stata

## 开始

本工具位于"Program"栏下。点击“Launch”启动工具。

![](<../../.gitbook/assets/image (5).png>)

## 使用

{% hint style="info" %}
开始前，你应该准备一个**同时包含变量标签表和值标签表**的.xlsx文件。

变量标签表中必须包含变量名、变量标签和变量使用的值标签的名字。对每一个变量，变量名是必须的，而变量标签和值标签的名字是可选的。

值标签表则需要包含值标签名、值和其对应的标签。对每一个值，其所属的值标签和其对应的标签都是必需的。

举个栗子，假设变量`A1`表示受访者的性别，而1表示男性，2表示女性，并且你将这一值标签命名为`A1_LAB`。A1就是变量名，“受访者的性别”是变量标签，而`A1_LAB`则是变量使用的标签，应该**同时在两张表里出现**。1和2则是值，而“男性”和“女性”则是值对应的标签。

工作表和列名可以随意命名。**每一张工作表都应当包含标题行。**
{% endhint %}

### 第一步 导入.xlsx文件

点击"Files -> Import"以导入.xlsx文件。

![](<../../.gitbook/assets/image (1).png>)

{% hint style="info" %}
请确保文件没有被其他进程占用，尤其是Excel。
{% endhint %}

### 第二步 设置

选择工作表和列。

![](<../../.gitbook/assets/image (3).png>)

### 第三步 生成Stata命令

点击"Generate -> Stata Command"以生成Stata命令。你将看到以下窗口。点击"Save As"将其保存到本地的.do文件。

![](<../../.gitbook/assets/image (2).png>)

{% hint style="info" %}
你可以在此窗口上编辑。“Save As”会将编辑的结果保存。
{% endhint %}
