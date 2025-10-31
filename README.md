# Salesforce Formula Prettifier

A Lightning Web Component tool that helps Salesforce Admins visualize, understand, and evaluate formula fields in a clean, readable format.

## What Does This Tool Do?

Formula fields in Salesforce can become complex and difficult to read, especially when they contain nested functions and long field references. This tool:

- **Prettifies formulas** - Formats your formula fields with proper indentation and syntax highlighting
- **Evaluates results** - Shows you the actual calculated value for a specific record
- **Supports two modes**:
  - **Select Mode**: Choose an object and field from dropdowns
  - **Paste Mode**: Copy and paste any formula directly

## Security & Permissions

This tool respects Salesforce security:
- **Object-Level Security**: You can only see objects you have access to
- **Field-Level Security**: You can only see formula fields you have permission to view

The tool uses Salesforce's built-in security enforcement to ensure you only access data you're authorized to see.

## Installation

Open the [Installation Link](https://linkly.link/2HjLA), login to your org and follow the installation wizard to add this tool to your Salesforce org. Replace 'login.salesforce.com' with 'test.salesforce.com' for sandboxes. 

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
2. Choose **Select Formula Field** mode
3. Select an **Object** from the dropdown
4. Select a **Formula Field** from the dropdown
5. The prettified formula appears automatically

#### Paste Mode
1. Click the **floating action button**
2. Toggle to **Paste** mode
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
- **Hover** over any token to see its details
- **Click on brackets** to highlight matching pairs
- **View field setup** by clicking the setup icon (when in Select mode)

#### Formula Evaluation

When viewing a formula on a record page:
- You will see the **formula evaluation result** and **field values** on hovering over the tokens in the prettified formula.

## Features

✅ Clean, readable formula formatting
✅ Real-time formula evaluation on records
✅ Support for all standard Salesforce formula functions
✅ Object and field-level security enforcement
✅ Works with custom and standard objects
✅ Syntax highlighting for easy reading
✅ Bracket matching for nested functions

## Limitations

- **Trial Period**: This package expires on December 1, 2025
- **Formula Fields Only**: Only works with formula fields, not roll-up summaries
- **Record Context**: Formula evaluation requires being on a record page

## Troubleshooting

### "Package Expired"
The trial version expires on December 1, 2025. Contact support for a license extension.

### Formula Won't Evaluate
Make sure:
- You're on a record page
- The selected object matches the record type you're viewing
- You have access to all fields used in the formula

### No Objects Showing in Dropdown
This means:
- There are no accessible formula fields in your org, OR
- Your user profile doesn't have permission to view any formula fields

## Privacy

This tool:
- Does NOT send data outside your Salesforce org
- Does NOT store any formula or field data
- Operates entirely within Salesforce security boundaries
- Respects all sharing rules and permissions

## Version Information

- **Current Version**: .1.0-1 (Beta package)
- **Expiration**: December 1, 2025

## Credits

Developed with 💜 for the Salesforce Community.
