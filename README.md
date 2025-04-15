# Overview

The **Ursina Engine** is a framework that uses the Python language. It allows developers to create both 2D and 3D projects. It is mainly used to create games. It is free and is licensed under the Massachusetts Institute of Technology|MIT license. In addition to games, it can also be used to create apps and simulations. The engine is available for Microsoft Windows, Linux, and MacOS (not officially supported).

There is also a community-created Android port:

https://github.com/PaologGithub/UrsinaForMobile/

----

# Installation

Install the latest **major** version of ursina via the pip command:

<code>pip install ursina</code>

Install the latest version of ursina from GitHub:

<code>pip install https://github.com/pokepetter/ursina/archive/master.zip</code>

Keep in mind that installing from the latest GitHub version may introduce new features or changes that could potentially break existing code.

----
# Features

**Structure**:

A regular project contains these features: 
<code>
from ursina import *

app = Ursina() #‎ Generates the Ursina window 

def update(): #‎ Function called every frame

   ... 

def input(key): #‎ Called when a key is pressed

   ...

app.run() #‎ Creates the window 
</code>

**Entities**:<br>Ursina is an entity-based engine. An entity is a Python class that acts as an object in Ursina, similar to the GameObject in Unity.<br>It can have a position, a rotation, a scale, a model, a texture, a color, a shader, a parent, ...<br>Scripts apply a behavior to the entity.

Each entity can have its own update function, that is executed each frame and an input function (executed when a key is pressed).<br>More attributes of an entity are shown here: https://www.ursinaengine.org/api_reference.html#Entity API Reference https://www.ursinaengine.org/entity_basics.html Entity Basics<br>

**Collisions and Colliders**:<br>Ursina can handle collisions when a collider is applied to an entity.<br>Alternatively, the functions <code>raycast</code> and <code>boxcast</code> can be used.<br />

**Prefabs**:<br>You can use ursina's prefabs. For example, there's a first person controller (<code>from ursina.prefabs.first_person_controller import FirstPersonController</code>), a color picker (<code>from ursina.prefabs.color_picker import ColorPicker</code>), a checkbox system (<code>from ursina.prefabs.checkbox import CheckBox</code>), a screen recorder (<code>from ursina.prefabs.video_recorder import VideoRecorder</code>), a particle system (<code>from ursina.prefabs.particle_system import ParticleSystem</code>), a file browser (<code>from ursina.prefabs.file_browser import FileBrowser</code>), a grid editor (<code>from ursina.prefabs.grid_editor import GridEditor</code>), an ascii editor (<code>from ursina.prefabs.ascii_editor import ASCIIEditor</code>), etc.

**Other useful tools and features**:<br>Networking:<br>Ursina has a built-in module networking module: from ursina.networking import *<br>Physics Engine:<br>Ursina has a built-in physics engine (from ursina.physics import *), yet not finished.<br>

**Level Editor (Beta Preview)**:<br>Ursina's level editor is currently in beta preview. Import it via:

<code>

from ursina import *

from ursina.editor.level_editor import LevelEditor

app = Ursina()

editor = LevelEditor()

app.run()

</code>

![](https://upload.wikimedia.org/wikipedia/commons/b/bd/Ursina_level_editor_screenshot.png) 

The trailer is accessible https://www.youtube.com/watch?v=37vLHB5PRTw&t=25s here. 

----

# Notable Projects

• **Dustred** by https://github.com/pokepetter pokepetter (Petter Amland, ursina's creator). Here's the code: https://github.com/pokepetter/red_planet GitHub Code<br /> or play it in the browser (web version created with taptapir*): https://pokepetter.github.io/red_planet/dustred Play Dustred.

• **Phalanger** by SLHIDE™. https://slhide.free.nf/phalanger.php Play Phalanger (Android, requires creating an account on their website).

• **Rally** by https://mandaw2014.itch.io Mandaw, Desktop https://mandaw2014.itch.io/rally Play Rally

And many more on https://itch.io/games/tag-ursina Itch.io.

ㅤㅤ*engine created by ursina's developer for creating browser games

----

# Fun facts

• ursina is over 7 years old, its birthday is the 07/9/2017<br>
• the old name for ursina's Entity was "Thing", see the GitHub edit history

----

# Other Websites
* https://www.ursinaengine.org/ Official website
* https://www.ursinaengine.org/documentation.html Full Documentation
