# Project Structure – Meeting Management System

## 1. Project Overview

The Meeting Management System is a Python application developed using Object-Oriented Programming (OOP) principles.

The project is organized into separate modules to improve code readability, maintainability, and scalability.

Its main purpose is to manage organizational meetings, meeting minutes, participants, suggestions, and keywords.

## 2. Directory Structure

```text
gestao-reunioes/
│
├── docs/
│   ├── ESTRUTURA.md
│   ├── REGRAS_DE_NEGOCIO.md
│   └── DIAGRAMA_UML.md
│
├── src/
│   ├── models/
│   ├── services/
│   ├── views/
│   └── main.py
│
├── README.md
└── .gitignore
```

## 3. Modules and Responsibilities

### Models

The `models/` directory contains the classes responsible for representing the system entities.

Classes:

- `Pessoa`: Base class representing a person.
- `Funcionario`: Represents an organization's employee.
- `ParticipanteExterno`: Represents an external participant.
- `Reuniao`: Represents an organizational meeting.
- `Ata`: Represents the meeting minutes.
- `ParticipanteReuniao`: Represents the relationship between participants and meetings.
- `Sugestao`: Stores suggestions submitted by participants.
- `PalavraChave`: Represents keywords associated with meeting minutes.

### Services

The `services/` directory contains the business logic and validation rules.

Responsibilities:

- Validate participant quantities.
- Validate keyword quantities.
- Manage meeting minutes status.
- Control document visibility.
- Manage approvals and suggestions.

### Views

The `views/` directory contains the user interface and interaction menus.

Responsibilities:

- Display the main menu.
- Provide registration options.
- Provide search and consultation options.
- Allow information updates.

### Main

The `main.py` file is the application's entry point.

It initializes the application and provides access to the main menu.

## 4. Object-Oriented Programming

The project applies the following OOP concepts:

- **Encapsulation:** Protecting object attributes and controlling access through methods.
- **Inheritance:** `Funcionario` and `ParticipanteExterno` inherit from `Pessoa`.
- **Polymorphism:** Different person types can be handled through a common interface.
- **Abstraction:** Representing real-world entities through classes and objects.

## 5. Business Rules

The system follows these requirements:

| Rule | Requirement |
|---|---|
| Participants | Minimum 2 and maximum 10 per meeting minutes document. |
| Issuer | Must be included among the participants. |
| Keywords | Minimum 1 and maximum 5 per document. |
| Visibility | Public by default, with an option to become private. |
| Initial status | Issued (`Emitida`). |
| Final status | Completed (`Concluída`). |

## 6. Documentation

The `docs/` directory contains the project's technical documentation:

- `ESTRUTURA.md`: Project architecture and directory organization.
- `REGRAS_DE_NEGOCIO.md`: Business rules and validations.
- `DIAGRAMA_UML.md`: UML class diagram and relationships.

## 7. Final Considerations

This architecture aims to maintain a clear separation of responsibilities, encourage code reuse, and apply Object-Oriented Programming principles throughout the application.