# Scene Wireframes + Unity Click Path (No-Code)

## A) Create Scenes
1. Unity খুলে Project panel এ `Assets/Scenes` folder বানাও
2. File > New Scene
3. Save As:
- Boot.unity
- MainMenu.unity
- Level_001.unity

## B) Boot Scene Layout
Objects:
- Canvas
- TitleText ("Tile & Bloom")
- LoadingText ("Loading...")
- Empty GameObject: BootManager

Flow:
- Boot -> MainMenu (auto after 1 sec)

## C) MainMenu Scene Layout
Objects:
- Canvas
- LogoText
- PlayButton
- SettingsButton (optional)
- Empty GameObject: MenuManager

Flow:
- PlayButton click -> Level_001

## D) Level_001 Scene Layout
Objects:
- Canvas
- TopBar
- MovesText (e.g., Moves: 20)
- GoalText (e.g., Goal: 10)
- BoardRoot (empty container for tiles)
- BottomBar
- BoosterButton
- PauseButton
- ResultPanel (default inactive)
- ResultTitle
- RetryButton
- NextButton
- Empty GameObject: LevelManager
- Empty GameObject: FTUEManager
- Empty GameObject: AnalyticsManager

## E) Inspector Wiring Checklist
- PlayButton OnClick -> MenuManager.LoadLevel()
- RetryButton OnClick -> LevelManager.Retry()
- NextButton OnClick -> LevelManager.Next()
- ResultPanel default -> unchecked (inactive)

## F) Build Settings
1. File > Build Settings
2. Add Open Scenes in order:
0 Boot
1 MainMenu
2 Level_001
3. Platform -> Android -> Switch Platform

## G) Test Flow
- App open -> Boot
- Auto -> MainMenu
- Tap Play -> Level_001
- Win or Lose -> ResultPanel visible
