<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <title>Piano HTML CSS</title>
    <link rel="stylesheet" href="style.css">
</head> 
<body>
  
<h1 style="text-align: center; color : black; background : linear-gradient(to right, black, white); border: 3px solid #2C3E50; font-family: Arial;">Projet Piano</h1>
<div class="piano">
<!-- Les 88 touches du piano -->  

<div class="touche blanche">A0</div>
<div class="touche noire">A#0</div>
<div class="touche blanche">B0</div>
<div class="touche blanche">C1</div>
<div class="touche noire">C#1</div>
<div class="touche blanche">D1</div>
<div class="touche noire">D#1</div>
<div class="touche blanche">E1</div>
<div class="touche blanche">F1</div>
<div class="touche noire">F#1</div>
<div class="touche blanche">G1</div>
<div class="touche noire">G#1</div>
<div class="touche blanche">A1</div>
<div class="touche noire">A#1</div>
<div class="touche blanche">B1</div>
<div class="touche blanche">C2</div>
<div class="touche noire">C#2</div>
<div class="touche blanche">D2</div>
<div class="touche noire">D#2</div>
<div class="touche blanche">E2</div>
<div class="touche blanche">F2</div>
<div class="touche noire">F#2</div>
<div class="touche blanche">G2</div>
<div class="touche noire">G#2</div>
<div class="touche blanche">A2</div>
<div class="touche noire">A#2</div>
<div class="touche blanche">B2</div>
<div class="touche blanche">C3</div>
<div class="touche noire">C#3</div>
<div class="touche blanche">D3</div>
<div class="touche noire">D#3</div>
<div class="touche blanche">E3</div>
<div class="touche blanche">F3</div>
<div class="touche noire">F#3</div>
<div class="touche blanche">G3</div>
<div class="touche noire">G#3</div>
<div class="touche blanche">A3</div>
<div class="touche noire">A#3</div>
<div class="touche blanche">B3</div>
<div class="touche blanche">C4</div>
<div class="touche noire">C#4</div>
<div class="touche blanche">D4</div>
<div class="touche noire">D#4</div>
<div class="touche blanche">E4</div>
<div class="touche blanche">F4</div>
<div class="touche noire">F#4</div>
<div class="touche blanche">G4</div>
<div class="touche noire">G#4</div>
<div class="touche blanche">A4</div>
<div class="touche noire">A#4</div>
<div class="touche blanche">B4</div>
<div class="touche blanche">C5</div>
<div class="touche noire">C#5</div>
<div class="touche blanche">D5</div>
<div class="touche noire">D#5</div>
<div class="touche blanche">E5</div>
<div class="touche blanche">F5</div>
<div class="touche noire">F#5</div>
<div class="touche blanche">G5</div>
<div class="touche noire">G#5</div>
<div class="touche blanche">A5</div>
<div class="touche noire">A#5</div>
<div class="touche blanche">B5</div>
<div class="touche blanche">C6</div>
<div class="touche noire">C#6</div>
<div class="touche blanche">D6</div>
<div class="touche noire">D#6</div>
<div class="touche blanche">E6</div>
<div class="touche blanche">F6</div>
<div class="touche noire">F#6</div>
<div class="touche blanche">G6</div>
<div class="touche noire">G#6</div>
<div class="touche blanche">A6</div>
<div class="touche noire">A#6</div>
<div class="touche blanche">B6</div>
<div class="touche blanche">C7</div>
<div class="touche noire">C#7</div>
<div class="touche blanche">D7</div>
<div class="touche noire">D#7</div>
<div class="touche blanche">E7</div>
<div class="touche blanche">F7</div>
<div class="touche noire">F#7</div>
<div class="touche blanche">G7</div>
<div class="touche noire">G#7</div>
<div class="touche blanche">A7</div>
<div class="touche noire">A#7</div>
<div class="touche blanche">B7</div>
<div class="touche blanche">C8</div>
</div>
------------------------------------------------------------------------------------

html {
  height: 100%;
}
@media (max-width: 600px) {
  .blanche { height: 30vw; }
  .noire   { height: 18vw; }
}
body {
  background-color: #8B5CF6;
}
.piano {
  display: flex;
  width: 100%;
  margin-top: 250px;
}

.touche {
  box-sizing: border-box;
}

.blanche {
  flex: 1;
  height: 15vw;
  background-color: white;
  border: 1px solid black;
  border-radius: 0 0 4px 4px;
}

.noire {
  width: 1.15%;
  height: 8.5vw;
  background-color: black;
  border-radius: 0 0 3px 3px;
  margin-left: -0.575%;
  margin-right: -0.575%;
  z-index: 1;
}
/*blablablaaaaaaaaaaaaa*/

.blanche:hover {
  background-color: #e0e0e0;
  height: 13.7vw;
}

.noire:hover {
  background-color: #444;
}

.blanche:active {
  background-color: #ccc;
  transform: translateY(2px);
}

.blanche {
  display: flex;
  align-items: flex-end;
  justify-content: center;
  font-size: 0.8vw;
  color: #555;
}

.piano {
  padding: 10px;
  background: linear-gradient(to bottom, #5a3825, #2b1a10);
  border-radius: 8px;
  box-shadow: 0 10px 30px rgba(0, 0, 0, 0.5);
}

h1 {
  animation: pulse 2s infinite;
}

@keyframes pulse {
  0%   { opacity: 1; }
  50%  { opacity: 0.6; }
  100% { opacity: 1; }
}

.blanche:nth-child(odd) {
  animation-delay: 0.2s;
}

.touche.noire {
    font-size: 9px;
    color: white;
    display: flex;
    justify-content: center;
    align-items: flex-end;
    padding-bottom: 8px;
    box-sizing: border-box;
    white-space: nowrap;
    overflow: hidden;
}
.touche.blanche {
    font-size: 12px;
    display: flex;
    justify-content: center;
    align-items: flex-end;
    padding-bottom: 10px;
    box-sizing: border-box;
}
.touche.noire {
    writing-mode: vertical-rl;
    font-size: 9px;
    padding: 5px 0;
}


</body>
</html>
