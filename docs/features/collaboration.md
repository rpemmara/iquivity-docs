# Team Collaboration

Work seamlessly with your team using powerful collaboration features. Available on Professional and Enterprise plans.

## Overview

iQuivity AI's Team Collaboration features enable multiple team members to work together efficiently, share resources, maintain consistency, and streamline workflows across your organization.

!!! note "Plan Availability"
    Team Collaboration features are available on:

    - **Professional Plan** - Up to 5 team members
    - **Enterprise Plan** - Unlimited team members

## Team Management

### Inviting Team Members

Add colleagues to your iQuivity AI workspace.

#### Invitation Process

**1. Access Team Settings**
- Navigate to **Settings** → **Team Management**
- Click **"Invite Member"** button

**2. Enter Member Information**
```
┌─────────────────────────────────────┐
│ Email Address:                      │
│ [teammate@company.com]              │
│                                     │
│ Role: [Select role ▼]              │
│ - Admin                            │
│ - Editor                           │
│ - Viewer                           │
│ - Custom                           │
│                                     │
│ Personal Message (optional):        │
│ [Welcome to the team!]              │
└─────────────────────────────────────┘
```

**3. Assign Role**

Choose the appropriate access level:

| Role | Create | Edit | Delete | Settings | Billing | Invite |
|------|--------|------|--------|----------|---------|--------|
| **Admin** | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ |
| **Editor** | ✅ | ✅ | ✅ | ❌ | ❌ | ❌ |
| **Viewer** | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ |
| **Custom** | Custom permissions | | | | | |

**4. Send Invitation**
- Click **"Send Invite"**
- Email sent to team member
- They receive link to join
- Account creation or login required

**5. Invitation Status**
- **Pending** - Invitation sent, not yet accepted
- **Active** - Team member has joined
- **Expired** - Invitation expired (7 days)
- **Revoked** - Invitation cancelled

!!! tip "Bulk Invitations"
    Invite multiple team members at once by entering multiple email addresses separated by commas or line breaks.

### Team Member Roles

Detailed breakdown of role permissions:

#### Admin Role 👑

**Full Access** to all features and settings:
- Create, edit, delete all content
- Access all team files and workspaces
- Manage team members (invite, remove, change roles)
- Access billing and subscription
- Modify account settings
- View analytics for all team members
- Set up integrations
- Create and manage API keys

**Use For:** Team leaders, project managers, account owners

#### Editor Role ✏️

**Content Creation** and management:
- Create new content (documents, images, videos)
- Edit own content
- Edit shared content (with permission)
- Upload and manage files
- Use templates and create custom templates
- Access shared workspaces
- Comment and collaborate
- View team analytics (limited)

**Cannot:**
- Change account settings
- Manage billing
- Invite or remove team members
- Access private content of others

**Use For:** Content creators, designers, writers, marketers

#### Viewer Role 👁️

**Read-Only Access**:
- View shared content
- Download shared files (if permitted)
- Comment on content (if enabled)
- Use templates
- View own usage statistics

**Cannot:**
- Create or edit content
- Upload files
- Change any settings
- Access private content
- Invite team members

**Use For:** Stakeholders, clients, reviewers, approval managers

#### Custom Role ⚙️

**Tailored Permissions**:

Configure specific access:

```
Content Permissions:
☑ Create documents
☑ Edit own documents
☐ Edit all documents
☑ Delete own documents
☐ Delete all documents

File Permissions:
☑ Upload files
☑ View shared files
☐ Edit shared files
☐ Delete shared files

Feature Access:
☑ AI Writer
☑ AI Images
☐ AI Videos
☑ Chatbots (view only)
☐ Templates (create)

Collaboration:
☑ Add comments
☐ Share externally
☐ Invite team members

Credit Access:
☑ Use team credits
Maximum per month: [100] credits
```

**Use For:** Contractors, part-time staff, specialized roles

### Managing Team Members

#### View Team

**Team Dashboard** displays:
- All team members
- Current roles
- Last active date
- Credit usage
- Content created
- Account status

**Filter and Sort:**
- By role
- By activity
- By credit usage
- By join date

#### Edit Team Member

**Modify Permissions:**
1. Click on team member name
2. Select **"Edit Permissions"**
3. Change role or customize permissions
4. Save changes
5. Member notified of changes

