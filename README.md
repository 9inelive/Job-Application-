# Job-Application-
Automates the job application process using n8n. This workflow tracks job listings, fills forms, sends follow-ups, and organizes application statuses to save time and keep your job search efficient and organized. Easy to customize for different job boards and application steps.

Please leave a like if you enjoy

### **Quick Setup (Required):**

1. **Import the workflow** - Copy the JSON and paste it into n8n
2. **Update Configuration Node** - Change these values in the "📋 Configuration" node:
    - `userName`: Your full name
    - `userEmail`: Your email address
    - `userPhone`: Your phone number
    - `linkedinUrl`: Your LinkedIn profile
    - `location`: Your target job location
    - `excludedTitles`: Job titles to avoid (comma-separated)
    - `excludedKeywords`: Keywords to avoid in descriptions
    - `excludedCompanies`: Companies to blacklist

### **Optional Setup (For Full Features):**

1. **Microsoft Outlook** - Connect your email account for sending applications
2. **Slack Webhook** - Replace `YOUR/SLACK/WEBHOOK` with your webhook URL
3. **Notion Database** - Replace `YOUR_DATABASE_ID` with your Notion database ID

### **What Works Out of the Box:**

- ✅ **Job scraping** from RemoteOK, GitHub Jobs, and Greenhouse
- ✅ **Filtering system** based on your criteria
- ✅ **Job normalization** and deduplication
- ✅ **Personalized application generation**
- ✅ **Manual/Auto application toggle**

### **Key Improvements Made:**

1. **Removed API dependencies** - No need for Adzuna API keys
2. **Simplified configuration** - All settings in one easy node
3. **Better error handling** - Won't crash if APIs are down
4. **Cleaner job sources** - Uses reliable, free APIs
5. **Manual trigger** - Test without waiting for schedule
6. **Visual emoji labels** - Easy to understand workflow

### **Default Behavior:**

- **Auto-apply: OFF** (Safety first - you'll get Slack notifications to review)
- **Runs every 6 hours** automatically
- **Checks for duplicates** using Notion (optional)
- **Generates personalized emails** with relevant tech keywords

### **To Test:**

1. Import the workflow
2. Update the Configuration node with your info
3. Click "Execute Workflow" on the Manual Trigger
4. Check the execution log to see found jobs

The workflow will work immediately after updating the configuration, with full features available once you connect your email and notification services!
