<p align="center">
  <img src="https://github.com/user-attachments/assets/f5b4aa83-8052-4bc3-9347-ea994051a959" alt="logo" width="500" />
</p>

## Overview
The **Pokemon Pokedex Application** is a web-based application that allows users to log in or create an account to explore a detailed Pokedex. Users can look up Pokemon, view their stats, pictures, and types, and add individual Pokemon to their roster.

## Features
- **User Authentication**: Users can log in or create an account to access the Pokedex.
- **Pokemon Lookup**: Search for Pokemon to view their:
  - Picture
  - Stats
  - Type(s)
- **Roster Management**: Users can select Pokemon and add them to their personal roster.

## Technologies Used
- **Backend**: Python, Flask
- **Frontend**: HTML, CSS
- **Database**: PostgreSQL
- **Containerization**: Docker

## Setup Instructions

### Installation
1. **Clone the Repository**:
   ```bash
   git clone <repository-url>
   cd Pokemon
   ```

2. **Set Up Virtual Environment** (optional but recommended):
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. **Install Dependencies**:
   ```bash
   pip install -r requirements.txt
   ```

4. **Set Up Database**:
   - Ensure PostgreSQL is installed and running.
   - Create a database and configure the connection string in `config.py` or your environment variables.
   - Initialize the database by running the provided SQL scripts or database migration tools.
   ```bash
   flask db upgrade  # If using Flask-Migrate
   ```

5. **Run the Application**:
   ```bash
   flask run
   ```
   - The application will be available at: `http://localhost:5000`

### Using Docker
1. **Build the Docker Image**:
   ```bash
   docker compose up
   ```

2. **Run the Container**:
   ```bash
   docker run -p 5020:5000 pokemon
   ```
   - The application will be accessible at `http://localhost:5020`.

3. **Stop the Container**:
   ```bash
   docker ps
   docker stop <container-id>
   ```

### Configuration
- Configure your PostgreSQL database connection string in `config.py` or the environment variables.

## Usage
1. Visit the homepage and log in or create a new account.
2. View detailed information about each Pokemon, including their picture, stats, and type(s).
3. Add desired Pokemon to your roster by clicking the "Add to Roster" button.
4. Access your roster to view all selected Pokemon.


## Future Enhancements
- **Battle Simulation**: Add a feature to simulate battles between rosters.
- **Team Recommendations**: Suggest optimal team compositions based on Pokemon stats and types.
- **Advanced Search**: Include filters for abilities, stats, and evolutions.


## License
This project is licensed under the MIT License. See the LICENSE file for details.

---



