# Wildlife and Fisheries Authorizations — Team Repository Hub

A GitHub Pages site that acts as a central hub for all BC Government Wildlife and Fisheries Authorizations team repositories.

**Live site:**

---

## How to Add a Repository



1. Open **`repos.js`** in any text editor.
2. Copy an existing entry (the `{ … }` block) and paste it _before_ the closing `]`.
3. Make sure the previous entry ends with a **comma** `,`.
4. Fill in the four fields:

```js
{
  name: "My Repository",              // Display name on the card
  description: "What this does.",     // One sentence description
  url: "https://github.com/bcgov/…", // Full URL to the repository
  language: "Python"                  // Optional. Leave "" to hide badge.
                                      // Options: Python, R, JavaScript,
                                      //          TypeScript, SQL, Shell, Bash
}
```

5. **Save** the file.


## 🗑 How to Remove a Repository

Delete the `{ … }` block for the repository in `repos.js`. Make sure commas `,` between remaining entries are correct.


## Design

- **Colours:** BC Government blue (`#234075`) and gold (`#E3A82B`)
- **Font:** BC Sans (loaded from the BC Government CDN)
- **Logo:** Official BC Mark loaded from the BC Government developer portal
- **Responsive:** Works on desktop, tablet, and mobile


