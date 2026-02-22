# Salesforce Formula Prettifier

A Lightning Web Component tool that helps Salesforce Admins visualize, understand, and evaluate formula fields in a clean, readable format.

## What Does This Tool Do?

Formula fields in Salesforce can become complex and difficult to read, especially when they contain nested functions and long field references. This tool:

- **Prettifies formulas** - Formats your formula fields with proper indentation and syntax highlighting
- **Evaluates results** - Shows you the actual calculated value for a specific record
- **Supports two modes**:
  - **Select Mode**: Choose an object and field from dropdowns
  - **Paste Mode**: Copy and paste any formula directly

## What's New

📋 **[View Release Notes](/Release%20Notes.md)** for detailed information about features and improvements in each version.

**Latest (v0.3.0):** Refresh button, enhanced evaluation feedback with contextual help, and UI improvements.

## Security & Permissions

This tool respects Salesforce security:
- **Object-Level Security**: You can only see objects you have access to
- **Field-Level Security**: You can only see formula fields you have permission to view

The tool uses Salesforce's built-in security enforcement to ensure you only access data you're authorized to see.

## Installation

This app can be installed directly from the [AppExchange](https://appexchange.salesforce.com/appxListingDetail?listingId=6c82b00e-c028-43dc-b678-9f7c864dbde9)

## How to Use

### Adding to a Lightning Page

1. Navigate to any Lightning record page (Account, Contact, Opportunity, etc.)
2. Click the **Setup gear** → **Edit Page**
3. Find **Salesforce Formula Prettifier** in the component list
4. Drag it anywhere onto your page layout (it will always appear in the bottom right corner of the page)
5. Click **Save** and **Activate**

### Using the Tool

#### Select Mode (Default)
1. Click the **floating action button** on your record page
2. Select an **Object** from the dropdown
3. Select a **Formula Field** from the dropdown
4. The prettified formula appears automatically

#### Paste Mode
1. Toggle to **Paste** mode
3. Paste your formula into the text area
4. Click **Prettify Formula**
5. View the formatted result

### Understanding the Display

**Syntax Highlighting:**
- **Purple**: Functions (IF, AND, OR, TEXT, etc.)
- **Light Blue**: Field references (Account.Name, Owner.Email)
- **Green**: String values ("text in quotes")
- **Indigo**: Numbers (1, 100, 0.5)
- **Red**: Operators
- **Yellow**: Punctuation

**Interactive Features:**
- **Hover** over any token to see its value
- **Click on brackets** to highlight matching pairs
- **View field setup** by clicking the setup icon (when in Select mode)

#### Formula Evaluation

When viewing a formula on a record page:
- You will see the **formula evaluation result** and **field values** on hovering over the tokens in the prettified formula.

## Features

- ✨ Clean, readable formula formatting
- 🧠 Real-time formula and field evaluation on records
- 🔐 Security-aware evaluation
- 🔎 Bracket matching for nested functions
- 🎯 Supports all standard Salesforce formula functions
- 🧩 Works across standard & custom objects
- 📂 Collapsible logic blocks for easy navigation
- ☁️ 100% Salesforce-native solution

## Limitations

- **Formula Fields Only**: Only works with formula fields, not roll-up summaries
- **Record Context**: Formula evaluation requires being on a record page

## Troubleshooting

### Unable to evaluate formula
Make sure:
- You're on the right record page
- You have access to all fields used in the formula

### No objects showing in the dropdown
This means:
- Your user doesn't have permission to view any formula fields

### Evaluation Result is not as expected
Formula is evaluated considering the 'Treat blank fields as' setting configured in the prettifier window. If you think the result is not as expected, make sure that setting is configured correctly.

## Privacy

This tool:
- Does NOT send data outside your Salesforce org
- Does NOT store any formula or field data
- Operates entirely within Salesforce security boundaries
- Respects all sharing rules and permissions

## Credits

Designed and developed by [Aymen Imtiaz](https://www.linkedin.com/in/aymen-imtiaz-salesforce-developer/) with 💜 for the Salesforce Community.
