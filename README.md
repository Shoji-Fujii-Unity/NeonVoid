# NEON VOID: Pocket FPS

## 日本語

### 概要

NEON VOID: Pocket FPS は、PCとスマートフォンで遊べる簡易3Dファーストパーソン・シューティングゲームです。
画面は横長で遊ぶことを前提にしています。
サウンドのON/OFF、多言語表示、ローカル保存に対応しています。

### ファイル

- index.html  
  ゲーム本体。ブラウザで開くとそのまま遊べます。

- README.md  
  この説明文。

### 動作環境

- PCブラウザ
- Androidブラウザ
- iOS Safari
- WebGLが有効なブラウザ

Three.jsを外部CDNから読み込んでいます。
初期状態ではネットワーク接続が必要です。
完全オフラインで運用する場合は、three.min.jsをプロジェクト内に置き、index.html内の読み込み先をローカルファイルへ変更してください。

### 起動方法

1. index.html をブラウザで開きます。
2. 横長画面のまま、ゲーム開始を選択します。
3. 言語とサウンド設定を必要に応じて変更してから開始できます。

### 遊び方

モンスターを倒してスコアを稼ぎます。
一定時間生存するとステージとウェーブが上がります。
HPが0になるとゲームオーバーです。

### 操作

PC:

- WASD: 移動
- 矢印キー: 移動
- マウス: 視点移動
- 左クリック: 射撃
- Space: 射撃
- ESC または P: 一時停止

スマートフォン:

- 左下スティック: 移動
- 右側画面をドラッグ: 視点移動
- FIREボタン: 射撃
- 右上ボタン: 一時停止

### 対応言語

- 日本語
- English
- 中文
- Español

言語設定はメニューおよび一時停止画面から変更できます。

### サウンド

ゲーム開始画面、一時停止画面からサウンドをON/OFFできます。
ブラウザの自動再生制限により、最初のタップまたはクリックの後で音が鳴る場合があります。

### セーブデータ

ローカルストレージに保存します。

保存される内容:

- 選択中の言語
- サウンド設定
- ハイスコア
- 累計キル数

ブラウザのサイトデータ消去やキャッシュ削除を行うと、セーブデータは消えます。

### ステージ

ゲームは全8ステージ構成です。
ステージは進行時間に応じて自動的に切り替わります。

1. NEON GRID
2. CRYSTAL MAZE
3. MAGMA CORE
4. VOID SPIRE
5. FROST LATTICE
6. ABYSS DOME
7. CIRCUIT LAB
8. ENDLESS

### モンスター

敵はすべてモンスターです。
種類によって強さ、移動方法、攻撃性質が異なります。

- Crawler: 地面を跳ねるように移動する小型敵
- Wraith: 壁をすり抜け、浮遊する敵
- Spider: 高速で近寄る多脚敵
- Flayer: 空を飛ぶ高機動敵
- Brute: 高HPの大型敵

### 画面表示

- SCORE: スコア
- WAVE: ウェーブ
- STAGE: 現在のステージ
- TIME: 生存時間
- HP: プレイヤーの残り体力

ステージ開始時にはステージ名が画面中央に表示されます。

### トラブルシューティング

画面が縦長になる:
スマートフォンでは横表示でプレイしてください。

メニューが隠れる:
横長画面前提で上下スクロールできます。
必要に応じて端末を横に向けてください。

Three.jsの読み込みに失敗する:
ネットワーク接続を確認してください。
オフライン環境ではThree.jsをローカルへ配置してindex.htmlの読み込みパスを変更してください。

音が鳴らない:
サウンド設定がONになっているか確認してください。
ブラウザの音声許可や静音モードを解除してください。

---

## English

### Overview

NEON VOID: Pocket FPS is a lightweight 3D first-person shooter for PC and mobile browsers.
The game is designed to be played in landscape mode.
It supports sound on/off, multilingual UI, and local save data.

### Files

- index.html  
  The game itself. Open it in a browser to play.

- README.md  
  This documentation.

### Requirements

- PC browser
- Android browser
- iOS Safari
- WebGL enabled

This project loads Three.js from a CDN by default.
Internet access is required unless you bundle three.min.js locally and update the script source in index.html.

