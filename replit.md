# Careers Website

## Overview
A professional careers website built with Python Flask that displays job openings and company benefits. This project was imported from GitHub and configured to run in the Replit environment.

**Current State**: Fully functional Flask web application with a responsive design

## Purpose
This website serves as a career portal where:
- Visitors can view available job positions
- Learn about company benefits and culture
- Browse job listings with location and salary information

## Recent Changes
- **October 19, 2025**: Initial Replit environment setup
  - Configured Python 3.11 with Flask and Gunicorn
  - Created Flask application with two routes (home and jobs pages)
  - Added responsive HTML templates with modern styling
  - Configured workflow to run on port 5000
  - Set up deployment configuration for production

## Project Architecture

### Structure
```
careers-website/
├── app.py                 # Main Flask application
├── templates/             # HTML templates
│   ├── home.html         # Homepage with hero section and job preview
│   └── jobs.html         # Full job listings page
├── static/               # Static assets
│   └── style.css         # Responsive CSS styling
├── pyproject.toml        # Python dependencies
└── uv.lock              # Dependency lock file
```

### Tech Stack
- **Backend**: Python 3.11 with Flask framework
- **Frontend**: HTML5, CSS3 (responsive design)
- **Template Engine**: Jinja2 (included with Flask)
- **Production Server**: Gunicorn
- **Package Manager**: UV (Python package manager)

### Key Features
1. **Home Page** (`/`):
   - Hero section with call-to-action
   - Benefits showcase with 4 key selling points
   - Preview of all available positions
   - Link to full job listings

2. **Jobs Page** (`/jobs`):
   - Detailed view of all job openings
   - Job cards with title, location, and salary
   - Apply and Learn More buttons (currently placeholders)

3. **Responsive Design**:
   - Mobile-friendly layout
   - Grid-based job cards
   - Adaptive navigation

### Current Job Listings
The application currently includes 4 sample positions:
- Software Engineer (San Francisco, CA)
- Data Analyst (Remote)
- Product Manager (New York, NY)
- UX Designer (Austin, TX)

## Configuration

### Development
- Server runs on `0.0.0.0:5000` with debug mode enabled
- Hot reload enabled for development
- Workflow: `python app.py`

### Production (Deployment)
- Uses Gunicorn WSGI server
- Configured for autoscale deployment
- Command: `gunicorn --bind=0.0.0.0:5000 --reuse-port app:app`

## Future Enhancements
Potential improvements to consider:
- Database integration for dynamic job listings
- Job application form functionality
- Admin panel for managing job postings
- Search and filter capabilities
- Integration with applicant tracking system
