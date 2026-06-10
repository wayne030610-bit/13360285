Smart Contract Sign-In System
專案簡介
這是一個基於 Solidity 智能合約的簽到系統，使用者可以透過區塊鏈完成簽到並查詢紀錄，確保資料不可竄改且透明。

開發環境

Remix IDE (https://remix.ethereum.org)

Solidity Compiler: 0.8.x

MetaMask (錢包，用來簽署交易)

測試網路: Sepolia 或 Goerli

編譯步驟

打開 Remix IDE

在左側檔案總管建立檔案 SignIn.sol，貼上合約程式碼

點選左側 Solidity Compiler → 選擇版本 0.8.x

按下 Compile SignIn.sol 完成編譯

部署步驟

在 Remix 左側選擇 Deploy & Run Transactions

環境選擇 Browser Extension  Sepolia Testnet-MetaMask
確認 MetaMask 已連線到測試網 (Sepolia 或 Goerli)

按下 Deploy，MetaMask 會跳出交易確認 → 按確認

部署完成後，合約地址會顯示在 Remix 下方

執行與測試方式

在 Remix 部署完成後，介面會顯示合約的功能按鈕

使用者可以呼叫 signIn() 按Transact後會出現MetaMask 按完確認和上面一樣彈出訊息後 簽到完成

使用者可以呼叫 getRecords() 查詢簽到紀錄

也可以用totalSigned看有多少帳號簽到
每次操作都會觸發 MetaMask 確認交易

建議截圖

Remix 編譯畫面

部署合約時 MetaMask 確認交易畫面

Remix 執行 signIn() 與 getRecords() 的結果

Etherscan 上的交易紀錄

專案結構
contracts/SignIn.sol      智能合約原始碼
README.md                 編譯與執行說明文件
screenshots/              部署與執行截圖