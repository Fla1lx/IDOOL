# IDOOL MVP Plan

## MVP Goal

Create a playable mobile idle / tycoon prototype where the player manages an auto repair shop, completes simple repairs, earns money, and upgrades the workshop to process cars faster and earn more.

The MVP should answer one main question: is the core loop satisfying enough to continue expanding the game?

## Core Game Loop

Car arrives -> repair starts -> repair timer runs -> money is earned -> workshop is upgraded -> the next repairs become faster or more profitable.

## Minimum MVP Systems

- Money as the main soft currency.
- Car queue with a small number of incoming cars.
- One repair bay where a car can be serviced.
- Repair timer that blocks the bay until work is complete.
- Workshop upgrades that improve speed, income, or queue capacity.
- Progress saving so money and upgrades persist between sessions.

## Development Stages

### Stage 1: Repository and Planning

- Prepare Unity-friendly repository files.
- Add README and MVP documentation.
- Confirm ignore rules for generated Unity folders and build outputs.

### Stage 2: Unity Project Setup

- Create or open the Unity project through Unity Hub.
- Configure mobile-oriented project settings.
- Add the first scene: `MainGame`.
- Set up basic folders under `Assets` for scripts, prefabs, scenes, UI, and art.

### Stage 3: Core Loop Prototype

- Spawn a car into the queue.
- Move a car into the repair bay.
- Start and complete a repair timer.
- Award money after repair completion.
- Show current money in UI.

### Stage 4: Upgrades and Balance

- Add upgrade buttons for repair speed and repair reward.
- Increase upgrade prices after each purchase.
- Tune the first 10-15 minutes of progression.
- Add simple feedback for completed repairs and purchased upgrades.

### Stage 5: Save and MVP Polish

- Save money, upgrade levels, and active repair state.
- Restore progress on app start.
- Add minimal mobile UI polish.
- Test the loop on a mobile aspect ratio.
