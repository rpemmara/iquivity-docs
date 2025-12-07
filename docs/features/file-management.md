# File Management

Organize and manage all your files in one centralized workspace. Keep your content organized, accessible, and secure.

## Overview

The File Management system provides a comprehensive solution for storing, organizing, and managing all your iQuivity AI content and uploads. From documents to images, videos to spreadsheets, everything is in one place.

## Uploading Files

### Upload Methods

**1. Drag and Drop** 📁
- Drag files from your computer
- Drop them anywhere in the Files area
- Instant upload starts automatically
- Progress bar shows upload status

**2. Click to Upload** 📤
1. Navigate to **Dashboard** → **Files**
2. Click **"Upload Files"** button
3. Browse and select files from your computer
4. Multiple file selection supported
5. Click **"Open"** to start upload

**3. Bulk Upload** 📦
- Select multiple files at once
- Upload entire folders
- Maintain folder structure
- Faster for many files

!!! tip "Quick Upload"
    Press **⌘/Ctrl + U** from anywhere in the platform to open the upload dialog!

### Supported File Formats

#### Documents 📄
- **PDF** - Portable Document Format
- **DOC/DOCX** - Microsoft Word
- **TXT** - Plain text files
- **RTF** - Rich Text Format
- **ODT** - OpenDocument Text
- **PAGES** - Apple Pages (converted)

#### Images 🖼️
- **JPG/JPEG** - Standard image format
- **PNG** - Lossless image format
- **GIF** - Animated images
- **SVG** - Scalable vector graphics
- **WEBP** - Modern web image format
- **BMP** - Bitmap images
- **TIFF** - High-quality images

#### Spreadsheets 📊
- **XLS/XLSX** - Microsoft Excel
- **CSV** - Comma-separated values
- **ODS** - OpenDocument Spreadsheet
- **NUMBERS** - Apple Numbers (converted)

#### Audio 🎵
- **MP3** - Compressed audio
- **WAV** - Uncompressed audio
- **M4A** - Apple audio format
- **OGG** - Open-source audio
- **FLAC** - Lossless audio

#### Video 🎬
- **MP4** - Standard video format
- **MOV** - Apple video format
- **AVI** - Windows video format
- **WMV** - Windows Media Video
- **MKV** - Matroska video
- **WEBM** - Web video format

#### Other Formats 📚
- **ZIP/RAR** - Compressed archives
- **JSON** - Data format
- **XML** - Markup language
- **EPUB** - E-books
- **MD** - Markdown files

### Upload Limits

File size limits vary by plan:

| Plan | Max File Size | Total Storage |
|------|---------------|---------------|
| **Free** | 25 MB | 1 GB |
| **Starter** | 100 MB | 10 GB |
| **Professional** | 500 MB | 100 GB |
| **Enterprise** | 2 GB | Custom |

!!! warning "Large Files"
    Files over 100 MB may take several minutes to upload. Keep your browser window open until upload completes.

### Upload Status

Monitor uploads in real-time:

```
┌────────────────────────────────────┐
│ Uploading: presentation.pdf        │
│ ████████████░░░░░░ 67%            │
│ 23 MB of 34 MB • 12 seconds left   │
└────────────────────────────────────┘
```

**Upload States:**
- ⏳ **Queued** - Waiting to start
- ⬆️ **Uploading** - Transfer in progress
- ✅ **Processing** - File processing and indexing
- ✓ **Complete** - Ready to use
- ❌ **Failed** - Error occurred (retry available)

## Organizing Files

### Folder Structure

Create a logical folder hierarchy to keep files organized.

#### Creating Folders

1. Navigate to **Files**
2. Click **"New Folder"** button
3. Enter folder name
4. Press **Enter** or click **"Create"**

**Nested Folders:**
```
📁 Marketing
  ├─ 📁 Campaigns
  │   ├─ 📁 2024 Q1
  │   ├─ 📁 2024 Q2
  │   └─ 📁 Social Media
  ├─ 📁 Assets
  │   ├─ 📁 Images
  │   ├─ 📁 Videos
  │   └─ 📁 Templates
  └─ 📁 Reports
```

#### Folder Operations

**Move Folders** 📦
- Drag folder to new location
- Or right-click → **Move to** → Select destination
- All contents move together

**Rename Folders** ✏️
- Right-click folder
- Select **"Rename"**
- Enter new name
- Press **Enter**

**Delete Folders** 🗑️
- Right-click folder
- Select **"Delete"**
- Confirm deletion
- Folder moves to trash (recoverable for 30 days)
- Empty folders can be permanently deleted

**Share Folders** 📤
- Right-click folder
- Select **"Share"**
- Set permissions (view/edit)
- Generate share link or invite team members

!!! note "Folder Permissions"
    On team plans, you can set who can access specific folders. See [Team Collaboration](collaboration.md) for details.

