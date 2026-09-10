## **Module 1: Technical Infrastructure & Crawler Accessibility**

### 

### **1.1 Edge Crawler Configuration (Cloudflare / WAF)**

* **Disable Automated AI Bot Blocking:** Verify that Cloudflare’s default setting *"Block AI bot traffic with robots.txt"* is deactivated across all domains.  
* **Permit Search Agent User-Agents:** Ensure edge Web Application Firewall (WAF) challenge rules (such as Turnstile or interactive JS challenges) do not drop requests or strip semantic HTML headers from verified AI crawler bots.  
* **Robots.txt Standardisation:** Deploy the following standardized allowlist block to robots.txt on all primary domains:

Plaintext  
User-agent: GPTBot  
User-agent: OAI-SearchBot  
User-agent: ClaudeBot  
User-agent: PerplexityBot  
Allow: /

### 

### **1.2 LLM-Optimised Edge Delivery & /llms.txt**

* **Deploy Root /llms.txt Manifest:** Create an /llms.txt plain Markdown endpoint at the root domain detailing service offerings, regional coverage, emergency SLAs, and core RFC/standard compliance.  
* **/llms.txt Reality Check (Google VP Brendan Craham / Edward Sturm Benchmark):** Google Search and Google AI Overviews completely ignore `/llms.txt`. Leading SEO entities (e.g., Ahrefs) do not deploy it, and empirical tests confirm zero ranking or citation impact in Google Search. Deploy `/llms.txt` strictly as a developer manifest for direct third-party LLM API scrapers, never as an active Google AEO/GEO ranking mechanism.  
* **Enable Edge Markdown Content Negotiation:** For dynamic platforms (Cloudflare Workers), serve clean Markdown whenever incoming HTTP headers match Accept: text/markdown, ensuring inline JSON-LD structured schema remains appended in fenced code blocks.  
* **Server-Side Rendering (SSR) Verification:** Verify that directory profiles, price tables, and technical scan engines render in raw HTML/SSR rather than dynamic client-side JavaScript, ensuring headless retrieval scrapers do not encounter empty layout templates.

### **1.3 Elimination of Accidental Cloaking & User-Agent Inconsistencies**

* **Strict Content Parity:** Ensure human visitors, Googlebot, and AI retrieval agents receive identical semantic DOM content.
* **Ban User-Agent Redirects & Stripping:** Disallow edge routing rules or Cloudflare Workers that serve alternate content or strip sections based on incoming User-Agent headers, preventing automated cloaking penalties.

### **1.4 Prohibition of Back-Button Hijacking & Navigation Trapping**

* **Spam Policy Enforcement:** Interfering with standard browser navigation triggers site-wide algorithmic demotions and manual spam actions.
* **Prohibited Navigation Behaviors:**
  * Preventing the browser back button from returning immediately to the referring search engine or prior page.
  * Hijacking the back button history state to redirect users to unvisited commercial landing pages or promotional offers.
  * Triggering unsolicited modal takeovers or interstitial traps on back-navigation intent.

## 
