# rime-poj

[Rime](https://rime.im) 臺語 (Hô-ló-ōe) 白話字 ( https://en.wikipedia.org/wiki/Pe̍h-ōe-jī ) 輸入方案

授權條款：見 [LICENSE](LICENSE)

## 安裝

與其他依託Rime的輸入法一樣，國際音標是一組獨立發行的「輸入方案」數據包（或稱「配方」）。

安裝適合您的設備及操作系統的 [Rime輸入法](https://rime.im/download) 程序後，請按照以下說明，配置POJ輸入法。


### 手動安裝及配置

1.  從 [GitHub代碼庫](https://github.com/rime/rime-ipa) 下載全部原始碼的ZIP壓縮檔，或單獨下載所需的YAML文件。

2.  打開Rime輸入法 [用戶文件夾](https://github.com/rime/home/wiki/UserData)，將下載的YAML文件移到此處。

3.  啓用POJ輸入方案。

    在用戶文件夾創建或編輯文件 `default.custom.yaml`，將所需輸入方案的ID加入「輸入方案列表」配置選項：

    ```yaml
    patch:            # 若文件中已有該行，無須重複
      schema_list/+:  # 同上；"/+" 表示加添輸入方案，若無 "/+" 則表示以下列方案替換預設列表
        - schema: poj   # 依需選配
    ```

4.  完成以上步驟之後，[重新deploy](https://github.com/rime/home/wiki/CustomizationGuide#%E9%87%8D%E6%96%B0%E4%BD%88%E7%BD%B2%E7%9A%84%E6%93%8D%E4%BD%9C%E6%96%B9%E6%B3%95)Rime輸入法的工作資料，使上述配置改動生效。

## 輸入白話字

在Rime輸入法中按 `F4` 或 ``Control+` `` 打開 [方案選單](https://github.com/rime/home/wiki/UserGuide#%E4%BD%BF%E7%94%A8%E6%96%B9%E6%A1%88%E9%81%B8%E5%96%AE)，選取POJ（白話字）輸入方案，即可輸入對應編碼獲得音標符號。

運指齊按快速鍵 `Control+Shift+1` 在最近使用的兩個輸入方案（如常用的中文輸入法和白話字）之間相互切換。
### 聲調符號如何輸入
  - á：a2
  - à：a3
  - â：a5
  - ã：a6
  - ā：a7
  - a̍：a8
  - a̋：a9

**注意：調號在添加調符的母音後就要立刻添加，如tia5u，而非tiau5。**
### 葫蘆點o͘
  - 輸入 ou，有聲調則再後面輸入調號

### 鼻化韻
  - ⁿ：nn
  - ᴺ：NN

