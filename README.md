

---

### Comprehensive Steps and Procedures for the Greenwood Library Website Project

---

### **1. Project Initialization**

#### **1.1. Set Up Repository**

The first step was setting up the project repository on GitHub to manage version control and collaboration efficiently. This allows all contributors to work simultaneously on different sections, ensuring that changes are tracked and the project remains organized.

- **Create Repository**: 
  - A new repository called `greenwood-library-website` was created on GitHub.
  - A `README.md` file was included at the start to explain the purpose and goals of the project.

  ```bash
  git init greenwood-library-website
  cd greenwood-library-website
  touch README.md
  ```

- **Add Project Description**: 
  - The `README.md` was populated with a brief description of the website’s purpose, its key sections (Book Reviews and Events), and the contributors.
  
  **README.md**:
  ```markdown
  # Greenwood Library Website
  A simple, clean, and expandable website showcasing book reviews and upcoming events related to books and authors.
  
  ## Sections
  - **Book Reviews**
  - **Upcoming Events**
  
  Contributors: Morgan (Book Reviews), Jamie (Events)
  ```

#### **1.2. Define Project Structure**

The basic folder and file structure for the website was set up to house all content:
- **book_reviews.html**: For the book reviews section.
- **events.html**: For the events section.
- **index.html**: Placeholder for the homepage (future addition).
- **README.md**: Project documentation.

The structure looked like this:

```
greenwood-library-website/
├── book_reviews.html
├── events.html
├── index.html (future)
└── README.md
```

---

### **2. Development of Website Sections**

The project was developed in modular sections to ensure clarity and expandability.

#### **2.1. Book Reviews Section (Branch: `morgan-book-reviews`)**

Morgan was assigned to develop the **Book Reviews** section. 

- **Step 1**: **Create a new branch** for working on the book reviews page.
  ```bash
  git checkout -b morgan-book-reviews
  ```

- **Step 2**: **Develop the Book Reviews Page** (`book_reviews.html`)
  - The HTML structure was created with the following components:
    - Title for the page
    - A brief description to explain the section’s purpose
    - A list of sample books with reviews and ratings for future contributions.
    
    **book_reviews.html**:
    ```html
    <!DOCTYPE html>
    <html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Book Reviews</title>
    </head>
    <body>
        <header>
            <h1>Book Reviews</h1>
            <p>Explore the reviews of books read by our contributors.</p>
        </header>
        <section>
            <article>
                <h2>Title of Book 1</h2>
                <p>Review content for the first book goes here. The review will include thoughts, ratings, and recommendations.</p>
            </article>
            <article>
                <h2>Title of Book 2</h2>
                <p>Review content for the second book goes here...</p>
            </article>
        </section>
    </body>
    </html>
    ```

- **Step 3**: **Commit the changes** and push them to GitHub.
  ```bash
  git add book_reviews.html
  git commit -m "Added Book Reviews Section"
  git push origin morgan-book-reviews
  ```

---

#### **2.2. Events Section (Branch: `update-events`)**

Jamie was assigned to develop the **Events** section.

- **Step 1**: **Create a new branch** for working on the events page.
  ```bash
  git checkout -b update-events
  ```

- **Step 2**: **Develop the Events Page** (`events.html`)
  - The structure was similar to the book reviews page, featuring:
    - Title for the page
    - A brief description of the events section
    - A list of upcoming events with relevant details such as date, location, and description.
    
    **events.html**:
    ```html
    <!DOCTYPE html>
    <html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Upcoming Events</title>
    </head>
    <body>
        <header>
            <h1>Upcoming Events</h1>
            <p>Stay informed about upcoming book-related events and activities.</p>
        </header>
        <section>
            <article>
                <h2>Book Fair 2025</h2>
                <p>Date: March 1, 2025</p>
                <p>Location: City Convention Center</p>
                <p>Description: Join us for a celebration of books with authors, readers, and publishers.</p>
            </article>
            <article>
                <h2>Author Meet-and-Greet</h2>
                <p>Date: April 10, 2025</p>
                <p>Location: Downtown Bookstore</p>
                <p>Description: Meet the author of "The Best Fiction Book" and get your copy signed!</p>
            </article>
        </section>
    </body>
    </html>
    ```

- **Step 3**: **Commit the changes** and push them to GitHub.
  ```bash
  git add events.html
  git commit -m "Added Events Section"
  git push origin update-events
  ```

---

### **3. Merging Work into the Main Branch**

Once both the **Book Reviews** and **Events** sections were complete, it was time to **merge** both branches (`morgan-book-reviews` and `update-events`) into the `main` branch.

- **Step 1**: Review the pull requests.
  - The pull request process was used to review and discuss the code before merging into `main`.
  
- **Step 2**: **Merge both branches into main**.
  - After reviewing and approving the changes in both pull requests, the branches were merged into `main` using GitHub’s interface.
  
  ```bash
  git checkout main
  git merge morgan-book-reviews
  git merge update-events
  ```

---

### **4. Documentation and Updates**

To ensure the project was well-documented and the information was clear for future developers or collaborators, the **`README.md`** file was updated.

- **Add Project Details**:
  - Descriptions of each section.
  - Clear instructions for running the project.
  
  **README.md**:
  ```markdown
  # Greenwood Library Website
  
  This website showcases book reviews and upcoming events. It is designed to be simple, clean, and expandable.
  
  ## Sections
  - **Book Reviews**: A collection of reviews for various books.
  - **Upcoming Events**: A list of book-related events and activities.
  
  Contributors:
  - **Morgan**: Developed the Book Reviews section.
  - **Jamie**: Developed the Events section.
  
  ## How to Run the Project
  
  Clone the repository to your local machine:
  ```bash
  git clone <repository_url>
  ```
  
  To run the website locally, open the `book_reviews.html` and `events.html` files in your browser.
  ```

- **Commit and Push the README Changes**:
  ```bash
  git add README.md
  git commit -m "Updated README with project details"
  git push origin main
  ```

---

### **5. Testing and Validation**

Before considering the project finished, various tests were performed to ensure the site was functioning as expected:

1. **Cross-Browser Testing**: 
   - The website was tested across different browsers (Chrome, Firefox, Safari) to ensure it looked and behaved consistently.

2. **Responsive Design**: 
   - The pages were checked for mobile responsiveness to ensure the layout adjusts properly across various screen sizes (phone, tablet, desktop).

3. **Link Validation**: 
   - All links were tested to ensure they led to the correct pages and external links (if any) worked properly.

4. **Basic Usability Testing**: 
   - Feedback was gathered on the navigation and overall user experience to confirm that the sections were easy to find and the layout was intuitive.

---

### **6. Future Enhancements**

To ensure the website grows over time, you planned and documented several potential future features:

- **Dynamic Content**: Interactive calendar for events.
- **Additional Pages**: About Us, Contact Us, and Blog sections.
- **User Interaction**: Allow users to submit reviews directly on the website.

---

### **7. How to Run the Project Locally**

To run the project on your local machine:

1. **Clone the repository**:
   ```bash
   git clone <repository_url>
   ```

2. **Navigate into the project folder**:
   ```bash
   cd greenwood-library-website
   ```

3. **Open HTML files in your browser**:
   - Open the `book_reviews.html
