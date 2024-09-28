# ENS I AM DEFI WORKSHOP
### 1. **Introduction to Web3 Domains & Decentralized Hosting**

---

#### **What We’ll Cover:**

##### **ENS (Ethereum Name Service)**:
- **Overview**: The **Ethereum Name Service (ENS)** is often referred to as the "domain name system for Web3." Instead of long, complex Ethereum wallet addresses (e.g., `0xABC123...`), ENS allows users to register human-readable names like `yourname.eth`, which can be mapped to Ethereum addresses or decentralized websites.
- **Launched in**: ENS was launched on **May 4, 2017**, on the Ethereum blockchain.
- **How It Works**: Like the traditional DNS (Domain Name System) that converts `example.com` into a server IP address, ENS does the same but for Web3 resources like cryptocurrency wallets, decentralized websites, or smart contracts. The ENS names can be used to send crypto, interact with dApps, or point to decentralized content.
- **Curious Fact**: ENS names can include not only `.eth` domains but also domains from other naming systems like `.xyz` and `.luxe`. As of September 2023, ENS had registered over **3.5 million domains**, showing its growing adoption in Web3.

##### **Ethereum Basics**:
- **Overview**: **Ethereum** is a decentralized, open-source blockchain with smart contract functionality. Created by **Vitalik Buterin** and launched in **2015**, it was designed to go beyond Bitcoin’s capabilities by supporting complex applications.
- **dApps and Smart Contracts**: Ethereum allows the creation of **decentralized applications (dApps)** through the use of **smart contracts**, self-executing programs that run on the Ethereum blockchain without the need for intermediaries. These smart contracts enable services like ENS, where domain registration, updates, and management are automated and decentralized.
- **Curious Fact**: Ethereum underwent a major upgrade called "The Merge" in **September 2022**, transitioning from a Proof of Work (PoW) consensus mechanism to **Proof of Stake (PoS)**, making the network more energy efficient by reducing its energy consumption by **99.95%**.

##### **IPFS (InterPlanetary File System)**:
- **Overview**: **IPFS** is a peer-to-peer network for storing and sharing data in a decentralized way. Rather than relying on a single server, files on IPFS are distributed across multiple nodes. When you upload a file to IPFS, it’s given a **Content Identifier (CID)**, a unique fingerprint that allows it to be retrieved from any IPFS node.
- **Launched in**: IPFS was developed by **Protocol Labs** and released in **2015**. It aims to decentralize the internet by replacing the traditional HTTP protocol with a content-addressed model.
- **How It Works**: Instead of looking for content at a specific server location (as in traditional web hosting), IPFS fetches content based on its unique CID, regardless of where it is stored. This ensures that content is always accessible as long as at least one node is storing it, making it censorship-resistant and more reliable.
- **Curious Fact**: Unlike traditional web hosting, where you pay for bandwidth and server space, **IPFS uses storage and bandwidth from everyone who participates** in the network. This model aligns with Web3's decentralized philosophy, making it more robust and resistant to censorship.

---

#### **Why It Matters**:

Understanding the basics of **ENS, Ethereum, and IPFS** is crucial because they represent the building blocks of a decentralized internet—**Web3**. The current web (often called Web2) relies on centralized services, meaning the data is stored on servers controlled by companies like Google, Amazon, or Facebook. This has led to concerns about data privacy, censorship, and monopolies over internet services.

With Web3:
- **ENS** provides user-friendly names that make decentralized services more accessible.
- **Ethereum** powers decentralized applications and smart contracts, removing the need for trusted third parties.
- **IPFS** allows you to host websites and content without relying on centralized servers, ensuring greater resilience and accessibility.

These technologies together create a future where you can **own your identity and data**, interact with decentralized apps, and build websites that are **censorship-resistant**, self-hosted on distributed networks, and free from traditional constraints.

---

