# CMD-基礎命令
這裡介紹關於CMD的基礎常用命令。  
當命令為<font color="0000ab">藍色</font>時，則表示他為多型命令。

---
  
## 查詢相關命令  
### help
help：列出所有命令清單。  
help \<command\>：對該命令進行查詢。  

### 參數 /?  
\<command\> /?： 和help \<command\>效果一致。  
  
---

## 導覽相關命令  
### dir  
dir：觀看當前所在層級的所有檔案和子目錄。
dir /a：顯示具有指定屬性的檔案。  
> 屬性如下：  
> a:d：目錄  
> a:h：隱藏檔案  
> a:r：唯讀  
> a:s：系統檔案  
  
dir /b：使用單純格式，就是只顯示名稱，不顯示其他屬性。  
dir /d：與寬的列表格式相同，但是依照欄來排序。  
dir /n：使用新的長列表格式，檔名會顯示在最右方。  
dir /o：指定特定排序列出檔案。  
> 排列如下：  
> o:d：時間排序(從早到晚)  
> o:e：副檔名  
> o:g：優先列出子目錄  
> o:n：名稱排序  
> o:s：檔案大小  
  
dir /s：顯示指定目錄及所有子目錄中的檔案。  
  
### cd / chdir  
cd：顯示當前所在的目錄路徑。  
cd \<path\>：移動到所指定的目錄。
cd \<drive\>：移動到所指定的磁碟區。  
cd .. ：回到父層目錄。  
cd . ：代表當前目錄。  
　　
### md / mkdir  
md \<path\> ：根據指定的目錄做創建。  
  
### ren / rename
ren \<old\> \<new\>：重新命名檔案名稱。  
  
### <font color="0000ab">move</font>  
move \<src\> \<dest\>：  
* 如果dest不存在，則將src更名為dest。  
* 如果dest為目錄，則將src移動到dest裡。  
* 如果dest為檔案，則將src覆寫dest。
* src本身可以是檔案或目錄。
  
### <font color="0000ab">copy</font>  
copy \<src\> \<dest\>：  
* 如果dest不存在，則將src複製到dest。
* 如果dest為目錄，則將src複製到dest中。
* 如果dest為檔案，則將src覆寫dest，並向使用者確認。
* src本身只能是檔案。
  
### xcopy
xcopy /s \<src\> \<dest\>：複製每個目錄和子目錄，不包含空目錄。  
xcopy /e \<src\> \<dest\>：複製每個目錄和子目錄，包含子目錄。  
xcopy /y \<src\> \<dest\>：覆寫檔案時不詢問使用者。  
xcopy /i \<src\> \<dest\>：如果目的地不存在，且來源檔案有多個，認定目的地是目錄。  
  
### del / erase
del \<file\>：刪除指定檔案。
del \<path\\*\>  : ：刪除指定路徑下的所有檔案。  
del /q：安靜模式，不會逐一詢問使用者。  
  
### rd / rmdir
rd \<path\>：刪除指定路徑目錄。  
rd /s \<path\>：在遞迴模式下刪除指定路徑目錄。  
rd /q \<path\>：在安靜模式下刪除指定路徑目錄。  
rd /s /q \<path\>：在遞迴模式和安靜模式下刪除指定路徑目錄。  
  
---
[回目錄](../README.md)