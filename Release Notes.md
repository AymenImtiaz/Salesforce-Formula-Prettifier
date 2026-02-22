# Release Notes

## Version 0.3.0 (February 2026)

### New Features

**Refresh Button**
- Added a refresh button to re-prettify and re-evaluate formulas without having to change your selections.
- Useful when you want to see updated field values or re-run the evaluation after record changes

**Enhanced Formula Evaluation Feedback**
- Added contextual help next to "Result" to provide guidance on common reasons for evaluation failures:
  - Incorrect record page context
  - Missing field-level access permissions
  - "Treat blank fields as" setting is not configured correctly

---

## Version 0.2.0 (February 2026)

### New Features

**Treat Blank Fields As Setting**
- Added support for the "Treat blank fields as" formula setting
- Enables real-time comparison between "Blanks" and "Zeroes" behavior
- Reflects how Salesforce evaluates numeric/currency/percent fields when they're blank
- Defaults to "Zeroes" to match Salesforce's standard default behavior

### Technical Notes
Due to Salesforce API limitations, the "Treat blank fields as" setting cannot be directly retrieved from the FieldDefinition object. The tool provides this configuration manually, allowing you to match the field's actual setting and see accurate evaluation results.

---

## Version 0.1.0 (December 2025)

### Initial Release

**Core Formula Prettification**
- Clean, readable formatting with proper indentation
- Syntax highlighting for functions, fields, strings, numbers, operators, and punctuation
- Support for all standard Salesforce formula functions
- Collapsible logic blocks for easy navigation of complex formulas

**Two Operating Modes**
- **Select Mode**: Choose object and formula field from dropdowns
- **Paste Mode**: Copy and paste any formula text directly

**Real-Time Formula Evaluation**
- Evaluates formulas against actual record data
- Displays field values on token hover
- Shows formula result in real-time
- Respects object-level and field-level security

**Interactive Features**
- Bracket matching for nested functions
- Click-to-highlight matching parentheses
- Direct link to field setup (Select mode)
- Copy formatted formula to clipboard

**Security & Privacy**
- 100% Salesforce-native solution
- Respects all object and field permissions
- No data leaves your Salesforce org
- Operates within Salesforce security boundaries

**User Experience**
- Floating action button for easy access
- Resizable, draggable window
- Toggle between Select and Paste modes seamlessly
- Works across standard and custom objects