### Tags & Labels

Add metadata to files for easy discovery and organization.

#### Adding Tags

**Method 1: Individual File**
1. Select a file
2. Click **"Add Tag"** in details panel
3. Type tag name
4. Press **Enter**
5. Add multiple tags

**Method 2: Bulk Tagging**
1. Select multiple files (⌘/Ctrl + Click)
2. Right-click selection
3. Choose **"Add Tags"**
4. Enter tags (comma-separated)
5. Apply to all selected

**Tag Examples:**
- 🏷️ Project names: `website-redesign`, `Q4-campaign`
- 🏷️ Content type: `draft`, `final`, `review`
- 🏷️ Status: `published`, `archived`, `in-progress`
- 🏷️ Priority: `urgent`, `important`, `low-priority`
- 🏷️ Client: `acme-corp`, `startup-inc`

#### Creating Labels

Labels are visual markers with colors:

1. Select file
2. Click **"Labels"**
3. Choose color
4. Add label name
5. Apply to file

**Color Coding:**
- 🔴 Red - Urgent/Important
- 🟠 Orange - In Progress
- 🟡 Yellow - Needs Review
- 🟢 Green - Approved/Complete
- 🔵 Blue - Client Work
- 🟣 Purple - Personal Projects

#### Tag Management

**Tag Library** 📚
- View all tags in **Files** → **Tags**
- See file count per tag
- Rename tags (updates all files)
- Merge similar tags
- Delete unused tags

**Auto-Tagging** (Premium) 🤖
- AI suggests tags based on content
- Automatic tag application
- Smart tag recommendations
- Pattern recognition

### Search & Filter

Find files quickly with powerful search tools.

#### Basic Search

**Search Bar** 🔍
- Located at top of Files page
- Type filename or content
- Real-time search results
- Highlights matching text

**Quick Filters:**
```
┌─────────────────────────────┐
│ 📄 All Files                │
│ 📁 Folders Only             │
│ 🖼️ Images                   │
│ 📹 Videos                   │
│ 📄 Documents                │
│ ⭐ Starred                  │
│ 🗑️ Trash                    │
└─────────────────────────────┘
```

#### Advanced Search

Access via **Search** → **Advanced**

**Search Criteria:**

**File Attributes**
- File name contains
- File type equals
- File size (min/max)
- Upload date (range)
- Modified date (range)
- Created by (team member)

**Content Search**
- Full-text search in documents
- Search in file metadata
- Search in comments

**Tags & Labels**
- Has tag
- Has label
- Lacks tag
- Multiple tag combinations

**Example Advanced Search:**
```
Type: Image
Tags: marketing, Q4-2024
Size: > 1MB
Date: Last 30 days
```

#### Sort Options

Sort files by:
- 📅 **Date** (newest/oldest first)
- 📝 **Name** (A-Z or Z-A)
- 📊 **Size** (largest/smallest first)
- ⭐ **Stars** (starred items first)
- 📌 **Priority** (labeled items first)
- 👁️ **Recently viewed**
- ✏️ **Recently modified**

!!! tip "Saved Searches"
    Save frequently used search criteria for quick access. Click **"Save Search"** after building your query.

## File Operations

### Preview Files

View files without downloading:

**Supported Previews:**
- **Documents** - Read PDFs, Word docs, text files
- **Images** - View all image formats
- **Videos** - Play with controls
- **Audio** - Built-in player
- **Code** - Syntax highlighting for code files

**Preview Controls:**
- 🔍 Zoom in/out
- 🖼️ Fullscreen mode
- ⬅️➡️ Navigate between files
- 💬 Add comments
- 📥 Download
- 🔗 Share

### Download Files

**Single File Download** 📥
1. Click file
2. Click **"Download"** button
3. File saves to your device

**Multiple File Download** 📦
1. Select multiple files (⌘/Ctrl + Click)
2. Right-click selection
3. Choose **"Download"**
4. Files download as ZIP archive

**Folder Download** 📁
- Right-click folder
- Select **"Download Folder"**
- Contents packaged as ZIP
- Maintains folder structure

**Keyboard Shortcut:** ⌘/Ctrl + D

### Share Files

Share files with team members or external collaborators.

#### Sharing Methods

**1. Generate Share Link** 🔗

1. Select file
2. Click **"Share"** button
3. Click **"Create Link"**
4. Configure options:
   - **Access level**: View only or Download
   - **Expiration**: Never, 24h, 7 days, 30 days, custom
   - **Password**: Optional password protection
   - **Notify**: Email notification
5. Copy link
6. Share via email, chat, etc.

**Link Options:**
```
🔓 Anyone with link can view
🔒 Password protected
⏰ Expires in 7 days
👁️ View only (no download)
```

**2. Invite Team Members** 👥

