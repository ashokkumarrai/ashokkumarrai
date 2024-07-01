// Command: Create HA Doctor Portfolio Website

// Step 1: Basic Information
CreatePage: Home
SetTitle: "Dr. Jane Doe, MD - Holistic Health Advocate"
SetSubtitle: "Integrating Traditional Medicine with Holistic Approaches"
AddSection: 
  - Type: Hero
  - Image: "hero_image.jpg"
  - Headline: "Welcome to My Practice"
  - Subheadline: "Your Health, Holistically Enhanced"
  - CallToAction: "Schedule an Appointment"

// Step 2: About Me
CreatePage: About
SetTitle: "About Dr. Jane Doe"
AddSection: 
  - Type: Bio
  - Headline: "Meet Dr. Jane Doe"
  - Image: "dr_jane_doe.jpg"
  - Text: "With over 15 years of experience in integrative medicine, Dr. Jane Doe combines conventional treatments with holistic therapies to promote overall well-being."

// Step 3: Services Offered
CreatePage: Services
SetTitle: "Our Services"
AddSection: 
  - Type: ServicesList
  - Headline: "Comprehensive Care Tailored to You"
  - Services: 
      - Name: "General Medicine"
        Description: "Complete primary care services."
        Image: "general_medicine.jpg"
      - Name: "Holistic Nutrition"
        Description: "Personalized nutrition plans."
        Image: "holistic_nutrition.jpg"
      - Name: "Mind-Body Therapies"
        Description: "Integrative therapies for mental and physical health."
        Image: "mind_body_therapies.jpg"

// Step 4: Testimonials
CreatePage: Testimonials
SetTitle: "What Patients Are Saying"
AddSection: 
  - Type: Testimonials
  - Headline: "Testimonials"
  - Testimonials: 
      - Text: "Dr. Doe's holistic approach has transformed my health!"
        Author: "John Smith"
      - Text: "I feel more energetic and balanced."
        Author: "Mary Johnson"

// Step 5: Blog
CreatePage: Blog
SetTitle: "Health Insights Blog"
AddSection: 
  - Type: BlogOverview
  - Headline: "Latest Articles"

// Step 6: Contact
CreatePage: Contact
SetTitle: "Get in Touch"
AddSection: 
  - Type: ContactForm
  - Headline: "Contact Dr. Jane Doe"
  - Fields: ["Name", "Email", "Phone", "Message"]
  - SubmitButtonText: "Send Message"

// Step 7: Footer
AddFooter: 
  - Sections:
      - ContactInfo: 
          - Text: "123 Wellness Way, Suite 100, Healthy City, ST 12345 | (123) 456-7890 | email@example.com"
      - SocialMedia: 
          - Icons: ["Facebook", "Twitter", "LinkedIn", "Instagram"]
      - QuickLinks: 
          - Links: ["Home", "About", "Services", "Blog", "Contact"]

<footer>
    <p>&copy; 2024 Dr. Jane Doe. All rights reserved.</p>
    <p>Powered by [ANB GRaphic & Tech Solutions]</p>
    <?php wp_footer(); ?>
</footer>
</body>
</html>

// Additional Settings
SetTheme: "Modern, Clean, Professional"
EnableSEO: True
EnableAnalytics: True
