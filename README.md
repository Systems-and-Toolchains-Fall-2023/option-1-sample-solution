# Team Members
- Shuying Huang (andrew id: shuyingh)
- Xiaoxi Wei (andrew id: xiaoxiw)

# Data Source
Our project uses the following dataset:
[FIFA 22 Complete Player Dataset](https://www.kaggle.com/datasets/stefanoleone992/fifa-22-complete-player-dataset)  
We only use all Men Player Data across all years to conduct the projects. The **data** folder contains all data we use.

# Dataset Schema

### Added columns
- `unique_id`: 
  - Type: Long
  - Nullable: false
  - Description: A unique identifier for each player record. This is the primary key.
  - Constraints: Must be unique for each player record (primary key). Not null.

- `year`: 
  - Type: Integer
  - Nullable: false
  - Description: The year the player data pertains to.
  - Constraints: Cannot be null. Must be a valid year between 15 - 22.

### General Features

- `sofifa_id`: 
  - Type: Integer
  - Nullable: true
  - Description: The unique identifier for each player in the SoFIFA database.

- `player_url`: 
  - Type: String
  - Nullable: true
  - Description: The URL leading to the player's profile page on the SoFIFA website.

- `short_name`: 
  - Type: String
  - Nullable: true
  - Description: The player's short name.

- `long_name`: 
  - Type: String
  - Nullable: true
  - Description: The player's full name.

- `age`: 
  - Type: Integer
  - Nullable: true
  - Description: The player's age.

- `dob`: 
  - Type: Date
  - Nullable: true
  - Description: The player's date of birth.

- `height_cm`: 
  - Type: Integer
  - Nullable: true
  - Description: The player's height in centimeters.

- `weight_kg`: 
  - Type: Integer
  - Nullable: true
  - Description: The player's weight in kilograms.

- `nationality_id`: 
  - Type: Integer
  - Nullable: true
  - Description: The identifier for the player's national team.

- `nationality_name`: 
  - Type: String
  - Nullable: true
  - Description: The name of the player's nationality.

- `preferred_foot`: 
  - Type: String
  - Nullable: true
  - Description: The player's preferred foot (left/right).

- `real_face`: 
  - Type: String
  - Nullable: true
  - Description: Indicates if the player has a real face scan in the game (yes/no).

- `player_face_url`: 
  - Type: String
  - Nullable: true
  - Description: The URL of the player's face image.

### Performance Features

- `overall`: 
  - Type: Integer
  - Nullable: true
  - Description: The player's overall rating.

- `potential`: 
  - Type: Integer
  - Nullable: true
  - Description: The player's potential rating.

- `value_eur`: 
  - Type: Double
  - Nullable: true
  - Description: The player's market value.

- `wage_eur`: 
  - Type: Double
  - Nullable: true
  - Description: The player's weekly wage.

- `release_clause_eur`: 
  - Type: String
  - Nullable: true
  - Description: The player's release clause amount.

- `international_reputation`: 
  - Type: Integer
  - Nullable: true
  - Description: The player's international reputation on a 1-5 scale.
  - Constraints: Value must be an integer between 1 and 5 (inclusive).

- `weak_foot`: 
  - Type: Integer
  - Nullable: true
  - Description: The player's weak foot proficiency on a 1-5 scale.
  - Constraints: Value must be an integer between 1 and 5 (inclusive).

- `skill_moves`: 
  - Type: Integer
  - Nullable: true
  - Description: The number of skill moves the player is capable of.

- `work_rate`: 
  - Type: String
  - Nullable: true
  - Description: The player's work rate (e.g., High/ Low, Medium/ High).

- `body_type`: 
  - Type: String
  - Nullable: true
  - Description: The player's body type (e.g., Stocky, Normal, Lean).

- `player_positions`: 
  - Type: String
  - Nullable: true
  - Description: The positions the player is capable of playing in.

### Skill Features

- `pace`, `shooting`, `passing`, `dribbling`, `defending`, `physic`:
  - Type: Integer
  - Nullable: true
  - Description: The player's core skill features.

- `attacking_crossing`, `attacking_finishing`, `attacking_heading_accuracy`, `attacking_short_passing`, `attacking_volleys`, `skill_dribbling`, `skill_curve`, `skill_fk_accuracy`, `skill_long_passing`, `skill_ball_control`:
  - Type: Integer
  - Nullable: true
  - Description: The player's detailed attacking and skill features.

- `movement_acceleration`, `movement_sprint_speed`, `movement_agility`, `movement_reactions`, `movement_balance`:
  - Type: Integer
  - Nullable: true
  - Description: The player's movement skill features.

- `power_shot_power`, `power_jumping`, `power_stamina`, `power_strength`, `power_long_shots`:
  - Type: Integer
  - Nullable: true
  - Description: The player's power features.

- `defending_marking_awareness`, `defending_standing_tackle`, `defending_sliding_tackle`:
  - Type: Integer
  - Nullable: true
  - Description:The player's defending skill features.

### Others  

- `mentality_aggression`, `mentality_interceptions`, `mentality_positioning`, `mentality_vision`, `mentality_penalties`, `mentality_composure`:
  - Type: Integer
  - Nullable: true
  - Description: These relate to mental aspects of the players.  
  
- `goalkeeping_diving`, `goalkeeping_handling`, `goalkeeping_kicking`, `goalkeeping_positioning`, `goalkeeping_reflexes`, `goal`
  - Type: Integer
  - Nullable: true
  - Description:These relate to goal aspects of the players.
