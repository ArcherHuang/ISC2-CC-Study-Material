# Security Concepts 安全概念
* CIA Traid are three main goals
  * CIA 是三個主要目標

## Confidentiality 機密
* Confidentiality protects information from unauthorized disclosure.
  * 機密性保護信息免遭未經授權的洩露。

#### Confidentiality Concerns
* 1. Snooping 窺探
  * snooping gathering information that is left out in the open.
    * 窺探收集公開遺漏的信息。
  * "Clean desk policies" protect against snooping.
    * 清理桌面策略”防止窺探。
* 2. Dumpster Diving 垃圾箱潛水
  * Dumpster diving is to dump data anywere or dustbin.
    * 垃圾箱潛水是將數據轉儲到任何地方或垃圾箱。
  * "Shedding" protects against dumpster diving.
    * “脫落”防止垃圾箱潛水。
* 3. Eavesdropping 竊聽
  * listing sensitive information
    * 列出敏感信息
  * "Rules about sensitive conversations" prevent eavesdropping
    * “關於敏感對話的規則”防止竊聽
* 4. Wiretapping 竊聽
  * Electronic evaesdropping - listing through wire(internet)
    * 電子竊聽 - 通過電線竊聽（互聯網）
  * "Encryption" protects against Wiretapping
    * “加密”防止竊聽
* 5. Social Engineering 社會工程學
  * The attacker uses psychological tricks to persuade an employee to give then sensitive information or access to internal systems.
    * 攻擊者使用心理技巧說服員工提供敏感信息或訪問內部系統。
  * Best defence is to "Educating users"
    * 最好的防禦是“教育用戶”

## Integrity 完整性
* Integrity protects information from unauthorized changes.
  * 完整性保護信息免遭未經授權的更改。

#### Integrity Concerns
* 1. Unauthorized modification 未經授權的修改
  * Attacks make changes without permission.
    * 攻擊在未經許可的情況下進行更改。
  * "Least priviege" protects against integrity attacks
    * “最小特權”可防止完整性攻擊
* 2. Impersonation 冒充
  * Attacks pretend to be someone else
    * 冒充他人進行攻擊
  * "User education" protects against attacks
    * “用戶教育”防範攻擊
* 3. Man-in-the-middle (MITM) 中間人 (MITM)
  * Attacks place the attacker in the middle of a communications session.
    * 攻擊將攻擊者置於通信會話的中間。
  * "Encryption" protects against MITM attacks
    * “加密”防止 MITM 攻擊
* 4. Replay 重播
  * Attacks eavesdrop on logins and reuse the captured credentials.
    * 攻擊竊聽登錄並重複使用捕獲的憑據。
  * "Encryption" protects against Replay attacks
    * “加密”防止重放攻擊

## Availability 可用性
* Availability protects authorized access to systems and data.
  * 可用性保護對系統和數據的授權訪問。

#### Availability Concerns
* 1. Denial of service (DoS) 拒絕服務 (DoS)
  * Unlimited request to a server
    * 對服務器的無限請求
  * "Block unauthorized connections" to protect against denial of service attacks.
    * “阻止未經授權的連接”以防止拒絕服務攻擊。
* 2. Power outages 停電
  * Naturally or Man-made
    * 自然或人造
  * "Redundant power and generators" protect against power outages.
    * “冗餘電源和發電機”可防止停電。
* 3. Hardware failures 硬件故障
  * any component failures
    * 任何組件故障
  * "Redundant components" protect against hardware failure
    * “冗餘組件”防止硬件故障
* 4. Destruction 破壞
  * Naturally or Man-made
    * 自然或人造
  * "Backup data centers" protect against destruction.
    * “備份數據中心”防止破壞。
* 5. Service outages 服務中斷
  * Programing error and the failure of underlying equipment.
    * 編程錯誤和底層設備故障。
  * building systems that are resilient in the face of errors and hardware failures.
    * 構建在面對錯誤和硬件故障時具有彈性的系統。

## Authentication and authorization 認證與授權
* The access control process consists of three steps that you must understand. These steps are identification, authentication and authorization.
  * 訪問控製過程包括您必須了解的三個步驟。 這些步驟是識別、認證和授權。

