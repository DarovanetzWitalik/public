# GITHUB_ISSUES_AND_PRS

Нижче готові тексти, які можна просто вставити в GitHub.

---

## Issue 1
**Title:** Refactor duplicated navigation markup across HTML pages

**Body:**
```md
The project repeats the same navigation block in every HTML page.
This violates the DRY principle and makes maintenance harder: if one menu item changes, the same edit must be repeated in several files.

Affected code:
- YOUR_REPO_URL/blob/main/index.html#L11-L17
- YOUR_REPO_URL/blob/main/task1.html#L11-L17
- YOUR_REPO_URL/blob/main/task2.html#L11-L17
- YOUR_REPO_URL/blob/main/task3.html#L11-L17
- YOUR_REPO_URL/blob/main/task4.html#L11-L17

Suggested fix:
- move navigation generation into a shared JS component or server-side include;
- keep one source of truth for the menu structure.
```

**Branch name:** `fix/shared-navigation`

**Commit message:** `Refactor duplicated navigation into shared component`

**PR title:** `Refactor duplicated navigation`

**PR body:**
```md
This pull request removes duplicated navigation markup and replaces it with a shared reusable solution.

Closes #1
```

---

## Issue 2
**Title:** Move inline styles from HTML into CSS classes

**Body:**
```md
Several pages use inline styles directly inside HTML tags.
This breaks separation of concerns because presentation is mixed with page structure.
It also makes the styling harder to reuse and maintain.

Affected code:
- YOUR_REPO_URL/blob/main/task2.html#L19-L29
- YOUR_REPO_URL/blob/main/task3.html#L25-L55

Suggested fix:
- create dedicated CSS classes in style.css;
- replace inline style attributes with class names.
```

**Branch name:** `fix/remove-inline-styles`

**Commit message:** `Move inline styles to stylesheet`

**PR title:** `Move inline styles to CSS classes`

**PR body:**
```md
This pull request removes inline styling from HTML and moves presentation rules into the shared stylesheet.

Closes #2
```

---

## Issue 3
**Title:** Replace deprecated big tag with CSS-based solution

**Body:**
```md
The project uses the deprecated <big> tag in task1.html.
Although it still works in some browsers, it is not recommended in modern HTML and should be replaced with semantic markup plus CSS.

Affected code:
- YOUR_REPO_URL/blob/main/task1.html#L27-L30
- YOUR_REPO_URL/blob/main/task1.html#L55-L55

Suggested fix:
- replace <big> with <span class="text-large">...</span>;
- add the corresponding class in style.css.
```

**Branch name:** `fix/replace-big-tag`

**Commit message:** `Replace deprecated big tag with CSS class`

**PR title:** `Replace deprecated big tag`

**PR body:**
```md
This pull request replaces deprecated HTML markup with a CSS-based and more maintainable solution.

Closes #3
```
