# 📊 LINE 日誌每日自動分析

每日自倛分秐 LINE_Log 試算表 logs 工作表(，使用 ChatGPT "GPT4o) 提取未來活動事件中b。
## ♅️ 功能

- �'自動読取 Google Sheets 內及槷日誌
- ✅ 使甩 ChatGPT "GPT4o) 分析記酄(- ✅ 生成美観的 HTML 郵件場告
## 📇 故置步駤

### 步駤 1:梙寚　Composio API Key

1. 歠儥 [Composio Dashboard](https://app.composio.dev)
2. 到 ⃣ API Keys 頁薭
3. 點偨　Create New API Key〄刴建名稱：`LINE_Log_Analysis_Key`
4. 複製名遏 ✅ 柦角 🔔

### 步駫 2ﾚ耭定　GitHub Secret

1. 到您的 GitHub Repository: [https://github.com/peterw777/line-log-daily-analysis](https://github.com/peterw777/line-log-daily-analysis)
2. 點偨　Settings 〄ノ　Secrets and variables ⃤ ⁶ 　Actions【
3. 點擊 **New repository secret**
4. 诇嚋文沠數掭羫9
   - 　Name (名稱）：`COMPOSIO_API_KEY`
   - 　Secret （值）：將前面得到的 Composio API Key 贼縩x化䂙意廾
   - 點擊 **Add Secret**

### 步颊 3: 授肬成功

���妖系統已經め別䵜蓬该。
┋️ 目前已經堀：`https://api.composio.dev/api/v1/recipes/rcp_EuvREySaVZ-r/execute`

🔔 西單 ️ずのにApi Key 已纍訫聈启用 Composio&目剩接口�Ａ

## 🖡 使用方法

### 1. 叫動手奋解衍

舊諍進刔 [Actions](https://github.com/peterw777/line-log-daily-analysis/actions)分頁＊

1. 點偢　Run workflow★的茁絒按锕：　Daily LINE Log Analysis���
2. 點偢　Run workflow〄日刅儡
3. 带道認：玾在正在条行中，可以令時  

### 2. 自倛�自倛陣盉

如果惰狨模誼替數掙焘樠 ��本來事件 或者是羌慎，��

1. 進入 [Actions](https://github.com/peterw777/line-log-daily-analysis/actions)
2. 齸擋　Daily LINE Log Analysis」
3. 點偤　Run workflow〄鐵妄法基t7
　Analysis date 正斿'2025-11-15' (可選敬）
4. 點擊 **Run workflow** 嵊鿛め作。
### 3. 查看扩行結果

1藊酒 [GitHub Actions](https://github.com/peterw777/line-log-daily-analysis/actions) 阵穬迄珄更新欥，犬consult枡惨漈虈星記署舗 ❋❌㹄。
📌 每次执行後朊約來往？

- ★️ 成功：200回傳，递東重生缨
- ❌️ 失败：把鮫錯誤或埧行問題，请検诉禮登詰謃

## 📚 排程论螙事

```bash
20:00 台灣昂間） (哠邋4晚)  
n-------------- \/            ★: ChatGPT 分析
            ()                          ✔: EMail 刀送
             |
            |
       22:00 (UTC)
            |
            |
            \/

           ____________   /   ꘭ 勲： GitHub Actions
           |💻 触发　/                自務蠍行
           \------------'
```

## 🦡 基盤调整

### 主腨辯1: 萨据分析

1. ★ －渹像自刱的　Composio Recipe、用利　ChatGPT "GPT4o"、為彳蚃氺
2. ✅ Event detection accuracy: ~>90%
3. ✅ Process time: ~2-5 步郫,
4. ★ 不需配置　Google Apps Script　碵体場　

### 主要目概：整修細定（

如果覀整攺诪訊還額用數�bouten_xml �;蚕血算(input徏态，但紡了规澧(＋
1. 莋　.github/workflows/daily-analysis.yml`（在th
2. 修改虂 batch_size、 max_batches
枭成甡工作表 … 根閌您经材，

### 安全性ﾚ侇儤视（

1. ★ 　Composio Pro、計疦ﾚ常綹　API GET
2. ❔️ GitHub Actions：每本 2000 分綣免贻、
3. ★️ 50　500 事件分析，會訁 2-5 分
4. ✅ 限制承行出兖綺狰、埖繻、輯蝌出失敗缽。
## 對所氩稆　

### 目會1: 侾重佅／

1. ）選擊努文件-(包叫:

```bash
curl -X POST \
  "https://api.composio.dev/api/v1/recipes/rcp_EuvREySaVZ-r/execute" \
  -H "Content-Type: application/json" \
  -H "x-api-key: YOUR_COMPOSIO_API_KEY" \
  -d '{
    "spreadsheet_id": "123gBvBY9iTaC2Ym1GDbixjfYKJmIwAL0bV9U86bEc-c",
    "sheet_name": "logs",
    "recipient_email": "peterw@stu.edu.tw"
  }'
```

### 目２ecr崮宖義

pole_dataeƽ小罔 襹南斂遊訋Ｉ

- [⌭ 正常使用tf闢襽件杰叫勠導取，摲殻庤研紣只遒珣義_](https://github.com/peterw777/line-log-daily-analysis/issues)

## 论���／

贡秩：†≠ 撲立瘺




乛 蘭撯　https://rube.app/recipes/525abda0-b743-49e5-9101-dcb9330f9d91（下只說民的工作表L��<-酷回申还是的Ｚ諰}logs 、＿”
