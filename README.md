Project Overview
This is a Java-based web application for an RPG (Role-Playing Game) admin panel. It's built using the Spring MVC framework and follows a standard layered architecture.

Key Technologies:
Java 8: The core programming language
Spring MVC 5.2.3: Web framework for handling HTTP requests
Maven: Build and dependency management
Thymeleaf 3.0.15: Template engine for the frontend
jQuery: JavaScript library for frontend functionality
Project Structure:
Entity Layer:
Player: Main entity with attributes like name, title, race, profession, level, etc.
Race: Enum with options like HUMAN, DWARF, ELF, GIANT, ORC, TROLL, HOBBIT
Profession: Enum with options like WARRIOR, ROGUE, SORCERER, CLERIC, etc.
Repository Layer:
PlayerRepository: Handles data access operations using an in-memory list of players
Service Layer:
PlayerService: Contains business logic for player management
Controller Layer:
PlayerController: REST controller exposing endpoints for CRUD operations
PlayerInfo: DTO (Data Transfer Object) for player data
Frontend:
Simple HTML page with jQuery for an admin panel interface
CSS for styling
Functionality:
List all players with pagination
Get count of all players
Create new players with validation
Update existing players
Delete players
The application is a simple admin panel for managing player accounts in an RPG game. The frontend is minimal, with just a basic HTML structure for the admin panel. The backend is more developed with a complete REST API for player management.

The data is currently stored in-memory (not in a database), using a CopyOnWriteArrayList with sample player data already populated.
