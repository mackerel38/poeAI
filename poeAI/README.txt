poeAI ShogiGUI package

Share this whole folder as one folder.
In ShogiGUI, add poeAI.exe from this folder.
Keep these files together:
- poeAI.exe      Windows launcher for ShogiGUI
- launcher.ini   launcher setting; Distro=default uses the default WSL distro
- poeAI          WSL/Linux USI engine
- poeAI_nn.nnue  NNUE evaluation file loaded automatically

ShogiGUI EvalFile can stay empty.
The launcher copies poeAI and poeAI_nn.nnue into WSL ~/.poeAI_shogigui_runtime before starting.
If the engine does not move, check launcher.log in this folder and confirm WSL starts with:
  wsl --exec /bin/echo ok
