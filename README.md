##Web_Server_IH & MyWebServer
這個 README 包含兩個 ASP.NET Core Web 伺服器應用程式的描述。


##先決條件
在您的電腦上安裝 .NET Core SDK (下載)


##MyWebServer
這是一個簡單的 ASP.NET Core Web 伺服器應用程式，對於根目錄 URL ("/") 的請求會回應 "Hello, world!"。

##開始
Step1: Clone或下載包含此程式碼的存儲庫。
Step2: 使用您喜歡的程式碼編輯器打開項目。
Step3: 使用以下命令構建並運行項目：
arduino
複製程式碼
dotnet run
在瀏覽器中導航至 http://localhost:5000 以查看 "Hello, world!" 訊息。


##項目結構
Startup.cs: 此檔案包含 ASP.NET Core 應用程式的設定。
MyWebServer.csproj: ASP.NET Core 應用程式的專案檔。


##如何使用
配置服務: 如果您需要向應用程式添加任何服務，可以在 Startup 類的 ConfigureServices 方法中執行。
配置中介軟體: 中介軟體組件在 Startup 類的 Configure 方法中配置。在這個例子中，我們使用了：
UseDeveloperExceptionPage: 在開發模式下添加開發人員例外頁面。
UseRouting: 啟用應用程式的路由。
UseEndpoints: 配置用於處理請求的端點。在這個例子中，我們有一個單獨的端點，用於回應對根 URL ("/") 的 GET 請求，並顯示 "Hello, world!" 訊息。


##Web_Server_IH
這是另一個 ASP.NET Core Web 伺服器應用程式，具有基本的身份驗證和授權功能。

##開始
Step1: Clone或下載包含此程式碼的存儲庫。
Step2: 使用您喜歡的程式碼編輯器打開項目。
Step3: 使用以下命令構建並運行項目：
arduino
複製程式碼
dotnet run
根據需要訪問應用程式的不同端點。


##項目結構
Program.cs: 此檔案包含 ASP.NET Core 應用程式的入口點，並配置 HTTP 請求管道。
Web_Server_IH.csproj: ASP.NET Core 應用程式的專案檔。


##如何使用
配置服務: 如果您需要向應用程式添加任何服務，可以在 Main 方法中的 WebApplication.CreateBuilder(args) 方法後執行。
配置身份驗證和授權: 在 Main 方法中，我們配置了基於 Negotiate 協商的身份驗證。並添加了授權服務。
配置 HTTP 請求管道: 在 Main 方法中，我們配置了 HTTP 請求管道，包括錯誤處理、HSTS、HTTPS 重新導向、靜態檔案服務、路由、授權和 Razor 頁面映射。

##貢獻
歡迎通過提交拉取請求或在 GitHub 存儲庫上開啟問題來貢獻此項目。


##致謝
此項目受到各種 ASP.NET Core 教程和文檔的啟發。
感謝 Microsoft.AspNetCore 團隊提供的工具和資源，用於開發使用 ASP.NET Core 的 Web 應用程式。

##作者
Ariel C.