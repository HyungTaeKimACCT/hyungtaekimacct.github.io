---
layout: default
title: Teaching
---

<section class="section bg-light">
    <div class="container">
        <h2 class="section-title">Teaching</h2>
        <div class="content-card">
            <h3>Course Materials by Semester</h3>
            <p>Students can access lecture notes and course materials through the links below:</p>
            
            <div class="teaching-grid">
                <!-- Fall 2026 -->
                <div class="course-item">
                    <h4>Fall 2026 - ACCT 162 Auditing</h4>
                    
                    <!-- Week 1 Example -->
                    <div class="week-section">
                        <h5>Week 1: Introduction to Auditing</h5>
                        
                        <!-- YouTube Video Embed -->
                        <div class="video-container">
                            <iframe width="100%" height="400" 
                                src="https://www.youtube.com/embed/YOUR-VIDEO-ID" 
                                title="Week 1 Lecture" 
                                frameborder="0" 
                                allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" 
                                allowfullscreen>
                            </iframe>
                        </div>
                        
                        <!-- Course Materials -->
                        <div class="course-links">
                            <a href="{{ '/assets/course-materials/acct162/week1-notes.pdf' | relative_url }}" target="_blank" class="course-link">• View Lecture Notes (PDF)</a>
                            <a href="{{ '/assets/course-materials/acct162/week1-notes.pdf' | relative_url }}" download class="course-link">• Download Lecture Notes</a>
                        </div>
                    </div>
                    
                    <!-- Add more weeks as needed -->
                    <p style="margin-top: 1.5rem; color: var(--text-light); font-size: 0.9rem;">
                        <em>Additional weeks will be added as the semester progresses.</em>
                    </p>
                </div>
            </div>
            
            <div class="office-hours-section">
                <h3>Office Hours</h3>
                <p>Schedule a meeting during office hours: <a href="https://calendar.google.com/calendar/appointments/schedules/YOUR-SCHEDULE-ID" target="_blank" class="office-hours-link">Book Appointment</a></p>
            </div>
        </div>
    </div>
</section>

<style>
.week-section {
    margin-bottom: 2rem;
    padding-bottom: 2rem;
    border-bottom: 1px solid var(--border-color);
}

.week-section:last-of-type {
    border-bottom: none;
}

.week-section h5 {
    font-size: 1rem;
    font-weight: 600;
    color: var(--text-dark);
    margin-bottom: 1rem;
}

.video-container {
    margin: 1rem 0;
    position: relative;
    padding-bottom: 56.25%; /* 16:9 aspect ratio */
    height: 0;
    overflow: hidden;
    background-color: #000;
}

.video-container iframe {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
}
</style>
