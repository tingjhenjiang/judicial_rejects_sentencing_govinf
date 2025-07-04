# judicial_rejects_sentencing_govinf
「司法院拒絕依據政府資訊公開法提供量刑資訊系統所使用的資料」專案

## 緣起
先前憲法法庭就死刑是否違憲審理時，看到國內一直以來沒有很好的實證研究，因此依據政府資訊公開法要求司法院提供量刑資訊系統（例如事實型量刑資訊系統）使用的資料集，以便結合修法歷程進行研究（量化研究、因果推論），而被司法院拒絕提供，因而有了這一次的行政爭訟。

## 司法院拒絕提供、公開資訊的理由之一：無法過濾後提供
司法院訴訟代理人林三元在台北高等行政法院114訴120案件114/06/09準備程序庭期開庭時宣稱拒絕提供其中理由之一是無法落實政府資訊公開法第18條第2項過濾後提供的義務，將一些特定類型案件過濾後提供。

## 司法院「無法過濾後提供」的宣稱實際為假，實際操作作為證據
「無法過濾後提供」實際為假，這個專案目的之一即戳破這個謊言。
這個專案裡面提供驗證用的資料及程式碼，可以實際操作。[實際操作過程錄影影片已經上傳到Youtube](https://youtu.be/rg-2ighECxg)。

## 使用資料的說明
*  必須要存放在同一個目錄
*  根據 environment.yml [創建 conda environment](https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html)
*  在 conda 環境中，用適當的開發軟體（如VS Code）執行 simulate_crime_sentencing_data_and_retrieval.ipynb 以復現 Python 部分
*  simulated_data.xlsx 用 Office Excel 開啟後，必須修改資料來源位置（資料→查詢與連線→選取查詢→右鍵編輯→選取步驟1→右鍵編輯來源→輸入正確檔案路徑）指向csv
*  安裝 docker 後使用 docker compose up -d 指令以建立資料庫軟體堆疊