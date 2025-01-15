### **Detailed Steps Taken for the Greenwood Library Website Project**

#### **1. Project Initialization**
- **Create Git Repository**: 
   - A new Git repository was initialized to begin the project.
   - The repository includes a `README.md` file, documenting the purpose of the project, key sections, and the intended workflow for contributors.
   
- **Repository Setup**:
   - Clone the repository to your local machine: 
     ```bash
     git clone <repository_url>
     ```

---

#### **2. Branch Creation and Collaboration Workflow**

- **Create Feature Branches**: 
   - Branches were created for different sections of the website to facilitate collaboration:
     - **`morgan-book-reviews`**: For the Book Reviews section.
     - **`update-events`**: For the Events section.

- **Add and Commit Changes to Feature Branches**:
   - On each branch, relevant changes were made, and files were added.
   - Example commits were made like:
     ```bash
     git commit -m "Added Book Reviews section"
     ```

---

#### **3. Development of Website Sections**

- **Book Reviews Section**:
   - Created a new HTML file (`book_reviews.html`) under the **`morgan-book-reviews`** branch.
   - This section includes:
     - A title for the page.
     - A brief description of the page’s purpose, which includes space for book reviews.
   
   - Added **Book Review Submission Form**:
     - Users can submit their own reviews via an HTML form.
     ```html
     <form action="submit_review.php" method="POST">
         <label for="book_title">Book Title:</label>
         <input type="text" id="book_title" name="book_title" required><br>
         <label for="author">Author:</label>
         <input type="text" id="author" name="author" required><br>
         <label for="rating">Rating (1-5):</label>
         <input type="number" id="rating" name="rating" min="1" max="5" required><br>
         <label for="review">Review:</label><br>
         <textarea id="review" name="review" rows="4" cols="50" required></textarea><br>
         <input type="submit" value="Submit Review">
     </form>
     ```

---

- **Events Section**:
   - Created a new HTML file (`events.html`) under the **`update-events`** branch.
   - This section contains a brief description of upcoming events and their details.
   - Events are now dynamically listed via a JSON file, which can be expanded in future versions to fetch data from a backend.
     Example JSON:
     ```json
     [
       {
         "title": "Author Meet-and-Greet",
         "date": "2025-02-10",
         "location": "Greenwood Library"
       },
       {
         "title": "Book Launch: The New Dawn",
         "date": "2025-03-15",
         "location": "Greenwood Auditorium"
       }
     ]
     ```

---

#### **4. Merging Feature Branches into Main**
- **Pull Requests (PRs)**:
   - After completing the development on each branch, pull requests were created for review.
   - Example PRs:
     - **PR for `morgan-book-reviews`**: Book Reviews section.
     - **PR for `update-events`**: Events page.
   - These PRs were merged into the `main` branch after successful reviews.

---

#### **5. Documentation and Git Workflow Enhancements**

- **Documented Conflict Resolution**:
   - Added a section in the `README.md` for resolving Git merge conflicts, ensuring contributors could handle conflicts properly.
   ```markdown
   ## Resolving Merge Conflicts
   If you encounter a merge conflict while integrating your changes with `main`, follow these steps:
   1. Run `git fetch` to get the latest changes from the remote.
   2. Run `git merge origin/main` to merge the changes into your branch.
   3. Resolve conflicts in the affected files and stage them with `git add <file>`.
   4. Commit the changes with `git commit`.
   5. Push your changes to the remote branch.
   ```

- **Code Review Process**:
   - Explained the code review process to ensure quality control.
   ```markdown
   ## Code Review Process
   - Submit a pull request after making changes to your branch.
   - Ensure your code is tested and follows the project’s style guidelines.
   - Assign a reviewer to check the code before merging.
   - Address any comments from reviewers before merging the changes.
   ```

---

#### **6. Advanced Git Features and CI Integration**

- **Git Rebase**:
   - To maintain a clean commit history, introduced the use of `git rebase` to keep feature branches up-to-date with `main` before merging.
   ```bash
   git checkout feature-branch
   git fetch
   git rebase origin/main
   ```

- **Continuous Integration (CI)**:
   - Set up GitHub Actions to automate HTML validation on every push to `main`:
     ```yaml
     name: HTML Validation

     on:
       push:
         branches:
           - main

     jobs:
       html-validation:
         runs-on: ubuntu-latest
         steps:
           - name: Checkout Repository
             uses: actions/checkout@v2

           - name: Install HTMLHint
             run: npm install -g htmlhint

           - name: Run HTML Validation
             run: htmlhint **/*.html
     ```

---

#### **7. Usability Testing and User Feedback**

- **User Feedback Form**:
   - Added a form to gather user feedback on the website’s functionality and user experience.
   ```html
   <form action="submit_feedback.php" method="POST">
       <label for="feedback">Your Feedback:</label><br>
       <textarea id="feedback" name="feedback" rows="4" cols="50" required></textarea><br>
       <input type="submit" value="Submit Feedback">
   </form>
   ```

- **Usability Testing**:
   - Planned usability testing sessions to gather real user input on the website’s interface, improving user experience based on feedback.

---

#### **8. Final Merging and Push to Main Branch**
- **Final Review and Merging**:
   - After completing all feature development and testing, the final changes were pushed to the `main` branch.

   - Final merge command:
     ```bash
     git checkout main
     git pull origin main
     git merge <feature-branch>
     git push origin main
     ```

---

### **Conclusion**

These detailed steps outline the comprehensive approach you took to develop and enhance the **Greenwood Library Website**. From the creation of new sections (Book Reviews and Events) to setting up collaborative workflows, resolving merge conflicts, and integrating automated testing, each step contributes to improving the website's functionality and overall project structure.

Additionally, the Git workflows were optimized for smoother collaboration with features like Git rebase and automated validation through CI. The project is now better equipped for growth and further enhancements, such as adding dynamic event management and interactive features for users.
