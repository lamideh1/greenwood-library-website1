### **Greenwood Library Website Project: Git Version Control and Web Development Adventure**

### **Project Overview**

This repository represents a collaborative web development project designed to showcase **book reviews** and **upcoming events**. The project is being developed collaboratively, with different contributors working on specific sections. The goal is to build a simple, expandable website that evolves over time, incorporating additional features and content such as **About Us**, **Contact Us**, a **Blog**, and other sections. The project integrates **Git version control** and collaborative development practices to enhance both the learning experience and the development process.

The website’s creative aspect comes from designing engaging user experiences, including interactive book reviews, event listings, and future interactive features. Students involved in this project apply **Git workflows**, manage branching and merging, and contribute creative content to a live project, simulating real-world web development.

---

### **Purpose and Goals**

The primary goal of this project is to create a user-friendly platform that showcases book reviews and upcoming events, with potential future features such as a dynamic events calendar, blog posts, or news updates. The website is being developed by a team of contributors, each focusing on different sections and functionalities. Through collaborative work, contributors will:

- Apply Git for version control, using best practices like branching, merging, and pull requests.
- Develop creative, engaging web content that provides a meaningful user experience.
- Learn how to scale and manage larger projects with multiple contributors.
- Introduce advanced features, such as dynamic content, interactive forms, and automated testing in the future.

---

### **Sections Added So Far**

#### **1. Book Reviews Section**
- **File**: `book_reviews.html`
- **Branch**: `morgan-book-reviews`
- **Description**: The book reviews section is designed to display reviews and ratings of various books. The page has a simple layout that includes:
  - A **title** for the section.
  - A **description** explaining the purpose of the page and its role in showcasing book reviews.
  
- **Development Process**:
  - **Branch Creation**: Morgan created the `book_reviews.html` file under the `morgan-book-reviews` branch.
  - **Design**: The design was kept simple to focus on user interaction and accessibility, with easy navigation for users to read and contribute their reviews.
  - **Integration**: After completion, the branch was merged into the main branch through a pull request for review.

- **Purpose**: This section allows users to easily navigate through reviews, rate books, and add their feedback. It provides the foundation for an evolving community-driven review system.

#### **2. Events Page**
- **File**: `events.html`
- **Branch**: `update-events`
- **Description**: The events page lists upcoming book-related events, such as author meetups, book fairs, webinars, and more.
  - **Title**: Highlights the title of the page.
  - **Description**: An overview of the events section, detailing the types of events users can find here.

- **Development Process**:
  - **Branch Creation**: Jamie worked on the `events.html` file under the `update-events` branch.
  - **Design**: The page features an organized list of events with an easy-to-read layout and registration buttons for users to sign up.
  - **Integration**: The branch was merged into the main project after review, with the pull request ensuring quality and error-free code.

- **Purpose**: The events page serves as a central hub for users to view and register for book-related events, further enhancing the website's functionality and user engagement.

---

### **Branch Workflow**

#### **1. Branches Created**
To maintain a clean, manageable workflow for collaborative development, the project followed a feature-based branching strategy. Each contributor created their own branch to work on specific features:

- **morgan-book-reviews**: Created to work on the book reviews section.
- **update-events**: Created for the events page functionality.

#### **2. Merging Work into Main**
Once the features were completed, each contributor merged their respective branches into the **main branch**. This merging was done using **pull requests (PRs)** to ensure the changes were reviewed and integrated correctly.

- **Pull Request Process**: A pull request was created for each branch, reviewed for code quality, and any necessary changes were requested before merging.
- **Conflict Resolution**: In case of any merge conflicts, contributors used Git’s built-in tools to resolve conflicts efficiently.

---

### **Key Actions Taken**

1. **Initialized the Project**:
   - The project began with creating a new Git repository. A **README.md** file was added to document the project’s purpose, structure, and development process.

2. **Developed the Book Reviews Section**:
   - The `book_reviews.html` page was created and added under the `morgan-book-reviews` branch.
   - This branch was merged into the main project after the section was reviewed and approved.

3. **Developed the Events Page**:
   - The `events.html` page was created under the `update-events` branch.
   - The branch was reviewed and merged into the main project, ensuring the features were integrated smoothly.

4. **Project Documentation**:
   - The **README.md** file was updated to reflect the additions of the new sections and provide a more detailed overview of the project structure and contributions.

---

### **How to Run the Project**

To view and run the project on your local machine, follow these steps:

1. **Clone the Repository**:
   First, clone the repository to your local machine:

   ```bash
   git clone <repository_url>
   ```

2. **Navigate to the Project Folder**:
   After cloning, change to the project directory:

   ```bash
   cd greenwood-library-website
   ```

3. **Open the Files in a Web Browser**:
   Open the HTML files in a browser to view the website.

---

### **Testing and Optimization**

Testing plays a crucial role in ensuring the website functions properly and delivers a positive user experience. Testing efforts so far have included:

- **Cross-browser compatibility** testing to ensure the website functions well across popular browsers like Chrome, Firefox, and Safari.
- **Responsive design** testing to ensure that the website looks great on different devices, including mobile phones and tablets.
- **Link validation** to ensure all internal and external links are working correctly.
- **Usability testing** to confirm that the website is user-friendly and intuitive.

For future optimization:

- **Automated Testing**: The project can be enhanced by integrating **automated testing** using tools like **Jest** or **Mocha** for unit testing and **Cypress** for end-to-end testing.
- **Continuous Integration**: Implementing **continuous integration (CI)** tools like **GitHub Actions** or **Travis CI** will allow for automated code testing and deployment, ensuring that every change is properly tested before it’s merged into the main branch.

---

### **Future Enhancements**

To further improve the project and ensure its growth:

1. **Adding More Interactive Sections**:
   - Future sections such as **About Us**, **Contact Us**, **Blog**, and **News** will be added, which will further expand the website’s capabilities.
   - A **dynamic events calendar** that automatically updates when new events are added will be integrated for a better user experience.

2. **Creative Design Enhancements**:
   - As contributors gain more experience, the project will integrate more creative elements like **animations**, **interactive user feedback forms**, and **custom graphics**.

3. **Advanced Features**:
   - Contributors will be encouraged to add more interactive features like **user-generated content**, **discussion forums**, and **book suggestion tools**.

---

### **Conclusion**

The **Greenwood Library Website** project successfully demonstrates the power of Git collaboration and creative web development. Through branching, merging, and pull requests, contributors worked together to build a functional, user-friendly platform for book reviews and upcoming events. Moving forward, the project will incorporate automated testing, continuous integration, and more advanced creative features, ensuring it remains dynamic, scalable, and engaging for users.
