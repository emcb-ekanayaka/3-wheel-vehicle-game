# 3-wheel-vehicle-game

# 3-Wheel Vehicle Game - Unity 3D

A fun and engaging 3-wheel vehicle driving game built with Unity 3D. Collect diamonds, avoid hazards, and navigate through waypoints in this physics-based driving experience.

![Game Screenshot](https://via.placeholder.com/800x400/35424e/ffffff?text=3+Wheel+Vehicle+Game)

## Features

### Core Gameplay
- **Physics-based Vehicle Control** - Realistic 3-wheel vehicle handling
- **Diamond Collection System** - Collect coins to increase your score
- **Hazard Avoidance** - Watch out for destroyer coins that reduce your diamond count
- **Waypoint Navigation** - Follow the arrow to complete the course
- **Game Over Mechanics** - Crash into barriers to end the game

### Vehicle Physics
- Dual control systems: `Wheelhandler` (custom physics) and `SimpleCarController` (WheelCollider-based)
- Realistic acceleration, steering, and braking
- Ground sticking mechanics for terrain navigation
- Proper mass distribution and center of mass calculation

### Visual & UI
- Smooth camera follow system
- Real-time diamond counter UI
- Waypoint navigation arrow
- Wheel visual synchronization

## Project Structure

### Core Scripts

#### Vehicle Control
- **`Wheelhandler.cs`** - Custom physics-based vehicle controller
- **`SimpleCarController.cs`** - Unity WheelCollider-based controller
- **`InputHandler.cs`** - Input management and scene restart
- **`GroundStick.cs`** - Keeps vehicle grounded on terrain

#### Game Systems
- **`PlayerInventory.cs`** - Manages diamond collection and tracking
- **`InventoryUI.cs`** - Updates diamond count display
- **`WaypointManager.cs`** - Handles waypoint navigation and game completion

#### Collectibles & Hazards
- **`Coin.cs`** - Standard diamond collection
- **`DestroyerCoin.cs`** - Hazard that reduces diamond count
- **`Barrier.cs`** - Obstacles that trigger game over

#### Camera & Visuals
- **`CameraFollow.cs`** - Smooth third-person camera follow
- **Visual Wheel System** - Synchronized wheel visuals with physics

## How to Play

1. **Movement**: Use `WASD` or arrow keys to drive the vehicle
2. **Collect Diamonds**: Drive through gold coins to increase your score
3. **Avoid Hazards**: Stay away from destroyer coins (they reduce your diamonds)
4. **Follow Waypoints**: Navigate through the course using the arrow indicator
5. **Don't Crash**: Avoid barriers or the game ends
6. **Restart**: Press `R` to restart the level at any time

## Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/your-username/3-wheel-vehicle-game.git
