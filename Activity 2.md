## 🐛 Activity 2: The Bug Hunt Challenge
**Mission:** Debug the Recipe Book! Find bugs, report them, and fix them like a pro developer.

### 🎯 What You'll Learn
- Creating and managing GitHub Issues
- Claiming and assigning issues
- Linking Pull Requests to Issues
- Professional bug reporting

---

### 📋 Phase 1: Bug Reporting (Everyone Reports 2 Bugs)

**Your Task:** Find 2 "bugs" in OTHER people's recipes and report them as Issues.

**What counts as a bug?**
- 🔴 Missing ingredients in the ingredients list but mentioned in instructions
- 🔴 Incorrect cooking time (e.g., "Cook rice for 2 minutes")
- 🔴 Missing steps in instructions
- 🔴 Typos or formatting issues
- 🔴 Confusing or unclear instructions
- 🔴 Missing difficulty level or cooking time

**How to Report a Bug:**

1. Go to the **Issues** tab in the repository
2. Click **New Issue**
3. Use this format:
```markdown
**Title:** Bug in [Recipe Name] - [Brief Description]

**Example:** Bug in sarah-midnight-ramen.md - Missing ingredient in recipe

**Description:**
- **Recipe File:** `folder-name/file-name.md`
- **Bug Type:** Missing ingredient / Wrong time / Typo / etc.
- **Description:** The instructions mention "soy sauce" but it's not listed in ingredients.
- **Line Number (if applicable):** Line 12

**Suggested Fix:**
Add "2 tablespoons soy sauce" to the ingredients list.
```

4. Add a **label** (bug, documentation, etc.)
5. Click **Submit new issue**

---

### 🔧 Phase 2: Bug Fixing (Fix 2 Bugs Reported by Others)

**Your Task:** Choose 2 issues reported by OTHER people and fix them!

**Steps to Fix a Bug:**

1. **Claim the Issue**
   - Comment on the issue: "I'll fix this! 🛠️"
   - This lets others know you're working on it

2. **Create a Branch**
```bash
   git checkout -b fix-issue-#[issue-number]
```
   Example: `git checkout -b fix-issue-#5`

3. **Make Your Fix**
   - Open the recipe file mentioned in the issue
   - Fix the bug
   - Save the file

4. **Commit Your Changes**
```bash
   git add .
   git commit -m "Fix: [Brief description] - Closes #[issue-number]"
```
   Example: `git commit -m "Fix: Add missing soy sauce to ingredients - Closes #5"`

5. **Push Your Branch**
```bash
   git push origin fix-issue-#[issue-number]
```

6. **Create a Pull Request**
   - Go to GitHub repository
   - Click **Pull Requests** → **New Pull Request**
   - Select your branch
   - Use this PR format:
```markdown
   **Title:** Fix: [Brief description] (Closes #[issue-number])
   
   **Description:**
   Fixes #[issue-number]
   
   **Changes Made:**
   - Added missing ingredient "soy sauce" to ingredients list
   - Fixed typo in step 3
   
   **Testing:**
   - Verified all ingredients mentioned in instructions are now in the list
```

7. **Link the Issue**
   - In your PR description, write `Fixes #[issue-number]` or `Closes #[issue-number]`
   - This automatically closes the issue when PR is merged!

---

### 🎊 Bonus Challenges

- 🏆 **Bug Hunter Badge:** First person to report 5 valid bugs
- 🛠️ **Fix Master:** First person to fix 5 issues
- 🤝 **Collaborator Pro:** Help someone else fix their issue through comments

---

### 📌 Important Rules

✅ **DO:**
- Report bugs in OTHER people's recipes (not your own)
- Fix bugs reported by OTHER people (not bugs in your own recipe)
- Be respectful and constructive in bug reports
- Claim an issue before working on it

❌ **DON'T:**
- Report fake or silly bugs just to increase count
- Work on an issue someone else has claimed
- Fix bugs in your own recipe (wait for others to report them)

---

### 🎯 Success Checklist

By the end of this activity, you should have:
- [ ] Reported 2 bugs as Issues
- [ ] Claimed 2 issues to fix
- [ ] Created 2 branches (one for each fix)
- [ ] Made 2 Pull Requests
- [ ] Linked PRs to Issues using "Closes #X"
- [ ] Learned how real bug tracking works!

---

### 💡 Pro Tips

- **Use descriptive issue titles** - Future you will thank present you!
- **Screenshots help** - If there's a visual bug, add a screenshot
- **One issue = One problem** - Don't combine multiple bugs in one issue
- **Check existing issues** - Someone might have already reported it!
- **Learn from the best (and worst)** - [Good example](https://github.com/deepseek-ai/DeepSeek-V3/issues/1069) ✅ vs [Bad example](https://github.com/deepseek-ai/DeepSeek-V3/issues/1073) ❌
---