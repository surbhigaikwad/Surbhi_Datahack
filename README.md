# Text-to-Website Generator

## Overview
The **Text-to-Website Generator** is a web application that transforms natural language descriptions into fully functional, responsive websites in real-time. Designed for users with little to no coding experience, this tool provides an intuitive interface to create professional-looking websites effortlessly.

## Features
1. **Intuitive No-Code Interface**  
   - Users can describe their website requirements in simple natural language.  
   - A user-friendly input field ensures seamless interaction.  

2. **Dynamic Website Generation**  
   - Converts user descriptions into responsive websites.  
   - Users can choose from predefined color palettes and layouts.  
   - Provides front-end code for further customization.  

3. **Drag-and-Drop Customization**  
   - Allows easy adjustments to navigation menus, elements, fonts, and colors.  
   - No technical expertise required for modifications.  

4. **Re-Prompting and Fine-Tuning**  
   - Users can iteratively refine and modify the generated website.  
   - Minor tweaks and updated prompts allow for better customization.  

5. **Fast Generation**  
   - Websites are generated in under five minutes.  
   - Optimized for efficiency and high-quality output.  

6. **Login & Signup Page**  
   - Users can create an account or log in to save projects.  
   - Secure authentication ensures data privacy and easy access.  

---

## Product UI

### Installation

#### Prerequisites
- Node.js and npm installed
- Python (for backend processing if required)
- Git

#### Steps
1. Clone the repository:
   ```sh
   git clone https://github.com/Kriti-Product-Development/WebGalaxy.git
   cd WebGalaxy
   ```
### 2. Install dependencies for the frontend:
```sh
cd frontend
npm install
```
### 3. Start the application:
```sh
npm start
```
# Text-to-Website Generator

## Usage
1. Open the application in a web browser.
2. Sign up or log in to your account.
3. Enter a description of the website you want.
4. Click **"Generate"** to create a website based on your input.
5. Use the drag-and-drop editor to customize elements.
6. Select a template from the available options and customize it.
7. Download the generated code for further development if needed.

---

## Architecture
The application consists of:
- **User Authentication** using Firebase Console.
- **Frontend:** Built with React.js for a dynamic UI/UX.
- **Backend:** Built with Flask to handle input processing and model integration.
- **AI Model:** NLP-based system to parse and interpret user prompts into structured HTML and CSS.

---

## Tech Stack
### **Frontend:**
- **React.js** – For building the user interface.
- **Tailwind CSS** – For consistent and responsive styling.

### **Backend:**
- **Node.js + Express** – For handling API requests and input processing.
- **Python** – For AI model processing.

### **AI/NLP:**
- **Gemini** – For natural language prompt processing.

### **Database:**
- **Firebase** – For real-time authentication.

---
## MODEL UI
### Overview
This AI-powered tool enables the automated generation and enhancement of website templates using Google Gemini models. By analyzing user input, it intelligently modifies HTML, CSS, and images to produce optimized, modern web designs.

### Features
- AI-driven template selection and customization.
- Google Gemini API integration for content extraction and transformation.
- Automated HTML structure improvements.
- Dynamic color palette generation based on themes.
- Intelligent image selection via Unsplash API.
- Regeneration of existing templates using alternative matches.

### Installation
#### Prerequisites
Ensure you have Python installed
Set up the environment variables by creating a .env file or using product_development.env.
Set up Pipenv and install dependencies by running:
  pipenv shell
To generate a fresh requirements.txt file from an existing environment:
  pip freeze > requirements.txt
  

### Environment Setup
Create a `.env` file or use `product_development.env`:
```env
GEMINI_API_KEY_1=your_key_here
GEMINI_API_KEY_2=your_key_here
GEMINI_API_KEY_3=your_key_here
UNSPLASH_API_KEY=your_key_here
```
Load variables in Python:
```python
from dotenv import load_dotenv
load_dotenv("product_development.env")
```

### How to Start Website Generation (this is where the model runs)
#### 1. 
To generate a website based on user input, run:
```bash
python website_generator_model.py
```
Then, enter the prompt specifying the website you want to generate. The generated website will be stored in the generated folder.
#### 2. Website Regeneration
For regenerating templates with an alternative match:
```bash
python update_regenerate.py
```
Here, the user will enter the prompt either to regenerate the whole website or update specific sections based on the prompt. The updated website will be saved in the generated folder, where the user can run and check the modifications.


## Known Issues & Bugs
- Some complex user prompts may generate incorrect layouts.
- The drag-and-drop editor may have responsiveness issues on mobile.
- Optimization for generation time needs further improvement.

---
## Future Enhancements
- **Advanced AI-driven Layout Generation** – Improve AI logic to generate more dynamic and diverse layouts.
- **Multi-Page Website Support** – Extend support for generating multiple pages with navigation linking.
- **Prebuilt Templates & Themes** – Allow users to select from pre-designed templates and themes.
- **User Authentication & Cloud Storage** – Enable users to save and edit projects.
- **Backend Code Generation** – Extend AI capabilities to generate backend code for dynamic functionality (e.g., form submissions, database storage).
- **Mobile App Version** – Develop a mobile application for on-the-go website creation.

---