**Update Information:**
- Change role
- Modify custom permissions
- Set credit limits
- Update department/team
- Add notes

#### Set Credit Limits

**Per-User Credit Allocation:**

```
┌─────────────────────────────────────┐
│ Team Member: John Doe               │
│                                     │
│ Monthly Credit Limit:               │
│ ◉ Unlimited                         │
│ ○ Custom: [____] credits           │
│                                     │
│ Current Usage: 145/1000 credits     │
│ ████████░░░░░░░░░░ 14.5%           │
│                                     │
│ ☑ Send alert at 80% usage          │
│ ☑ Block at limit reached            │
└─────────────────────────────────────┘
```

**Benefits:**
- Control costs
- Prevent overuse
- Allocate resources fairly
- Track individual usage

#### Remove Team Members

**Offboarding Process:**

1. **Select Member** to remove
2. Click **"Remove from Team"**
3. **Choose Content Handling:**
   - Transfer ownership to another member
   - Keep in shared workspace
   - Delete all content
4. **Confirm Removal**
5. Member loses access immediately
6. Optional exit survey/feedback

**After Removal:**
- Member cannot access team workspace
- Personal content can be exported (if specified)
- Shared content remains accessible to team
- Credit usage history retained

!!! warning "Content Ownership"
    Always reassign important content before removing a team member to avoid losing work.

## Collaboration Features

### Shared Workspaces

Create dedicated spaces for team collaboration.

#### Creating Shared Workspaces

**1. Create Workspace**
- Go to **Files** → **Workspaces**
- Click **"New Workspace"**
- Name your workspace
- Add description

**2. Configure Workspace**

**Workspace Settings:**
- Name and description
- Default permissions
- Visibility (team-wide or specific members)
- Storage allocation
- Folder structure

**3. Add Members**
- Invite specific team members
- Set per-member permissions
- Assign workspace roles

**4. Organize Content**
- Create folder structure
- Set up templates
- Define workflows
- Establish naming conventions

#### Workspace Permissions

**Workspace-Level Access:**
- **Owner** - Full control
- **Manager** - Manage content and members
- **Contributor** - Add and edit content
- **Viewer** - Read-only access

### Real-Time Collaboration

Work together on documents simultaneously.

#### Collaborative Editing

**Features:**
- **Live Cursors** - See where team members are working
- **Real-Time Updates** - Changes appear instantly
- **Presence Indicators** - Know who's online
- **Change Highlighting** - See recent edits

**Collaboration Tools:**
```
Current Editors:
● John Doe (typing...)
● Jane Smith (viewing)
○ Mike Johnson (offline)
```

**Conflict Prevention:**
- Section locking (optional)
- Edit notifications
- Auto-merge changes
- Version conflict resolution

#### Comments and Feedback

**Add Comments** 💬

**1. Select Text or Element**
- Highlight text in document
- Or click on image/video

**2. Add Comment**
- Click comment icon
- Type your feedback
- @mention team members
- Add priority level

**3. Thread Discussions**
- Reply to comments
- Mark as resolved
- Track conversation history
- Assign action items

**Comment Features:**
```
┌─────────────────────────────────────┐
│ 💬 Jane Smith - 2 hours ago         │
│                                     │
│ This section needs more detail      │
│ about the pricing structure.        │
│                                     │
│ @john Can you add this?             │
│                                     │
│ ↪️ John Doe - 1 hour ago            │
│    Will do! Updated now.            │
│                                     │
│ ✓ Resolved by Jane Smith            │
└─────────────────────────────────────┘
```

**Comment Management:**
- Filter by: Open, Resolved, All
- Sort by: Date, Priority, Author
- Search within comments
- Export comment threads
- Email notifications

#### Version History

**Track All Changes** ⏱️

**View History:**
1. Open document
2. Click **"Version History"**
3. See all versions with:
   - Timestamp
   - Author
   - Changes made
   - File size

**Compare Versions:**
- Side-by-side comparison
- Highlight changes
- See additions/deletions
- Review edit timeline

**Restore Previous Version:**
1. Select version to restore
2. Preview changes
3. Click **"Restore"**
4. Current version saved before restore
5. Or create copy of old version

**Version Management:**
- Auto-save every 30 seconds
- Manual save creates major version
- Keep last 30 days of history (Professional)
- Unlimited history (Enterprise)
- Export version history

