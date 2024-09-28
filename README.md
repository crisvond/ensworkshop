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
### ** How to Create a GitHub Account, Create a New Repository, and Add an HTML File**

This guide will walk you through the steps to create a **GitHub account**, set up a **new repository**, and **add an HTML file** to the repository. This process will be useful when integrating GitHub with platforms like **Fleek** for hosting.

---

### **Step 1: Create a GitHub Account**

1. **Go to GitHub’s Website**:
   - Visit [https://github.com](https://github.com).

2. **Sign Up**:
   - Click the **"Sign Up"** button.
   - Enter your email address, create a username, and choose a password.
   - GitHub may ask you to solve a puzzle to verify that you are human.

3. **Set Preferences**:
   - Choose whether you'd like to receive updates from GitHub.
   - Select the **free account** option, which gives you access to all necessary features.

4. **Email Verification**:
   - After signing up, GitHub will send you an email for verification.
   - Open the email, click the verification link, and log in.

---

### **Step 2: Create a New GitHub Repository**

1. **Go to Your GitHub Dashboard**:
   - Once logged in, click on your profile icon in the top right, and select **"Your Repositories"** from the dropdown menu.

2. **Create a New Repository**:
   - On the **"Your Repositories"** page, click the green **"New"** button.

3. **Fill in Repository Details**:
   - **Repository Name**: Enter a name for your repository (e.g., `my-website`).
   - **Description** (Optional): You can add a brief description of the repository.
   - **Public or Private**: Choose whether you want the repository to be public or private.
   - **Initialize the repository with a README**: Check this box if you want GitHub to create a README file automatically (optional).

4. **Click "Create Repository"**:
   - Once all fields are filled, click **"Create Repository"**.

---

### **Step 3: Add an HTML File Manually to the Repository**

1. **Go to Your Repository**:
   - After creating the repository, you will be directed to your repository's page (e.g., `https://github.com/username/my-website`).

2. **Add a New File**:
   - On your repository page, click the **"Add file"** dropdown button and select **"Create new file"**.

3. **Name Your HTML File**:
   - In the input field that appears, type the name for your file (e.g., `index.html`). 
     - `index.html` is typically the main file for a website.

4. **Add Your HTML Code**:
   - In the large text editor below, manually add your HTML code. For example, here’s a simple HTML template:

   ```html
   <!DOCTYPE html>
   <html lang="en">
   <head>
       <meta charset="UTF-8">
       <meta name="viewport" content="width=device-width, initial-scale=1.0">
       <title>My Website</title>
   </head>
   <body>
       <h1>Welcome to My Website!</h1>
       <p>This is my first website hosted on GitHub.</p>
   </body>
   </html>
   ```

5. **Commit the New File**:
   - Scroll down to the **"Commit new file"** section.
   - In the first field, write a brief description of the file (e.g., `Add index.html`).
   - Make sure **"Commit directly to the main branch"** is selected.

6. **Click "Commit New File"**:
   - Click the green **"Commit new file"** button to save your file into the repository.

---

### **Step 4: Connect Your GitHub Repository to Fleek**

1. **Log into Fleek**
2. **Create a New Site**:
   - Click the **"Create New Site"** button and select **GitHub** as the source.
3. **Authorize Fleek**:
   - Authorize Fleek to access your GitHub account.
4. **Select Your Repository**:
   - Choose the newly created repository (e.g., `my-website`) to deploy it to Fleek.

---

### **Conclusion**:
You have now successfully created a GitHub account, set up a new repository, added an HTML file manually, and are ready to connect it to Fleek for hosting.

---

## **Using Fleek for Domain and ENS Integration**

This document will guide you through the process of adding a **domain** or **ENS** (Ethereum Name Service) to your Fleek-hosted website. Fleek offers a user-friendly platform to manage both traditional DNS domains and decentralized ENS domains, ensuring your content is easily accessible to your users.

---

### **What is Fleek?**
Fleek is a Web3 hosting platform that makes it simple to host websites and applications on decentralized networks like IPFS (InterPlanetary File System). It also supports both traditional DNS domains and **ENS domains**—a decentralized alternative to DNS that resolves `.eth` domains on the Ethereum network.

### **Domains on Fleek**

#### **1. ENS Domains on Fleek**
An **ENS domain** (`.eth`) is a decentralized, Ethereum-based alternative to DNS. With ENS, you can map various records (IPFS hashes, websites, wallet addresses) to your `.eth` domain. For instance, a site hosted on IPFS can be mapped to `yourens.eth`, making it accessible to users who can resolve ENS domains.

##### **How ENS Resolution Works**
For an ENS domain to resolve, users need a compatible browser or extension (e.g., **MetaMask**), or they can use public gateways like **ETH Limo**. By appending `.limo` to your ENS domain (`yourens.eth.limo`), the ENS name is resolved via a regular HTTPS request.

---

### **Step-by-Step Guide: Adding an ENS Domain on Fleek**

#### **Step 1: Create a Site on Fleek**
Before you can add a domain, you need to have a site deployed on Fleek. Follow these steps:
1. Log into Fleek https://fleek.xyz/.
2. Click **"Create New Site"** and follow the instructions to upload your HTML files (via GitHub).
3. Once deployed, go to your site’s **Site Overview** page.

#### **Step 2: Add Your ENS Domain**
1. Navigate to the **Settings** section of your site on Fleek.
2. Go to the **Domains** tab.
3. Under the **ENS Domains** section, enter your ENS domain (e.g., `yourens.eth`) and click **Add ENS Domain**.
   - Fleek will validate the domain to ensure it’s not already added to another site.
4. Once validated, choose how to set the ENS **content hash**—this is where you map the ENS domain to the IPFS content.

---

### **Step 3: Setting the ENS Content Hash**

##### **Option 1: Automatic ENS Configuration (Recommended)**
1. **Automatic Configuration**: Fleek automatically manages the ENS configuration by interacting with your Ethereum wallet.
2. Choose between **IPFS** or **IPNS** as the content hash record:
   - **IPFS**: If the site won’t be updated often (requires gas fees for updates).
   - **IPNS**: Ideal for frequently updated sites (does not require gas fees for updates).
3. Fleek will ask you to sign the transaction to set the content hash.
4. Once configured, your ENS domain will be live, and your site will be accessible via gateways like `yourens.eth.limo`.

**Note**: You need access to the wallet that owns the ENS record to use automatic configuration.

##### **Option 2: Manual ENS Configuration**
If you prefer to manually manage the ENS record (or don’t have access to the wallet controlling the ENS), follow these steps:
1. In Fleek, choose the **manual option** to copy the content hash.
2. Visit the [ENS Manager](https://app.ens.domains/) and set the content hash:
   - Choose **IPFS** or **IPNS**, and copy the corresponding content hash from Fleek.
   - In the **Content** field on the ENS Manager, paste the content hash.
   - Confirm and complete the Ethereum transaction to set the hash.

After completing the manual setup, return to Fleek and click **"OK! I have added it"** to verify the configuration.

---

### **Step 4: Access Your Site via ENS**
Once your ENS domain is configured, your site can be accessed using:
- **ENS-enabled browsers or extensions**: E.g., `yourens.eth` (resolved by MetaMask or ENS-compatible browsers).
- **Public Gateways**: E.g., `yourens.eth.limo` (HTTPS resolution using ETH Limo).

---

### **Traditional DNS Domain Setup on Fleek**

Fleek also supports traditional **DNS domains**. To set up a custom DNS domain, follow these steps:

#### **Step 1: Add a Custom Domain**
1. On your site’s **Site Overview** page, go to **Settings** > **Domains**.
2. Enter your **custom domain** (e.g., `yourdomain.com`), and Fleek will validate the domain.
3. Fleek will generate a **pull zone URL** for your site, which serves as a link between the content on IPFS and the custom domain.

#### **Step 2: Configure Your DNS**
1. Go to your **DNS provider** and add a **CNAME** or **ANAME** record to point your domain to the pull zone URL.
2. Once set, return to Fleek and click **"OK! I have added it"** to trigger the validation process.

#### **Step 3: Domain Activation**
After Fleek validates your DNS settings, your custom domain will be marked as **Active**, and your site will be accessible via the custom domain. Fleek automatically updates the DNS when you deploy new content.

---

### **DNSLink Configuration**
**DNSLink** allows you to map your domain to the most recent IPFS content automatically. To set up DNSLink:
1. After linking a custom domain to your site, go to the **DNSLink** section in the Fleek dashboard.
2. Follow the steps to configure DNSLink with your DNS provider.
3. Once DNSLink is active, your domain will always point to the latest version of your site on IPFS.

---

### **Conclusion**

By using Fleek, setting up both **ENS domains** and **custom DNS domains** becomes straightforward, ensuring that your website is decentralized, resilient, and always accessible. Whether you choose ENS for a fully decentralized experience or traditional DNS, Fleek provides seamless management of your domains, making it easier than ever to deploy Web3 websites.

Feel free to explore Fleek’s platform and leverage its tools to make your decentralized website more robust and secure.
- **Explanation**: This function checks if the user clicks anywhere outside the modal. If they do, it closes the modal by setting the `display` to `"none"`. The condition `if (event.target == modal)` ensures that the modal only closes if the background overlay is clicked.
### **Extra Documentation: Enhancing Your Website with Web3 Tools and Metadata**

As we move into the world of Web3, it’s important to know how to integrate **Web3 tools** and optimize your website with additional tags and metadata. Below is a guide to adding **Web3 scripts**, **extra HTML metadata**, and how to embed additional content like videos or widgets.

---

### **1. Adding Web3 Integration Scripts**

To interact with **Web3 wallets** like **MetaMask** or connect with the **Ethereum blockchain**, you need to include specific JavaScript libraries. The most common Web3 libraries are **Web3.js** and **Ethers.js**.

#### **Including Web3.js or Ethers.js in Your Project**

- **Web3.js** is used to interact with Ethereum’s blockchain and decentralized applications (dApps). Here’s how to add the Web3.js library:

```html
<!-- Include Web3.js -->
<script src="https://cdn.jsdelivr.net/npm/web3@latest/dist/web3.min.js"></script>
```

- **Ethers.js** is another library often used in Web3 projects to interact with Ethereum and other blockchains:

```html
<!-- Include Ethers.js -->
<script src="https://cdn.ethers.io/lib/ethers-5.2.umd.min.js"></script>
```

#### **Example Script to Connect to MetaMask**

If you want to interact with **MetaMask**, you can include the following JavaScript code in your file:

```html
<script>
    // Check if MetaMask is installed
    if (typeof window.ethereum !== 'undefined') {
        console.log('MetaMask is installed!');

        // Connect to MetaMask
        ethereum.request({ method: 'eth_requestAccounts' })
            .then(accounts => {
                console.log(`Connected with account: ${accounts[0]}`);
            })
            .catch(error => {
                console.error('Error connecting to MetaMask:', error);
            });
    } else {
        console.log('MetaMask is not installed!');
    }
</script>
```

This code checks if MetaMask is installed, and if so, it requests permission to connect to the user's Ethereum account.

---

### **2. Adding HTML Metadata**

Metadata provides essential information about your website, such as its title, description, and keywords. Adding proper metadata helps improve your site’s SEO (Search Engine Optimization) and the way it appears when shared on social media platforms.

#### **Basic Meta Tags for SEO**

- **Title**: Defines the title of your page, which appears in the browser tab and search results.
  
```html
<title>My Web3 Website</title>
```

- **Meta Description**: Provides a short description of your page for search engines and when the link is shared on social media.

```html
<meta name="description" content="A decentralized website built using Web3 tools, hosted on IPFS. Learn how to create your own Web3 site.">
```

- **Meta Keywords**: Specifies keywords relevant to your website, which can help with SEO.

```html
<meta name="keywords" content="Web3, IPFS, decentralized website, ENS, blockchain, MetaMask">
```

---

### **3. Open Graph Tags for Social Media Sharing**

If you want your website to look professional when shared on platforms like Facebook, Twitter, or LinkedIn, use **Open Graph (OG) tags**. These tags control how your content appears on social media.

```html
<!-- Open Graph Meta Tags -->
<meta property="og:title" content="My Web3 Website">
<meta property="og:description" content="A decentralized website built with Web3 tools and hosted on IPFS.">
<meta property="og:image" content="https://mywebsite.com/path/to/preview-image.jpg">
<meta property="og:url" content="https://mywebsite.com">
<meta property="og:type" content="website">
```

---

### **4. Embedding External Content**

You can add interactive and multimedia content to your Web3 website by embedding videos, widgets, or live Web3 data from the blockchain.

#### **Embedding a YouTube Video**

If you want to embed a YouTube video on your site, you can use the following `<iframe>` tag:

```html
<iframe width="560" height="315" src="https://www.youtube.com/embed/video_id" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
```

Replace `"video_id"` with the ID of the YouTube video you want to embed.

#### **Embedding a Twitter Widget**

If you want to embed a Twitter feed or a specific tweet:

```html
<a class="twitter-timeline" href="https://twitter.com/YourHandle?ref_src=twsrc%5Etfw">Tweets by YourHandle</a>
<script async src="https://platform.twitter.com/widgets.js" charset="utf-8"></script>
```

This will display your Twitter feed on your website.

---

### **5. Using Web3-Specific Metadata**

If your site interacts with Web3 technologies like **dApps** or **wallets**, it’s good to include **EIP-1102** support to ensure browsers and wallets can recognize your site as Web3-enabled. This can be done by adding a `web3` property in the `<head>`.

```html
<meta name="web3-site" content="yes">
```

This is a way to inform browsers and extensions that your site interacts with Web3 technologies like Ethereum, improving compatibility with dApps.

---

### **6. Example Full Header with All Metadata and Scripts**

Here’s a complete example of what your `<head>` section might look like when you include Web3 scripts, metadata, and social media tags:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Web3 Website</title>

    <!-- Meta Description -->
    <meta name="description" content="A decentralized website built using Web3 tools, hosted on IPFS. Learn how to create your own Web3 site.">
    
    <!-- Meta Keywords -->
    <meta name="keywords" content="Web3, IPFS, decentralized website, ENS, blockchain, MetaMask">
    
    <!-- Open Graph Meta Tags for Social Media -->
    <meta property="og:title" content="My Web3 Website">
    <meta property="og:description" content="A decentralized website built with Web3 tools and hosted on IPFS.">
    <meta property="og:image" content="https://mywebsite.com/path/to/preview-image.jpg">
    <meta property="og:url" content="https://mywebsite.com">
    <meta property="og:type" content="website">
    
    <!-- Web3 Compatibility -->
    <meta name="web3-site" content="yes">

    <!-- Include Web3.js -->
    <script src="https://cdn.jsdelivr.net/npm/web3@latest/dist/web3.min.js"></script>

    <!-- Include Ethers.js -->
    <script src="https://cdn.ethers.io/lib/ethers-5.2.umd.min.js"></script>

    <!-- MetaMask Connection Script -->
    <script>
        if (typeof window.ethereum !== 'undefined') {
            ethereum.request({ method: 'eth_requestAccounts' })
                .then(accounts => {
                    console.log(`Connected with account: ${accounts[0]}`);
                })
                .catch(error => {
                    console.error('Error connecting to MetaMask:', error);
                });
        } else {
            console.log('MetaMask is not installed!');
        }
    </script>
</head>
<body>
    <!-- Your website content here -->
</body>
</html>
```

---

### **Conclusion**

By including the necessary **Web3 scripts** like **Web3.js** or **Ethers.js**, adding relevant **metadata** for SEO and social sharing, and using modern web tools to enhance your site, you can make your decentralized website more interactive and accessible.

Feel free to experiment with adding more Web3 functionality, such as integrating dApp interactions or displaying real-time blockchain data!


