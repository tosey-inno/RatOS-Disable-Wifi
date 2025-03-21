### 1. 透過網路線連接，並確認 `ratos.local` 可以連接至設備
![Image](https://github.com/user-attachments/assets/7b9b86aa-431a-478c-8b85-266e0729c553)

### 2. 開啟終端機，使用 `ssh` 連接至Raspberry Pi。(密碼 `raspberry`)
```
ssh pi@ratos.local
```
初次連接，會出現`fingerprinting` 的要求，請依照要求輸入`yes`
![Image](https://github.com/user-attachments/assets/91fdfabe-5e63-43f9-b479-999e46f6a2ff)

接著依提示輸入密碼 `raspberry`後，出現以下畫面代表連接成功。
![Image](https://github.com/user-attachments/assets/572ca365-4821-43e8-9f87-e77213ae38e2)

### 3. 關閉「自動啟動Wifi」功能
在終端機輸入
```
sudo systemctl disable autohotspot
```
使用`sudo` 指令會要求輸入系統密碼（`raspberry`），輸入完成後會出現以下畫面
![Image](https://github.com/user-attachments/assets/efb85045-0889-475e-abe9-1bb914fb2f0d)

### 4. 回到瀏覽器，進入`ratos.local` 重啟Raspberry Pi
![Image](https://github.com/user-attachments/assets/7a2b42b7-f5ac-427e-9cf8-75fd5b81fdb3)


### 5. 重啟後，使用瀏覽器確 `ratos.local`可連接至列印機，並確認`RatOS` WiFi訊號不再提示。