### Activity Feed

Stay updated on team activities.

**Activity Dashboard** 📊

View real-time updates:
- New content created
- Files uploaded
- Comments added
- Documents shared
- Templates used
- Workbooks updated
- Team member actions

**Activity Types:**
```
🎨 Sarah created new image "Product Banner"
📝 John edited "Blog Post Draft"
💬 Mike commented on "Q4 Campaign Plan"
📤 Lisa shared "Brand Guidelines" with team
⭐ Tom starred "Social Media Template"
🗑️ Alex deleted "Old Presentation"
```

**Filter Activities:**
- By team member
- By content type
- By date range
- By workspace
- By action type

**Activity Notifications:**
- Real-time notifications
- Email digests (daily/weekly)
- Mention alerts
- Custom notification rules

### Team Templates

Share and standardize templates across your team.

#### Creating Team Templates

**1. Create Template**
- Build custom template
- Test thoroughly
- Document usage

**2. Share with Team**
- Mark as **"Team Template"**
- Set permissions (who can use/edit)
- Add to team library
- Notify team members

**3. Template Management**
- Organize by category
- Add usage instructions
- Track usage statistics
- Update and maintain

#### Template Benefits

**Consistency** 🎯
- Standardized output
- Brand voice alignment
- Quality control
- Professional appearance

**Efficiency** ⚡
- Faster content creation
- Reduced training time
- Proven frameworks
- Best practices encoded

**Collaboration** 🤝
- Shared resources
- Team knowledge base
- Cross-training tool
- Scalable processes

### Team File Library

Centralized file management for teams.

**Shared File Features:**
- Team folders
- Shared tags and labels
- Collaborative organization
- Access control
- Usage analytics

**File Sharing Workflows:**
1. Upload to team folder
2. Tag appropriately
3. Set permissions
4. Notify relevant members
5. Track usage and feedback

## Team Analytics

Monitor team performance and usage.

### Team Dashboard

**Overview Metrics:**
```
╔════════════════════════════════════╗
║ Team Performance (This Month)      ║
╠════════════════════════════════════╣
║ Total Content Created: 247         ║
║ Active Team Members: 8/10          ║
║ Credits Used: 4,250 / 10,000      ║
║ Storage Used: 45 GB / 100 GB      ║
║ Collaboration Score: 92%           ║
╚════════════════════════════════════╝
```

### Individual Analytics

**Per-Member Metrics:**
- Content created
- Credit consumption
- Time active
- Collaboration level
- Quality scores
- Template usage

**Performance Tracking:**
- Set goals and targets
- Monitor progress
- Identify top performers
- Spot bottlenecks
- Optimize workflows

### Usage Reports

**Generate Reports** 📊

**Report Types:**
- Team activity summary
- Credit usage breakdown
- Content production metrics
- Collaboration statistics
- Storage utilization
- Template effectiveness

**Export Options:**
- PDF reports
- CSV data
- Excel spreadsheets
- Scheduled reports (weekly/monthly)

## Best Practices

### Setting Up Your Team

**1. Define Roles Clearly** 👥
- Assign appropriate permissions
- Document role responsibilities
- Set expectations
- Provide training

**2. Establish Workflows** 🔄
- Content creation process
- Review and approval steps
- Quality control checkpoints
- Publishing procedures

**3. Create Guidelines** 📋
- Brand voice and style
- Content standards
- File naming conventions
- Organization structure

**4. Set Up Templates** 📝
- Common content types
- Brand-compliant templates
- Process templates
- Documentation templates

### Optimizing Collaboration

**Communication** 💬
- Use comments effectively
- @mention for urgent items
- Regular team check-ins
- Clear feedback

**Organization** 📁
- Consistent folder structure
- Clear naming conventions
- Proper tagging
- Regular cleanup

**Efficiency** ⚡
- Utilize templates
- Batch similar tasks
- Automate repetitive work
- Share best practices

**Quality** ✨
- Peer review process
- Version control
- Testing procedures
- Continuous improvement

!!! success "Team Success Formula"
    Clear Roles + Good Communication + Shared Resources + Regular Reviews = High-Performing Team

---

**Previous:** [← Templates & Workbooks](templates.md) | **Next:** [Account Profile →](../account/profile.md)
