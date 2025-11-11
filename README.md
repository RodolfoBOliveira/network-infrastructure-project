# 🌐 LAN Network Infrastructure Plan

This repository contains the project materials developed for the **Structured Cabling** course unit (2024/2025) at the Coimbra Institute of Engineering (ISEC).

The primary goal was to plan a modern, robust, and scalable LAN network infrastructure for the **Dr. Joaquim Gomes Ferreira Alves Secondary School**, based on a structured cabling system compliant with the ISO/IEC 11801 standard.

---

## 🎯 Project Objective

The objective was to design a complete network infrastructure capable of overcoming common challenges found in many educational institutions, such as:

* Unstructured or non-standardized networks.
* Use of obsolete equipment.
* Incomplete or non-existent Wi-Fi coverage.
* Lack of network segmentation (VLANs) and appropriate security mechanisms.

The proposed design aims to create a secure, high-performance, and converged network focused on:
* **Convergence:** Supporting data (Ethernet), voice (VoIP), and wireless access (Wi-Fi) on a single infrastructure.
* **High Performance & Longevity:** Ensuring capacity for future technologies by adopting Category 6A and OM4 fiber optics.
* **Security & Segmentation:** Isolating traffic from different groups (students, teachers, administration, visitors) using VLANs.
* **Standardization:** Strictly following international standards ISO/IEC 11801 (design) and ANSI/TIA-606-C (labeling).

---

## 🏗️ Network Architecture

The school's infrastructure is physically distributed across four main buildings: Pavilion A, Pavilion B, Pavilion C, and the Canteen/Bar/Bookstore building.

The adopted network topology follows a **hierarchical star model**, as recommended by the ISO/IEC 11801 standard. 

<img width="1239" height="1149" alt="image" src="https://github.com/user-attachments/assets/308d1467-07b3-4ed9-b147-2add0fbb6d69" />


* **Core:** The **Campus Distributor (CD / MDF)**, the central core of the network, is strategically located on Floor 0 of Pavilion B.
* **Distribution (Backbone):**
    * Each of the other buildings (Pavilion A, Pavilion C, and Canteen) has a **Building Distributor (BDF)** on its respective Floor 0.
    * The campus backbone (connecting the MDF to the BDFs) is implemented with **multimode OM4 fiber optic cable**.
* **Access (Horizontal):**
    * In multi-story buildings (A, B, C), there are **Floor Distributors (FDs / IDFs)** on each floor to serve the work areas.
    * The vertical backbone (connecting BDFs to IDFs) also uses OM4 fiber optics.
    * The horizontal cabling (connecting IDFs to user outlets - TOs) is fully implemented with **Category 6A (Cat6A)** cable.

---

## 🔌 Services and Components

### Services to be Provided

The infrastructure is designed to support all essential services for the school's operation:

* **School Management:** Systems for managing student data, schedules, and grades.
* **Education:** E-learning platforms, access to multimedia content, and educational resources.
* **Communication:** Voice over IP (VoIP) services and institutional email.
* **Internal Resources:** Intranet portal, file servers, centralized authentication, and printing services.
* **Connectivity:** Internet access and cloud-based platforms.
* **Wireless Network:** Full Wi-Fi coverage in all buildings, with segmented networks for students, staff, and visitors.

### Network Components

The solution integrates active and passive equipment to build the infrastructure:

* **Active Equipment:** Includes devices that manage network traffic, such as Routers/Firewalls, Switches (core and access), Access Points (APs), Servers, and VoIP phones.
* **Passive Equipment:** Forms the physical foundation of the network, including Network Cables (Cat6A and OM4 Fiber), Patch Panels, Telecommunications Outlets, Racks, and cable trays.

---

## 📋 Key Standards and Materials

The selection of materials was a cornerstone of the project to ensure performance and longevity.

* **Horizontal Cabling:** **Category 6A (Cat6A)** was selected. This choice supports **10 Gigabits per second (10 Gbps)** transmissions over channels up to 100 meters, ensuring the network is prepared for future generations of Wi-Fi APs and high-bandwidth applications (e.g., streaming, VR).
* **Backbone (Campus and Vertical):** **Multimode OM4 Fiber Optic** cable was chosen. This fiber offers very high bandwidth (supporting 10 Gbps up to 550 meters and future 40/100 Gbps upgrades) and, crucially, is **completely immune to electromagnetic interference (EMI)**.
* **Labeling:** To ensure proper network management and maintenance, a clear and consistent labeling system based on the **ANSI/TIA-606-C** standard will be implemented.
* **Labeling Format:** The adopted format will be `DE-DP.PP-XX`.
    * **DE:** Building Distributor identifier (e.g., A, B, C, CNT).
    * **DP:** Floor Distributor identifier (e.g., P0, P1).
    * **PP:** Patch Panel identifier in the rack (e.g., PA, PB).
    * **XX:** Port number on the Patch Panel (e.g., 01, 02, ..., 24).

---

## 🛠️ Technologies and Tools

* **Reference Standards:** ISO/IEC 11801 (Design), ANSI/TIA-606-C (Labeling)
* **Simulation and Design Software:** Cisco Packet Tracer (used for coverage and topology maps)
* **Cabling:** Category 6A (Cat6A), Multimode OM4 Fiber Optic
* **Equipment (Budget Examples):**
    * **Router/Firewall:** Fortinet FortiGate 400E
    * **Switches:** D-link Smart Managed Switch (10G), Ubiquiti USW-24-POE
    * **Access Points:** Huawei AirEngine 5761-11
    * **WLAN Controller:** Cisco AIR-CT3504-K9
    * **Servers:** Dell PowerEdge R760
    * **IP Phones:** Huawei eSpace 6805
    * **UPS:** APC Smart-UPS SRT 1000VA
    * **Racks:** Digitus 600X6

---

## 📁 Repository Contents

* `Network_Infrastructure_Technical_Report.pdf`: The final, detailed technical report for the project. It includes requirements analysis, topology design, materials justification, the labeling scheme, and a detailed budget.
* `Network_Infrastructure_Presentation.pptx`: The slides used for the project presentation. It contains a visual summary of building layouts, services, materials, and maps for cabling distribution and wireless coverage.
* `Project_Budget.xlsx`: A spreadsheet file containing the detailed project budget, equipment list, quantities, and cost estimates.

---

## 👤 Authors

* Henrique Dias Neves Simões Ferreira
* João Pedro Vila Pomar
* José Pedro Leal Neto
* Rodolfo Miguel de Sousa Belchior Brás Oliveira