### How to Start

1. Open index.html in a browser.
2. Keep the display in landscape.
3. Optional: change language and sound settings.
4. Start the game.

### Gameplay

Fight monsters, earn score, and survive as long as possible.
The game advances through waves and stages as time passes.
The game ends when HP reaches 0.

### Controls

PC:

- WASD: move
- Arrow keys: move
- Mouse: look
- Left click: shoot
- Space: shoot
- ESC or P: pause

Mobile:

- Left stick: move
- Drag on the right side: look
- FIRE button: shoot
- Top-right button: pause

### Languages

- Japanese
- English
- Chinese
- Spanish

Language can be changed from the menu and pause screen.

### Sound

Sound can be toggled on/off from the start screen and pause screen.
Due to browser autoplay restrictions, audio may start only after the first tap or click.

### Save Data

Saved in local storage.

Stored:

- Selected language
- Sound setting
- High score
- Total kills

Deleting site data or browser storage will remove the save data.

### Stages

The game contains 8 stages.
Stages change automatically as the game progresses.

1. NEON GRID
2. CRYSTAL MAZE
3. MAGMA CORE
4. VOID SPIRE
5. FROST LATTICE
6. ABYSS DOME
7. CIRCUIT LAB
8. ENDLESS

### Enemies

All enemies are monsters.
Each type has different movement and combat behavior.

- Crawler: small hopping enemy
- Wraith: floating enemy that can pass through walls
- Spider: fast multi-legged enemy
- Flayer: flying high-speed enemy
- Brute: large high-HP enemy

### HUD

- SCORE: current score
- WAVE: current wave
- STAGE: current stage
- TIME: survival time
- HP: player health

Stage names appear briefly at stage start.

### Troubleshooting

Screen is portrait:
Use landscape mode on mobile.

Menu is hidden:
The menu scrolls vertically and is designed for landscape. Rotate the device if needed.

Three.js failed to load:
Check the network connection. For offline use, place Three.js locally and update the script path in index.html.

No sound:
Make sure sound is enabled and browser audio permissions are allowed.

---

## 中文

### 概述

NEON VOID: Pocket FPS 是一款可在 PC 和手机浏览器中游玩的简易 3D 第一人称射击游戏。
游戏默认采用横屏界面。
支持声音开关、多语言界面和本地存档。

### 文件

- index.html  
  游戏本体，直接用浏览器打开即可。

- README.md  
  本说明文件。

### 运行环境

- PC 浏览器
- Android 浏览器
- iOS Safari
- 支持 WebGL 的浏览器

项目默认从 CDN 加载 Three.js。
初始状态下需要联网。
若需要完全离线运行，请将 three.min.js 放到本地目录，并修改 index.html 中的引用路径。

### 开始方法

1. 用浏览器打开 index.html。
2. 保持横屏显示。
3. 可按需要修改语言和声音设置。
4. 开始游戏。

### 玩法

击杀怪物、获得分数、尽可能长时间生存。
随着时间推进，波次和关卡会提升。
HP 归零后游戏结束。

### 操作

PC:

- WASD：移动
- 方向键：移动
- 鼠标：视角
- 左键：射击
- Space：射击
- ESC 或 P：暂停

手机:

- 左下摇杆：移动
- 右侧拖拽：视角
- FIRE 按钮：射击
- 右上按钮：暂停

### 支持语言

- 日本語
- English
- 中文
- Español

可在主菜单和暂停界面切换语言。

### 声音

主菜单和暂停界面可切换声音开关。
由于浏览器自动播放限制，首次点击或触摸后才会播放声音。

### 存档

数据保存在浏览器本地存储中。

保存内容：

- 当前语言
- 声音设置
- 最高分
- 累计击杀数

删除浏览器站点数据后，存档会消失。

### 关卡

游戏共有 8 个关卡。
随着游戏进行会自动切换关卡。

1. NEON GRID
2. CRYSTAL MAZE
3. MAGMA CORE
4. VOID SPIRE
5. FROST LATTICE
6. ABYSS DOME
7. CIRCUIT LAB
8. ENDLESS

