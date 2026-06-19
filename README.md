### 1. 履歷版面壓縮回 1 頁 (保證字體大小)                                                                               
                                                                                                                          
  我剛剛修改了底層的 HTML CSS 模板。我沒有動到 10.5 的底線，而是將原本稍微偏大的 11.5px 微調到  11px ，同時把每一個區塊   
  (Section) 之間的空白 margin 縮減了 2~4px。                                                                              
  這個微調非常完美，字體依然清晰易讀，但已經成功把包含 ITA 在內的所有履歷完美收攏回 1 頁了！你可以隨時點開原連結重新確認。
  ──────                                                                                                                  
  ### 2. 如何在 GitHub 用 README 吸引 Recruiter / Hiring Manager？                                                        
                                                                                                                          
  針對 Automated AI Financial Data Pipeline 這個專案，你的目標受眾有兩種：                                                
                                                                                                                          
  1. Recruiter (HR)：他們看不懂程式碼，他們只看「關鍵字」跟「商業價值」。                                                 
  2. Hiring Manager (技術主管)：他們看「系統架構」跟「你用了什麼現代化工具 (n8n, MCP, GCP)」。                            
                                                                                                                          
  為了一次擊中這兩種人，你的 GitHub  README.md                                                                            
  絕對不能長得像一堆冷冰冰的設定檔教學。你需要把它當作「產品發表頁」來寫。以下是我強烈建議的 README                       
  結構大綱，你可以直接拿去填空：                                                                                          
                                                                                                                          
  #### 🏆 高手級 README 呈現架構：                                                                                        
                                                                                                                          
  1. 標題與視覺 (Hero Section)                                                                                            
  第一眼就要告訴大家這個專案在幹嘛。                                                                                      
                                                                                                                          
    # 🤖 AI-Powered Financial Data Pipeline                                                                               
    > An end-to-end automated bookkeeping workflow using n8n, GCP, and AI Agents to eliminate manual data entry.          
                                                                                                                          
    ![GCP](https://img.shields.io/badge/GCP-Deployed-blue) ![n8n](https://img.shields.io/badge/n8n-Workflow-orange)       
  ![LLMs](https://img.shields.io/badge/AI-Model_Context_Protocol-purple)                                                  
                                                                                                                          
  2. 💥 Business Impact (給 Recruiter 看的「商業價值」)                                                                   
  （把我們剛剛在履歷寫的 PAR 直接放進來，讓他們知道這個專案的含金量）                                                     
                                                                                                                          
    ## 🚀 Why I Built This (The Impact)                                                                                   
    Manual budget tracking is error-prone and time-consuming. I engineered this pipeline to:                              
    - **Eradicate 100% of manual data entry** for financial tracking.                                                     
    - **Categorize real-time transactions automatically** with zero human intervention using AI.                          
    - **Save dozens of hours monthly**, ensuring flawless financial reporting.                                            
  
  3. 🏗️ System Architecture (給技術主管看的「硬實力」)
  這是最重要的一步！ 絕對要畫一張架構圖。你可以用 Mermaid https://mermaid.js.org/ 語法直接在 Markdown 裡畫，Hiring Manager
  一看到這種架構圖，就會認定你具備「系統設計 (System Design)」的高級思維。
  
    ## 🧠 System Architecture
  
    ```mermaid
    graph LR
        A[Credit Card / Bank API] -->|Webhook| B(n8n Workflow)
        B --> C{AI Agent / MCP}
        C -->|Parse & Categorize| D[ezbookkeeping]
        D -->|Store Data| E[(GCP PostgreSQL)]
        C -->|Alert on anomalies| F[Slack / Email]
  
  (在 GitHub 上這會自動渲染成一張很專業的流程圖)
  
  4. ✨ Key Features (核心功能展示)
  用條列式說明你解決了什麼技術難題：
  
  • Model Context Protocol (MCP): Integrated intelligent agents to understand transaction context instead of relying on   
  brittle Regex rules.
  • n8n Orchestration: Managed the entire ETL workflow, handling API limits and error retries natively.
  • GCP Deployment: Fully containerized and hosted on Google Cloud for high availability.
  
  5. 🛠️ Tech Stack (清晰的技術堆疊)
  
  • Orchestration: n8n
  • Cloud/Database: Google Cloud Platform (GCP), PostgreSQL
  • AI/Logic: LLMs, Model Context Protocol (MCP)
  • Application: ezbookkeeping
  
  6. 🎬 Demo / Proof of Work (極度推薦！)
