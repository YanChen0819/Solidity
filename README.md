# Solidity 101 - Class 1

此篇為本作者實作 **Solidity 101** 教學，參考於 **WTF Academy**. 提供 Solidity code examples, exercises, and notes.  

## Table of Contents

- [Solidity 101 - Class 1](#solidity-101---class-1)
  - [Table of Contents](#table-of-contents)
  - [Introduction](#introduction)
  - [What is "Web 3.0" ?](#what-is-web-30-)
  - [Solidity 語法](#solidity-語法)
  - [1 st Contract : HelloWeb3.sol](#1-st-contract--helloweb3sol)


## Introduction

In this first class, you'll be introduced to basic concepts of Web3 and Solidity programming. The aim is to help you write your first "Hello Web3" contract and understand the underlying principles of decentralized applications (dApps).

在第一堂課中，我將補充 **WTF Academy** 程式範例外 Web3 和 Solidity 基本概念。最終編寫第一份「Hello Web3」合約，並瞭解分散式應用程式 (dApp) 的基本原理。

## What is "Web 3.0" ?

Web 3.0 與 Web 2.0 最大差異就是傳統 Web 2.0 需要一個組織作為中心管理網路服務，例如:Instagram(平台)管理文章，而 Web 3.0 藉由 peer-to-peer(P2P) 技術實現去中心。

## Solidity 語法
Solidity 是一種用於編寫以太坊虛擬機器（EVM）智能合約的程式語言。我認為掌握 Solidity 是參與鏈上專案的必備技能：區塊鏈專案大部分是開源的，如果你能讀懂程式碼，就可以規避很多虧錢項目。


## 1 st Contract : HelloWeb3.sol

```sol
// SPDX-License-Identifier: MIT
pragma solidity ^0.8.21;
contract HelloWeb3{
    string public _string = "";
}
```
- Solidity 註解以「//」開頭，後面跟著註解內容，註解不會被程式執行
- SPDX-License-Identifier 為程式碼所使用的軟體許可（license）可前往官網查看可用憑證，最常使用的是 MIT。
  


```sol  
// SPDX-License-Identifier: MIT
```


- 選用合約的版本，通常主流合約版本可以從 OpenZeppelin Wizard 提供的合約範本參考。
  
```sol 
pragma solidity ^0.8.21;
```
- 創建一份合約命名為 HelloWeb3。
- 創建一個「字串」物件並使其值為 "Hello Web3!"。

```sol
contract HelloWeb3{
    string public _string = "";
}
```