### 怪物

所有敌人都是怪物。
不同类型在强度、移动和攻击方式上不同。

- Crawler：小型跳跃敌人
- Wraith：可穿墙的浮空敌人
- Spider：高速多足敌人
- Flayer：高机动飞行敌人
- Brute：高生命值大型敌人

### 界面

- SCORE：当前分数
- WAVE：当前波次
- STAGE：当前关卡
- TIME：生存时间
- HP：玩家体力

关卡开始时会短暂显示关卡名。

### 故障处理

画面是竖屏：
手机请使用横屏。

菜单被遮挡：
菜单支持上下滚动，并针对横屏优化。必要时请旋转设备。

Three.js 加载失败：
检查网络连接。离线环境请将 Three.js 放到本地并修改 index.html 引用。

没有声音：
确认声音设置为开，并允许浏览器播放声音。

---

## Español

### Resumen

NEON VOID: Pocket FPS es un juego FPS 3D sencillo para PC y navegadores móviles.
Está diseñado para jugarse en modo horizontal.
Admite sonido activado/desactivado, interfaz multilenguaje y guardado local.

### Archivos

- index.html  
  El juego. Ábrelo en un navegador para jugar.

- README.md  
  Esta documentación.

### Requisitos

- Navegador de PC
- Navegador Android
- iOS Safari
- Navegador con WebGL

El proyecto carga Three.js desde un CDN por defecto.
Se necesita conexión a Internet salvo que uses three.min.js local y modifiques la ruta del script en index.html.

### Cómo empezar

1. Abre index.html en un navegador.
2. Mantén la pantalla en horizontal.
3. Opcional: cambia idioma y sonido.
4. Inicia el juego.

### Jugabilidad

Derrota monstruos, consigue puntos y sobrevive el mayor tiempo posible.
Las oleadas y niveles avanzan con el tiempo.
El juego termina cuando el HP llega a 0.

### Controles

PC:

- WASD: moverse
- Flechas: moverse
- Ratón: mirar
- Clic izquierdo: disparar
- Space: disparar
- ESC o P: pausa

Móvil:

- Stick izquierdo: moverse
- Arrastrar en la derecha: mirar
- BOTÓN FIRE: disparar
- Botón superior derecho: pausa

### Idiomas

- 日本語
- English
- 中文
- Español

El idioma se cambia desde el menú y la pantalla de pausa.

### Sonido

El sonido puede activarse o desactivarse desde el menú y la pausa.
Por restricciones de autoplay del navegador, el audio puede empezar después del primer toque o clic.

### Datos guardados

Se guardan en almacenamiento local.

Se guarda:

- Idioma seleccionado
- Configuración de sonido
- Puntuación máxima
- Total de eliminaciones

Si borras los datos del navegador, la partida guardada desaparece.

### Niveles

El juego tiene 8 niveles.
Los niveles cambian automáticamente según el avance.

1. NEON GRID
2. CRYSTAL MAZE
3. MAGMA CORE
4. VOID SPIRE
5. FROST LATTICE
6. ABYSS DOME
7. CIRCUIT LAB
8. ENDLESS

### Enemigos

Todos los enemigos son monstruos.
Cada tipo tiene movimiento y comportamiento distintos.

- Crawler: enemigo pequeño que salta
- Wraith: enemigo flotante que atraviesa paredes
- Spider: enemigo multi-patas rápido
- Flayer: enemigo volador de alta velocidad
- Brute: enemigo grande con mucha vida

### Interfaz

- SCORE: puntos actuales
- WAVE: oleada actual
- STAGE: nivel actual
- TIME: tiempo sobrevivido
- HP: salud del jugador

El nombre del nivel aparece brevemente al cambiar de nivel.

### Solución de problemas

La pantalla está en vertical:
Usa modo horizontal en el móvil.

El menú se oculta:
El menú se desplaza verticalmente y está optimizado para horizontal. Gira el dispositivo si es necesario.

No carga Three.js:
Revisa la conexión. Para uso sin Internet, coloca Three.js localmente y cambia la ruta en index.html.

No hay sonido:
Comprueba que el sonido esté activado y permite el audio en el navegador.