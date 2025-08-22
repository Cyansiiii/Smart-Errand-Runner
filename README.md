# Smart Errand Runner 🚀

**A location-aware web application that intelligently streamlines daily errands by discovering venues, suggesting related tasks with AI, and calculating the most efficient multi-stop route.**

This project is a technical showcase demonstrating the integration of modern frontend technologies, third-party APIs for geospatial data, and a generative AI model to create a powerful, real-world utility.

---

### ✨ Live Demo

*[https://github.com/Cyansiiii/Smart-Errand-Runner]*

---

 (Core Features)

* **Intelligent Venue Discovery**: Powered by the **Foursquare Places API**, the application can find any business or service from millions of venues. It searches for the best, closest, and highest-rated options that are currently open.
* **AI-Powered Suggestions**: Utilizes the **Gemini API** to provide smart, context-aware recommendations. Based on a user's errand list and nearby venues, the AI suggests related tasks or logical groupings to make the trip even more efficient.
* **Optimal Route Calculation**: The application's core logic solves the "Traveling Salesperson Problem" for a user's daily tasks. It calculates the most efficient multi-stop route to save time, fuel, and mental energy.
* **Dynamic & Interactive UI**: Built with a modern, responsive interface that provides immediate feedback, making it easy to manage your errand list and visualize your plan.

---

### 🛠️ Technology Stack

This project is built with a modern, scalable stack designed for performance and maintainability.

| Tier      | Technology                               | Purpose                                                              |
| :-------- | :--------------------------------------- | :------------------------------------------------------------------- |
| **Frontend** | **React** & **Tailwind CSS** | For a dynamic, component-based, and beautifully styled user interface. |
| **Mapping** | **Mapbox** | For high-performance interactive maps and route optimization.        |
| **Location** | **Foursquare Places API** | For rich, accurate, and comprehensive Point of Interest (POI) data.  |
| **AI** | **Google Gemini API** | For generating intelligent, context-aware errand suggestions.        |
| **Backend** | **Serverless Architecture (AWS Lambda)** | To securely manage API calls and ensure scalability.                 |

---

### 🔑 API Keys & Setup

To run this project locally or deploy it yourself, you will need to configure the necessary API keys. The application logic for handling these keys is in place.

1.  **Foursquare API Key**:
    * Sign up for a developer account at [Foursquare for Developers](https://location.foursquare.com/).
    * Create a new project and get your API Key.
    * In the `script` tag within the HTML, find the following line and replace the placeholder with your key:
        ```javascript
        const FOURSQUARE_API_KEY = 'YOUR_FOURSQUARE_API_KEY_HERE';
        ```

2.  **Gemini API Key**:
    * Get an API key from [Google AI Studio](https://aistudio.google.com/app/apikey).
    * In the `script` tag, find the following line and replace the placeholder if you are not using the free-tier model:
        ```javascript
        const GEMINI_API_KEY = ""; // The key is handled by the environment for the default model
        ```

---

### ⚙️ How It Works

The application follows a simple yet powerful workflow:

1.  **User Input**: The user enters their list of errands in natural language (e.g., "get coffee, mail a package, buy groceries").
2.  **Venue Discovery**: The application sends a request to the **Foursquare API**, using the user's query and a set location to find relevant, open, and nearby venues.
3.  **AI Enrichment**: The list of nearby venues is combined with the original errand list and sent to the **Gemini API**. Gemini analyzes this context to generate helpful suggestions, such as "Since you're near a pharmacy, you could also pick up prescriptions."
4.  **Display Results**: The AI-powered suggestions are displayed to the user in a clean, easy-to-read format.

---

### 🔮 Future Roadmap

This project serves as a strong foundation. Future enhancements could include:

* **User Accounts**: Allow users to save and manage recurring errand lists.
* **Real-Time Traffic**: Integrate live traffic data for even more accurate route optimization.
* **Personalization**: Use machine learning to tailor suggestions based on user history and preferences.
* **Native Mobile Apps**: Package the application for iOS and Android for a better on-the-go experience.