#### **Sources**:
- [ENS: Decentralizing Naming on Ethereum](https://ens.domains/)
- [Ethereum’s Major Transition to Proof of Stake](https://ethereum.org/en/upgrades/merge/)
- [Protocol Labs and IPFS Overview](https://ipfs.io/)
Here’s a document that explains each part of the HTML and JavaScript code used in the project. This will help you understand the functionality of each element.

---

## **Document Explanation for Code:**

### **1. `<!DOCTYPE html>`**
   - **Explanation**: The `<!DOCTYPE html>` declaration defines the document as an HTML5 document. It tells the browser to interpret the page as an HTML5 document for better compatibility and standardization.

---

### **2. `<html lang="en">`**
   - **Explanation**: The `<html>` element is the root element of an HTML document. The `lang="en"` attribute specifies that the language of the document is English. This helps with accessibility and SEO.

---

### **3. `<head>` Section**
   - **Explanation**: The `<head>` section contains metadata and links to external resources like stylesheets or fonts. The elements inside `<head>` do not display content directly but provide essential information for the document:
     - `<meta charset="UTF-8">`: Specifies the character encoding for the document (UTF-8 is standard and supports all characters).
     - `<meta name="viewport" content="width=device-width, initial-scale=1.0">`: Makes the website responsive by adjusting the width based on the device's screen.
     - `<title>`: Defines the title of the document displayed in the browser tab.
     - `<style>`: Includes internal CSS to style the HTML elements.

---

### **4. `<body>` Section**
   - **Explanation**: The `<body>` element contains the visible content of the webpage. Everything inside the `<body>` is rendered by the browser. This section includes elements like headers, divs, links, buttons, and modals.

---

### **5. `<div class="vcard">`**
   - **Explanation**: The `<div>` element is a block-level container used to group content for styling purposes. In this case, the `class="vcard"` groups the profile information into a card-style layout with the profile image, name, bio, and social media links.
     - `class="vcard"`: Assigns a class name to the div, which is used to apply specific styles from CSS.

---

### **6. `<a href="...">` (Anchor Tag)**
   - **Explanation**: The `<a>` element defines a **hyperlink**, which is used to link to other pages or external resources. 
     - `href="https://twitter.com/yourhandle"`: The `href` attribute specifies the target URL, in this case linking to Twitter.
     - The `<a>` element also acts as a button here when styled using CSS to look like a clickable button with a hover effect.

---

### **7. `<section class="projects">`**
   - **Explanation**: The `<section>` element is used to define a thematic grouping of content. In this example, the "My Projects" section contains multiple project cards. 
     - `class="projects"`: Specifies the class used to apply styles like background, spacing, and layout for the section.

---

### **8. `<div id="donation-modal">`**
   - **Explanation**: This `<div>` defines the **modal**, a pop-up box that contains the donation information. It is hidden by default and only becomes visible when the "Donate" button is clicked.
     - `id="donation-modal"`: The `id` attribute gives a unique identifier to this element, allowing us to control its visibility and behavior using JavaScript.

---

### **9. `<script>` (JavaScript Section)**
   - **Explanation**: The `<script>` element is used to embed or reference JavaScript code. In this document, it is used to control the behavior of the modal (popup). Below is a breakdown of the JavaScript that controls the modal behavior.

---

### **JavaScript Code Breakdown:**
```javascript
const modal = document.getElementById("donation-modal");
```
- **Explanation**: This line creates a constant variable `modal` and assigns it to the HTML element with the `id="donation-modal"`. This allows us to control the modal’s behavior (e.g., opening and closing it) using JavaScript.

```javascript
const btn = document.getElementById("donate-btn");
```
- **Explanation**: This line creates a constant `btn` that selects the **Donate** button with the `id="donate-btn"`. When the button is clicked, it triggers the modal to open.

```javascript
const span = document.getElementsByClassName("close")[0];
```
- **Explanation**: This line selects the **close button (X)** within the modal by targeting the first element with the class name `"close"`. This is used to close the modal when the user clicks the X button.

```javascript
btn.onclick = function() {
    modal.style.display = "block";
}
```
- **Explanation**: This function is executed when the **Donate** button is clicked. It changes the `display` style of the modal to `"block"`, which makes the modal visible.

```javascript
span.onclick = function() {
    modal.style.display = "none";
}
```
- **Explanation**: This function is executed when the **close button (X)** inside the modal is clicked. It sets the modal’s display style to `"none"`, which hides the modal.

```javascript
window.onclick = function(event) {
    if (event.target == modal) {
        modal.style.display = "none";
    }
}
```
- **Explanation**: This function checks if the user clicks anywhere outside the modal. If they do, it closes the modal by setting the `display` to `"none"`. The condition `if (event.target == modal)` ensures that the modal only closes if the background overlay is clicked.



