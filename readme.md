# --- README.md content ---

# Microgrid MMS Visual Model (HTML/Pyodide/Paper.js)

This is a conceptual web-based visualization model for a hybrid AC/DC mesh microgrid and its Management System (MMS). It serves as a framework to demonstrate the integration of:

* **HTML/CSS:** For the basic page structure and layout.
* **JavaScript:** To handle the loading of Pyodide and coordinate interactions.
* **Pyodide:** To execute Python code within the browser for simulation and conceptual MMS decision-making.
* **Paper.js:** For drawing, manipulating, and animating the microgrid topology on an HTML5 Canvas element.

**Note:** This project is currently a **framework** and a **work in progress**. The detailed visualization drawing in Paper.js and the comprehensive simulation/MMS logic in Python are represented by conceptual placeholders and require significant further development.

## How to Run

1.  Ensure you have the `index.html`, `README.md`, and `.gitignore` files in the same folder.
2.  Open the `index.html` file directly in a modern web browser that supports WebAssembly (most current desktop and mobile browsers do).

The page will load the necessary libraries from CDNs, initialize the canvas, and run the basic conceptual Python simulation. You will see some text output in the "MMS Control Panel & Data" area, reflecting the simulated data and decisions.

## Project Structure

* `index.html`: The main HTML file containing the structure, canvas, control panel, and embedded JavaScript/Paperscript/Pyodide code.
* `README.md`: This file, providing project information.
* `.gitignore`: Specifies files to be ignored by Git.

## Technologies Used

* HTML5 Canvas
* Paper.js (loaded via CDN: `https://cdnjs.cloudflare.com/ajax/libs/paper.js/0.12.17/paper-full.min.js`)
* Pyodide (loaded via CDN: `https://cdn.jsdelivr.net/pyodide/v0.25.0/full/pyodide.js`)
* Python (executed by Pyodide)

## Future Enhancements (TODO)

To evolve this framework into a complete visualization:

* **Detailed Paper.js Implementation:** Draw the specific components and topology of your hybrid AC/DC mesh microgrid.
* **Dynamic Visualization:** Connect the simulation data (power flow magnitude/direction, voltage levels, battery state of charge, converter status) to the Paper.js elements, updating their appearance and adding animations.
* **Refined Simulation Logic:** Enhance the Python code with more realistic microgrid models, power flow equations, and sophisticated MMS algorithms (e.g., economic dispatch, optimal power flow, voltage control, grid interaction).
* **Continuous Simulation Loop:** Implement `setInterval` or a similar mechanism in JavaScript to periodically call the Python simulation step and update the visualization.
* **User Interaction:** Add HTML controls (buttons, sliders, inputs) to allow users to interact with the simulation or MMS.
* **Separation of Concerns:** Consider separating the Python and JavaScript code into separate files for better organization as the project grows.

## License

[Add information about the project's license here, or mention that a LICENSE file will be added.]

---
*(This README provides an overview. Feel free to customize it further based on the specific details and goals of your project.)*

# --- End of README.md content ---
