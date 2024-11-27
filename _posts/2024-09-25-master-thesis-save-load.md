---
background: /img/SaveLoadBackgound.png
background-color: aquamarine
layout: post
subtitle: Master Thesis project at HTW Berlin, Germany
---

<br>
## Project Details
Project-Type: student project
<br> Team Size: 1
<br> Time/Effort: 18 weeks full time including writing the thesis



## Framework Details
The Save System is a robust and versatile Unity tool for reliably saving game data. It uses JSON serialization to ensure platform-agnostic compatibility, enabling seamless data transfer across environments. A standout feature is its ability to handle complex object references, including nested and circular dependencies, ensuring accurate restoration of game states and dynamic reloading of prefabs. Supporting a wide range of data types, from simple variables to intricate object graphs, the system adapts to diverse game structures. With multiple saving methods, such as Attribute Saving and the ISavable interface, the system offers developers the flexibility to implement and customize efficient saving processes for games of varying complexity.


### Interface Saving
The **ISavable interface** allows Unity components, especially MonoBehaviour objects, to be saved and loaded with customized logic. This approach is ideal for scenarios requiring specialized save logic or handling references and dependencies dynamically. It provides two main methods:

- **OnSave**: Defines how the object's state is serialized.
- **OnLoad**: Reconstructs the object's state from saved data.

<img src="/img/interface-saving.png" alt="Unity Save and Load System" style="width: 100%; max-width: 100%; height: auto;" />


### Attribute Saving
**Attribute Saving** simplifies marking specific data for persistence using a declarative approach with attibutes:

- **[Savable]**: Marks individual fields or properties for saving.
- **[SavableObject]**: Automatically marks all fields and properties in a class for saving.

<img src="/img/attribute-saving.png" alt="Unity Save and Load System" style="width: 100%; max-width: 100%; height: auto;" />



## Links
GitHub: <a href="https://github.com/AyuCalices/MasterThesisSaveLoad" style="color: LightGray; text-decoration: underline; ">Save and Load System</a>
<br> Documentation: <a href="https://docs.google.com/document/d/10DOlMv5Di8w_ab0zSgxro_A_cU-crEhKx7GGj3WdMTQ/edit?usp=sharing" style="color: LightGray; text-decoration: underline; ">Google Docs</a>
<br> Thesis: <a href="\pdf\MasterThesis_Jaspers_Robin.pdf" style="color: LightGray; text-decoration: underline; ">PDF</a>