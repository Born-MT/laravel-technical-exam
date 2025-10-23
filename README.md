# Laravel Developer Technical Exam

**Time Limit:** 24 hours  
**Project Type:** CLI Application with API Integration

## Project Overview
Build a News Aggregator application that fetches articles from a public news API, stores them in a database, and displays them through a web interface.

---

## Core Requirements

### 1. **API Integration**
- Integrate with NewsAPI (https://newsapi.org/) or any similar free news API
- Create a Laravel Artisan command to fetch articles from multiple news sources/categories
- The command should be schedulable or accept parameters (e.g., category, date range, number of articles) in runtime execution.
- Handle API rate limiting and errors gracefully
- Log all API interactions (success/failure)

### 2. **Database & Models**
- Design and implement appropriate database schema for:
  - Articles (title, description, content, author, source, published date, URL, image URL)
  - Categories (technology, business, sports, etc.)
  - Sources (news outlets)
- Implement proper relationships between models
- Use migrations and seeders
- Apply appropriate indexes for performance

### 3. **Data Validation**
- Validate all incoming API data before saving
- Implement custom validation rules where appropriate
- Prevent duplicate articles from being saved
- Sanitize and format data (dates, URLs, text)

### 4. **Controllers & Views**
- Create a web interface with the following pages:
  - Homepage: Display latest articles (paginated)
  - Article detail page
- Use Blade templates with proper layout inheritance
- Display article images, titles, descriptions, and publication dates
- Include proper error handling and user feedback

### 5. **Clean Code Practices**
- Follow SOLID principles
- Implement Service classes to separate business logic from controllers
- Use Repository pattern for data access
- Create dedicated classes for API communication
- Write clean, self-documenting code with appropriate comments
- Follow PSR-12 coding standards
- Implement proper exception handling

---

## Nice to Have (Bonus Points)

### 6. **Authentication**
- User registration and login
- Allow authenticated users to bookmark/favorite articles
- Personal dashboard showing saved articles

### 7. **Frontend Enhancement**
- Implement one of the following:
  - **Vue.js** components for interactive filtering/search
  - **Livewire** for real-time article updates without page refresh
  - **Inertia.js** for SPA-like experience
- Add loading states and smooth transitions
- Filter/search functionality by category, source, or date range

### 8. **Additional Features**
- Email notifications for new articles in followed categories
- Export articles to PDF or CSV
- Article reading time estimation
- Dark mode toggle

---

## Deliverables

1. GitHub repository with clear README including:
   - Setup instructions
   - API key configuration steps
   - How to run the CLI command
   - Database setup instructions

2. `.env.example` file with all required configuration

3. Brief documentation explaining:
   - Your architectural decisions
   - Design patterns used
   - How you ensured code quality

---

## Evaluation Criteria

- **Functionality** (30%): Does it work as specified?
- **Code Quality** (30%): Clean, maintainable, follows best practices
- **Laravel Knowledge** (20%): Proper use of framework features
- **Database Design** (10%): Efficient schema and relationships
- **Documentation** (10%): Clear setup and explanation
