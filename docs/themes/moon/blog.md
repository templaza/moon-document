
---

# Blog Settings

**Location:**
`Site administration → Appearance → Blog`

This page allows administrators to control how the blog feature works across the entire site, including visibility, external blog integration, and comment management.
You can also refer to the Moodle Blog Documentation: [Moodle Blog](https://docs.moodle.org/500/en/Blogs) 
---

# 1. Enable Blog Associations

### Setting: **Enable blog associations**

**Purpose:**
Allows blog posts to be linked (associated) with:

* Courses
* Course activities (modules)

**When enabled:**

* Users can connect their blog posts to specific courses or activities.
* Blog entries may appear in course contexts.

**When disabled:**

* Blog posts cannot be linked to courses or activities.

**Recommended:**
Keep enabled if your LMS uses blogs for learning reflections or course-based discussions.

---

# 2. Blog Visibility

### Setting: **Blog visibility**

**Purpose:**
Controls who can view blog entries across the platform.

This setting defines the **maximum visibility level for viewers**, not for authors.

Typical options include:

* The world can read entries set to be world-accessible
* All site users can see all blog entries
* Only logged-in users can view blogs
* Disable blogs completely

**Important:**
This controls viewing permissions globally. Individual blog privacy settings still apply within this limit.

**Recommended:**

* For internal LMS: “All site users”
* For public sites: “The world can read world-accessible entries”

---

# 3. Enable External Blogs

### Setting: **Enable external blogs**

**Purpose:**
Allows users to connect external blog feeds (RSS/Atom) to their Moodle blog.

**When enabled:**

* Users can register external blog URLs.
* Moodle automatically imports new entries.

**When disabled:**

* Users cannot link external blogs.

**Use case:**
Helpful when instructors or students maintain blogs outside the LMS and want automatic synchronization.

---

# 4. External Blog Cron Schedule

### Setting: **External blog cron schedule**

**Purpose:**
Defines how often Moodle checks external blog feeds for new entries.

**Options:**

* Every hour
* Every 12 hours
* Every 24 hours (default)

**Important:**
This depends on the system cron job being configured correctly.

**Recommendation:**

* 24 hours for normal usage
* 1–12 hours if frequent updates are required

---

# 5. Maximum Number of External Blogs per User

### Setting: **Maximum number of external blogs per user**

**Default:** 1

**Purpose:**
Limits how many external blog feeds a user can connect.

**Example:**
If set to 3, each user may register up to 3 external blog URLs.

**Recommendation:**
Keep low (1–2) to avoid performance issues and excessive feed checks.

---

# 6. Enable Comments

### Setting: **Enable comments**

**Purpose:**
Allows users to comment on blog posts.

**When enabled:**

* Blog entries support discussion.
* Users can reply and interact.

**When disabled:**

* Blogs become read-only.
* No interaction is possible.

**Recommended:**
Enable for collaborative learning environments.

---

# 7. Show Comments Count

### Setting: **Show comments count**

**Purpose:**
Displays the number of comments next to blog posts (Default: Yes)

**Note:**
This requires an additional database query when displaying blog listings.

**Performance Consideration:**
On very large sites, disabling this may slightly improve performance.

---

# 8. Saving Changes

After modifying settings:

1. Click **Save changes**
2. If changes do not apply immediately:

  * Go to `Site administration → Development → Purge caches`
3. Test by:

  * Creating a blog entry
  * Checking visibility
  * Testing comments

---

# Recommended Configuration (Standard LMS)

| Setting                     | Recommended Value |
| --------------------------- | ----------------- |
| Enable blog associations    | Yes               |
| Blog visibility             | All site users    |
| Enable external blogs       | Yes (if needed)   |
| Cron schedule               | 24 hours          |
| Max external blogs per user | 1                 |
| Enable comments             | Yes               |
| Show comments count         | Yes               |

---

# Single Blog Content

## Add A New Blog Post
Please login to your Site admin > Enable the editing mode. Then navigate from the Main Menu > More > Blog > Click on Add a new entry button to start creating a new blog post.

![add-new-blog-post.png](img/add-new-blog-post.png)

