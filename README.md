# 🚀 Manage Azure Storage – Azure Lab Project

## 🧪 Lab Overview
This lab demonstrates how to create, configure, and secure Azure Storage resources including **Blob containers** and **File shares**. You'll explore lifecycle management, access control, and network restrictions using the Azure portal.

> ⏱ Estimated Duration: ~50 minutes  
> 🌍 Region Used: East US  
> 🔐 Prerequisite: Azure subscription (feature availability may vary by type)

---

## 🧩 Scenario
Your organization is migrating infrequently accessed files from on-premises storage to Azure. The goal is to reduce costs using lower-priced storage tiers and evaluate Azure’s built-in protection mechanisms—network access, authentication, authorization, and replication. You’ll also assess Azure Files as a potential host for legacy file shares.

---

## 🛠️ Tasks Breakdown

### 1️⃣ Create and Configure a Storage Account
- Use **Geo-redundant storage**
- Disable **public network access**
- Enable **lifecycle management** to move blobs to cool tier after 30 days
- Configure **network access scope** to selected IPs and virtual networks

### 2️⃣ Secure Blob Storage
- Create a private blob container named `data`
- Apply **time-based retention policy** (180 days)
- Upload a file to folder `securitytest` with:
  - Block blob type
  - Hot access tier
  - 4 MiB block size
- Generate **SAS token** for limited access
- Validate access restrictions via InPrivate browser

### 3️⃣ Secure Azure File Storage
- Create a file share named `share1` (Transaction optimized tier)
- Use **Storage Browser** to:
  - Upload files
  - Create folder structures
- Restrict access using:
  - Virtual network `vnet1`
  - Service endpoints for `Microsoft.Storage`
  - Removal of public IP access

---

## 🧠 Skills Demonstrated
- Azure Storage provisioning and configuration
- Blob and file access control via SAS and network rules
- Lifecycle management and cost optimization
- Immutable blob policies and retention strategies

---

## 📎 Notes
- Lab simulations previously provided have been retired.
- Public access is disabled by default—use SAS for controlled sharing.
- Network restrictions may take a few minutes to apply.

---

## 🧾 License
This lab was created as part of a campus project. Feel free to fork, adapt, and remix for educational or portfolio use.

