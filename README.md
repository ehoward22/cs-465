# Architecture:

In this project, I employed a combination of HTML, JavaScript (JS), Express, and Angular as the architectural foundations for the frontend. On the customer-facing side, I leveraged HTML documents supplemented with JavaScript to present the data, which was served through Express. Utilizing the Model-View-Controller (MVC) architecture, individual pages were loaded upon user request. Conversely, for the admin-facing side, I utilized Angular and developed multiple components that were dynamically loaded within a single HTML document. These components were preloaded, ensuring a seamless experience for administrators to navigate the system. By avoiding the need to load and cache new pages, the relevant code was already present on the client-side, awaiting execution. On the backend, I employed MongoDB, a NoSQL database that seamlessly integrates with Node.js. MongoDB's scalability and its storage of documents in BSON format facilitated efficient conversion to JSON.

# Functionality:

To store and present data, I employed JSON as a structured format. JSON is commonly used for transmitting data between servers and clients, providing a user-friendly representation of the information. JavaScript, being a widely adopted language, was instrumental in manipulating the behavior of webpages. As mentioned earlier, MongoDB stores data in BSON, a binary representation of JSON. Consequently, data retrieval was accomplished through the MongoDB driver, followed by reformatting into JSON. Subsequently, the retrieved data was utilized in conjunction with Handlebars and TypeScript. JSON played a crucial role in bridging the gap between the backend and frontend.

I particularly appreciated the use of Handlebars for programmatic data rendering. Its simplicity and efficiency greatly contributed to streamlined code development. Similarly, within Angular, I could employ the "ngFor" directive in templates, simplifying the display of queried data with minimal code. Additionally, Angular's component-based approach proved highly efficient, enabling reuse of shared components as templates. This reusability not only enhanced productivity but also fostered clean code maintenance.

# Testing:

Maintaining robust security measures was paramount, leading us to encrypt passwords and employ hashing techniques on the admin side, rather than transmitting raw passwords to and from the database. It was essential to ensure that sensitive hash information remained protected, avoiding exposure on platforms like GitHub. Implementing interfaces for the database helped safeguard against attacks such as SQL Injection. Furthermore, permission checks were enforced to validate the user or admin's access rights before allowing specific actions via the API.

# Reflection:

Embarking on full-stack development can be challenging, given the multitude of frameworks and stacks available. However, this project offered an invaluable opportunity to work consistently within a single stack, emphasizing the importance of dedicating oneself to learning a specific library or framework. Thanks to this project, my comprehension of Node.js, MongoDB, Express, and their harmonious integration has significantly improved. I now possess a deeper understanding of how these technologies collaborate to create a versatile development environment.
