### 1. snippets有効にする

1. ファイル → 基本設定 → 設定

    ![](img\2021-06-09-12-55-46.png)

2. input settings in seach area
3. click Text Editor
4. click Edit in settings.json
    ![](img\2021-06-09-12-58-05.png)

5. settings.jsonの最後所に以下のコードを追加する

    ```
    {

        ...

        "[markdown]":  {
            "editor.wordWrap": "on",
            "editor.quickSuggestions": true,
            "editor.snippetSuggestions": "top"
        },
        "editor.fontLigatures": null,
    }
    ```

### 2. snippetsの登録

1. ファイル → 基本設定 → 設定 → UserSnippets

    ![](img\2021-06-09-12-17-26.png)

2. new snippets file for markdown and input file name
    ![](img\2021-06-09-12-19-25.png)

3. 以下のコードをnew fileに追加する
   
    ```html
    {

        ...

        "text background color cyan":{
            "prefix": "color-span-bg-cyan",
            "body": [ "<span style='background-color:cyan'>$1</span>" ],
            "description: "text background color cyan"
        }, 

        "text font color orangered":{
            "prefix": "color-font-orangered",
            "body": [ "<font style='color:orangered'>$1</font>" ],
            "description: "text font color orangered"
        },
        ...
    }

    ```

### 3. snippetsの利用

input col.. すると下記提示メッセージが出て来ます
![](img\2021-06-09-13-06-25.png)

enterを叩くと下記コードが出てくる
![](img\2021-06-09-13-08-26.png)