* 1. Identification incolves making a claim of identity. 識別涉及提出身份聲明。
  * Electronic identification commonly uses usernames
    * 電子身份識別常用用戶名
* 2. Authentication requires proving a claim of identity. 身份驗證需要證明身份聲明。
  * Electronic autherntication commonly uses passwords.
    * 電子認證常用密碼。
* 3. Authorization ensures that an action is allowed. 授權確保允許操作。
  * Electronic authorization commonly uses access control lists.
    * 電子授權通常使用訪問控制列表。

* Authentication and authorization process, access control systems also provide "Accounting" functionality that allows administrators to track user activity and reconstruct that activity from logs. This may include tracking user activity on systems and even logging user web browsing history.
  * 身份驗證和授權過程，訪問控制系統還提供“會計”功能，允許管理員跟踪用戶活動並從日誌中重建該活動。 這可能包括跟踪用戶在系統上的活動，甚至記錄用戶的網絡瀏覽歷史記錄。

## Password security 密碼安全
* Password mechanisms 密碼機制
  * Password length requirements set a minimum number of characters. 
    * 密碼長度要求設置了最少字符數。
  * Password complexity requirements describe the types of characters that must be included.
    * 密碼複雜性要求描述了必須包含的字符類型。
  * Password expiration requirements force password changes.
    * 密碼過期要求強制更改密碼。
  * Password requirements prevent password reuse.
    * 密碼要求防止密碼重複使用。

## Multifactor authentication 多重身份驗證
* Multifactor authentication combines two different authentication factors.
  * 多因素身份驗證結合了兩個不同的身份驗證因素。
* Three different authentication factors. Something you know, something you are and something you have.
  * 三種不同的身份驗證因素。 你知道的東西，你的東西和你擁有的東西。

#### something you know 你知道的事
* Passwords, PIN's, Security questions.
  * 密碼、PIN、安全問題。
#### something you are 你是什麼
* Biometric security mechanisms.
  * 生物識別安全機制。
#### something you have 你有的東西
* Software and hardware tokens.
  * 軟件和硬件令牌。
#### single sign-On (SSO)
* Shares authentiacated sessions across systems 跨系統共享經過身份驗證的會話
  * In a single sign on approach, users log on to the first SSO enabled system that they encounter. And then that login session persists across other systems until it expires. If the organization sets the expiration period to be the length of a business day, that means that users will only need to log in once a day and their single sign on is then going to last the entire day.
    * 在單點登錄方法中，用戶登錄到他們遇到的第一個啟用 SSO 的系統。 然後該登錄會話在其他系統中持續存在，直到它過期。 如果組織將有效期設置為一個工作日，這意味著用戶每天只需登錄一次，然後他們的單點登錄將持續一整天。


## Non-repudiation 不可否認性
* Non-repudiation prevents someone from denying the truth.
  * 不可否認性防止某人否認真相。
* Solved the issue with 解決了這個問題
  * 1. Signed contracts
    * 簽訂合同
  * 2. Digital signatures
    * 數位簽章
  * 3. Video surveillance
    * 視頻監控

## Privacy 隱私
* Privacy Concerns 隱私問題
  * 1. Protecting our own data.
    * 保護我們自己的數據。
  * 2. Educating our users.
    * 教育我們的用戶。
  * 3. Protecing data collected by our organizations.
    * 保護我們組織收集的數據。

* Private information may come in many forms. Two of the most common elements of private information are "Personally identifiable information" and "Protected health information". 私人信息可能有多種形式。 私人信息的兩個最常見元素是“個人身份信息”和“受保護的健康信息”。
  * 1. Personally identifiable information, or PII, includes all information that can be tied back to a specific individual. 
    * 個人身份信息，或 PII，包括所有可以與特定個人聯繫起來的信息。
  * 2. Protected health information, or PHI, includes healthcare records that are regulated under the Health Insurance Portability and Accountability Act. Otherwise known as HIPAA.
    * 受保護的健康信息 (PHI) 包括受《健康保險流通與責任法案》監管的醫療保健記錄。 也稱為 HIPAA。