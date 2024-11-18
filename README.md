# Introduction

<div align="center">
    <!-- Logo -->
    <a href="#" target="_blank">
        <img src="https://github.com/user-attachments/assets/c9ab7a1c-589f-4bda-984a-2fe267b43aae" 
        alt="Logo" width="290" height="290">
    </a>
</div>

<br>

<div align="center">
    <!-- Title -->
    <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&pause=1000&center=true&repeat=false&width=435&lines=Prestige+Koi+Auction">
</div>


## :ledger: Table of Contents

- [About](#beginner-about)
- [Features Overview](#-features-overview)
- [Project Structure](#-project-structure)
- [Usage](#zap-usage)
- [Gallery](#camera-gallery)
- [License](#lock-license)

##  :beginner: About
**Prestige Koi Auction** is a modern and user-friendly platform designed to facilitate the buying and selling of koi fish through live auctions. Built with scalability and transparency in mind, this platform enables **Koi Breeders**, **Managers**, **Staff**, and **Members** to interact seamlessly while maintaining fair and organized auctions.  

The system emphasizes:  
- **Efficient Management**: Streamlined processes for request approvals, inspections, and slot assignments.  
- **Financial Transparency**: Clear records of deposits, refunds, payments, and fees.  
- **Seamless User Experience**: Intuitive interfaces for both auction participants and administrators.  

## 🚀 **Features Overview**  

### 🎨 **User Management**  
- **Multiple Roles**: Supports **Koi Breeder**, **Manager**, **Staff**, **Member**, and **Guest**.  
- **Secure Authentication**: Powered by **JWT (JSON Web Tokens)**.  

### 📋 **Auction Management**  
- **Auction Sessions**:  
  - Managers create auction sessions with multiple lots.  
  - Each lot represents one koi fish for bidding.  
- **Request Approval Process**:  
  - KoiBreeders submit auction requests.  
  - Managers approve requests or assign inspections to Staff.  

### 💳 **Financial Transactions**  
- **Deposits and Refunds**:  
  - Members pay deposits to join auctions, and refunds are processed for non-winning participants.  
- **Automated Payments**:  
  - Winning bids are processed, and proceeds are shared with breeders after platform fees are deducted.  

### 📈 **Transparency & Insights**  
- Real-time auction status.  
- Detailed transaction history.

## 🛠️ **Tech Stack**  

| **Category**         | **Technologies**                     |  
|-----------------------|---------------------------------------|  
| **Backend**          | Java, Spring Boot, Microsoft Sql Server|  
| **Frontend**         | React, Vite, Tailwind                |  
| **Authentication**   | JWT (JSON Web Tokens)                |  
| **DevOps**           | Docker, GitHub, Jenkins, AWS EC2       |  

## 📂 **Project Structure**  

```plaintext  
prestige-koi-auction/  
│  
├── backend/         # Spring Boot backend source code  
│   ├── src/  
│   ├── pom.xml  
│   └── ...  
│  
├── frontend/        # Frontend source code (React/Vue/Angular)  
│   ├── src/  
│   ├── package.json  
│   └── ...  
│  
└── README.md        # Project documentation
````

## :zap: Usage
***
    This guideline is only for Windows 

### Environment Requirements
- Java 21
- Node.js 18+
- MSSQL 2019+
- Maven 3.9+
- Redis

### Tools requirements
- Intellij IDEA (or Commuity edition)
- Visual Studio Code (or anything code editor)

### Installation

#### Database
- We use **localhost** and database name is **Koi_project** for SQL Server in **application.properties**. You can change this based on your device
    ````bash
    sqlserver://localhost:1433;databaseName=Koi_project
    ````
-  In SQL Server, the **Koi_project** database must already exist, if not,  please use query below: 
    ````bash
    CREATE DATABASE Koi_project
    ````
- After created **Koi_project** database. Run the **Spring Boot back-end** for the first time so it automatically creates tables and records

- Now, the project also needs to have the data available using the query below:
    ````bash
    INSERT INTO AuctionType(auctionTypeName) VALUES('FIXED_PRICE_SALE')
    INSERT INTO AuctionType(auctionTypeName) VALUES('SEALED_BID')
    INSERT INTO AuctionType(auctionTypeName) VALUES('ASCENDING_BID')
    INSERT INTO AuctionType(auctionTypeName) VALUES('DESCENDING_BID')
    
    INSERT INTO Variety(varietyName) VALUES('Kohaku')
    INSERT INTO Variety(varietyName) VALUES('Taisho Sanke')
    INSERT INTO Variety(varietyName) VALUES('Showa')
    INSERT INTO Variety(varietyName) VALUES('Shiro Utsuri')
    INSERT INTO Variety(varietyName) VALUES('Utsurimono')
    INSERT INTO Variety(varietyName) VALUES('Beni Kikokuryu')
    INSERT INTO Variety(varietyName) VALUES('Asagi')
    INSERT INTO Variety(varietyName) VALUES('Kikokuryu')
    INSERT INTO Variety(varietyName) VALUES('Hikari Muji')
    INSERT INTO Variety(varietyName) VALUES('Goshiki')
    ````

#### Front-End
- Install library:
    ````bash
    npm install
    ````
- Run project:
    ````bash
    npm run dev
    ````

#### Back-End
- Intellij will automatically install all libraries in the pom.xml file
- Before run project, please unzip [Redis](./Redis-x64-5.0.14.1.zip)
- Run **redis-server.exe** file to run redis server
- Run project by click on play button

##  :camera: Gallery
### Demo
<div align="center">
    <img alt="demo" src="https://github.com/user-attachments/assets/2404cfdf-2f6c-497f-b9d6-dd281017b79a">
</div>

### Manager screen
<div align="center">
    <img alt="demo" src="https://github.com/user-attachments/assets/3844b8ad-5df8-43bd-96a0-81e8d506b0d2">
</div>

### Member screen
<div align="center">
    <img alt="demo" src="https://github.com/user-attachments/assets/e14fd4dd-0308-4e06-a0d6-019f180a696e">
</div>

### Staff screen
<div align="center">
    <img alt="demo" src="https://github.com/user-attachments/assets/c83c1b3e-8093-487d-877e-26dc91ed05e2">
</div>

### Koi Breeder screen
<div align="center">
    <img alt="demo" src="https://github.com/user-attachments/assets/37834407-7296-42f4-9594-76b4bae78b26">
    <img alt="demo" src="https://github.com/user-attachments/assets/3421acf5-cd42-4a04-a0d4-6e4bc63bbd91">
</div>


##  :lock: License
[LICENSE](./LICENSE)