1. Select file
2. Click **"Share"**
3. Click **"Invite People"**
4. Enter email addresses
5. Set permissions:
   - **Viewer** - View and download only
   - **Commenter** - View and add comments
   - **Editor** - View, download, and modify
6. Add message (optional)
7. Send invitation

**3. Email Directly** 📧

- Click **"Share via Email"**
- Compose message
- File attached or linked
- Sent from your iQuivity account

#### Share Permissions

| Permission | View | Download | Edit | Delete | Share |
|------------|------|----------|------|--------|-------|
| **Viewer** | ✅ | ✅ | ❌ | ❌ | ❌ |
| **Commenter** | ✅ | ✅ | ❌ | ❌ | ❌ |
| **Editor** | ✅ | ✅ | ✅ | ❌ | ✅ |
| **Owner** | ✅ | ✅ | ✅ | ✅ | ✅ |

#### Managing Shares

View all shared files:
1. Go to **Files** → **Shared**
2. See **"Shared by me"** and **"Shared with me"**
3. Manage individual shares:
   - Revoke access
   - Change permissions
   - Update expiration
   - Disable links

!!! warning "External Sharing"
    Be cautious when sharing files externally. Always set expiration dates and use password protection for sensitive content.

### Delete & Recover Files

**Delete Files** 🗑️
1. Select file(s)
2. Press **Delete** key or right-click → **Delete**
3. File moves to **Trash**
4. Stored for 30 days before permanent deletion

**Trash Management**
- Access via **Files** → **Trash**
- View all deleted items
- See deletion date
- Storage space not freed until emptied

**Recover Files** ♻️
1. Open **Trash**
2. Select file(s) to recover
3. Click **"Restore"**
4. File returns to original location

**Permanent Deletion** 💀
- **Empty Trash** - Deletes all items permanently
- **Delete Forever** - Remove specific items immediately
- ⚠️ **Cannot be undone**

!!! danger "Permanent Deletion"
    Once you empty the trash or permanently delete a file, it cannot be recovered. Use this feature carefully!

### Duplicate Files

**Create Copies** 📄
1. Right-click file
2. Select **"Duplicate"**
3. Copy created with " (Copy)" suffix
4. Edit independently

**Use Cases:**
- Create template variations
- Backup before major edits
- Version control
- A/B testing

### Bulk Actions

Perform operations on multiple files simultaneously.

**Available Bulk Actions:**
- ✅ Select all / Deselect all
- 📁 Move to folder
- 🏷️ Add tags
- 🎨 Apply labels
- 📥 Download as ZIP
- 🗑️ Delete selected
- 📤 Share multiple files
- ⭐ Star/unstar

**Selecting Multiple Files:**
- **⌘/Ctrl + Click** - Add individual files
- **Shift + Click** - Select range
- **⌘/Ctrl + A** - Select all
- **Checkbox** - Select via checkbox

## Storage Management

### Viewing Storage Usage

Access via **Settings** → **Storage**

**Storage Dashboard:**
```
╔════════════════════════════════════╗
║  Storage Usage                     ║
║  ████████████████░░ 82 GB / 100 GB ║
║                                    ║
║  📄 Documents: 24 GB (29%)         ║
║  🖼️ Images: 35 GB (43%)            ║
║  📹 Videos: 20 GB (24%)            ║
║  📦 Other: 3 GB (4%)               ║
╚════════════════════════════════════╝
```

### Managing Storage

**Free Up Space** 💾

1. **Delete Unused Files**
   - Review old files
   - Remove duplicates
   - Archive or delete

2. **Empty Trash** 🗑️
   - Permanently delete trashed items
   - Instant storage recovery

3. **Compress Videos** 🎬
   - Reduce video file sizes
   - Lower resolution if needed
   - Remove source files after compression

4. **Download and Remove** 📥
   - Download important files locally
   - Remove from cloud storage
   - Upload again when needed

5. **Identify Large Files** 📊
   - Sort by size (largest first)
   - Review necessity
   - Delete or compress

**Storage Alerts** 🔔
- **80% full** - Yellow warning
- **90% full** - Orange warning
- **95% full** - Red alert
- Automatic email notifications

### Upgrade Storage

**Need More Space?**
1. Go to **Settings** → **Billing**
2. Click **"Upgrade Plan"**
3. Choose higher tier plan
4. Or purchase additional storage

**Storage Add-Ons:**
- +50 GB: $5/month
- +100 GB: $9/month
- +500 GB: $39/month
- Custom: Contact sales

!!! tip "Storage Best Practices"
    - Regularly review and clean up old files
    - Use external storage for archives
    - Compress large media files
    - Empty trash monthly
    - Monitor storage dashboard

---

**Previous:** [← AI Videos](ai-videos.md) | **Next:** [Templates & Workbooks →](templates.md)
