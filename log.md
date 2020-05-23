# 100 Days Of Code - Log (Round 5)

## R5-D57: May 22, 2020 - Friday

**Today's Progress:**  
- NovaForge
  - Fixed Restart funtionality: in game clouds disappear and camera resets
- Covid-19 (Coronavirus) Analytics
  - Updated stats for the day as usual

**Thoughts:**  
Another one that Unity made Unnecessarily complex.  They somehow don't have a way to set the position (Transform) of a gameobject or Camera.  So if you want to simply move something to a specific location, a simple line like `camera.transform.position = newPosition;` doesn't work.  

After Googling it and seeing all the other comments, this is a problem that so many people run into, and setting positions is such a fundamental part of a game that you would think this would be fixed by now.  But even with all it's flaws, Unity is 100x better than when you had to basically do everything on your own 15 years ago.

So even though this cost me another few hours, I figured it out in the end and next time will be that much easier.

**Link(s) to work:**
1. [NovaForge - Fixed Restart funtionality: in game clouds disappear and camera resets](https://github.com/BrianLeip/NovaForge/commit/8984752bb581de84ef32130f97d55156db4a8237)
2. [Covid-19 Analytics - Updated stats for the day](https://github.com/BrianLeip/Covid19_Analytics/blob/47d512b79880da66383105dc265892c2a6d66e2d/Covid19_Analytics.ipynb)

---
## R5-D56: May 21, 2020 - Thursday

**Today's Progress:**  
- NovaForge
  - Worked on setting the in-game element cloud colors. Unity makes this extraordinarily complicated to do.  Was at it for a few hours and nothing I tried worked.
- Covid-19 (Coronavirus) Analytics
  - Updated stats for the day as usual

**Thoughts:**  
It's amazing that something as simple as setting a start color for the particles is incredibly complicated in Unity. Here's what happened:  
- Changed ParticleSystem.color and got `ParticleSystem.color is deprecated, use ParticleSystem.main.color`
- OK, then I changed `ParticleSystem.main.color`, but that didn't do anything either.  It turns out that color is not a standard Color variable, but a `MinMaxGradient` variable where any number of sub-variables could be the active color
- There are also other modules like `ColorOverLifetimeModule` in the particle system that may override the color
- After finally finding the correct variable to change, I changed it, confirmed that it was changed in Debug.Log, and yet still the particle system remains white.  
- Called it a night

That was a very not-fun 2-3 hours spent trying to simply set the color of a particle system. It really makes a big difference visually in the game so I'd love to get it worked out, but Unity is not making it easy on me.  Hopefully they'll will streamline this in future versions.

**Link(s) to work:**
1. [NovaForge - Trying everything and the kitchen sink to get the in-game particles to be different color. Nothing is working.](https://github.com/BrianLeip/NovaForge/commit/b2b14f53530a45240fb2e1a4973137532ad495a9)
2. [Covid-19 Analytics - Updated stats for the day](https://github.com/BrianLeip/Covid19_Analytics/blob/08606181e6dcd4aaa458ebccac76fd021b5a6b96/Covid19_Analytics.ipynb)
---

## R5-D55: May 20, 2020 - Wednesday

**Today's Progress:**  
- NovaForge
  - Separated intro and in-game element cloud spawning
  - Moved space warp to be inside camera (you)
  - Absorbing particles increases quantum power
- Covid-19 (Coronavirus) Analytics
  - Updated stats for the day as usual

**Thoughts:**  
Felt good to get back into NovaForge now that the pressure cooker of the game jam is over.  This game has a lot of potential and I'm going to keep moving forward on it.

**Link(s) to work:**
1. [NovaForge - Separated intro and in-game element cloud spawning](https://github.com/BrianLeip/NovaForge/commit/4dab7d48dc6584a38dd519583a7d030b6b3bc91a)
2. [NovaForge - Moved space warp to be inside camera (you)](https://github.com/BrianLeip/NovaForge/commit/8d0f8d08b6057ad36398b68bea71bd72c4cc0635)
3. [NovaForge - Absorbing particles increases quantum power](https://github.com/BrianLeip/NovaForge/commit/dd0db91073f066582ea017f60aba3abeb7848517)
4. [Covid-19 Analytics - Updated stats for the day](https://github.com/BrianLeip/Covid19_Analytics/blob/e51f102e023fd560fcddedd812fc538131df070d/Covid19_Analytics.ipynb)
---

## R5-D54: May 19, 2020 - Tuesday

**Today's Progress:**  
- Input system testing (Unity)
  - Testing out Unity's new input system within the DOTween test project
- Covid-19 (Coronavirus) Analytics
  - Updated stats for the day as usual

**Thoughts:**  
Input is another area I need to improve on, so I'm testing out Unity's new input system.  This one is more stable than the UIBuilder / UI Elements and safe to use.

**Link(s) to work:**
1. [Unity Input system testing](https://github.com/BrianLeip/DOTween-Test/commit/47d9b465ab549f29ad1211653b09084bb591526a)
2. [Covid-19 Analytics - Updated stats for the day](https://github.com/BrianLeip/Covid19_Analytics/blob/ede8e3cfae0cf5f1eeceafd6f22c880211406427/Covid19_Analytics.ipynb)
---

## R5-D53: May 18, 2020 - Monday

**Today's Progress:**  
- DOTween Test (Unity)
  - Created a new project to test out the DOTween tool - used to animate UI
- Covid-19 (Coronavirus) Analytics
  - Updated stats for the day as usual

**Thoughts:**  
The game jam taught me that UI is an area I need to improve on, and also that Unity's UI Builder and UI Elements are still in very rough, early stages, so I need to use something more stable.  

To that end, I'm testing out DOTween which is a "Tweener" tool used by a ton of Unity developers along with Unity's canned UI system to create nice looking animated UI.

**Link(s) to work:**
1. [DOTween - Created a new project to test out the DOTween tool - used to animate UI](https://github.com/BrianLeip/DOTween-Test/commit/357e88c0f0c375e8fd85d3d0f5cb44a729f78023)
2. [Covid-19 Analytics - Updated stats for the day](https://github.com/BrianLeip/Covid19_Analytics/blob/69f370821aab2cb3d90ca13a3074e1e79ec78240/Covid19_Analytics.ipynb)
---

## R5-D52: May 17, 2020 - Sunday

**Today's Progress:**  
- Simulation Game Jam (NovaForge)
  - Separated out the intro scene from game scene, added transition between the two
  - More improvements to menu system
  - Added mechanic to deploy space warps
  - Bundled game, added an icon and uploaded to itch.io
  - Done (for now)
- Covid-19 (Coronavirus) Analytics
  - Updated stats for the day as usual

**Thoughts:**  
Sim game jam submission day: spent all day on NovaForge 13+ hours or so and then submitted it to itch.io for the competition.  
Was it perfect?  No.  Were there a lot of things missing?  Yup.  But after multiple game jams where I joined but didn't submit because it wasn't "good enough", I'm forcing myself to submit this one anyways, flaws and all.  I have a tendency to beat myself up when I don't create something that lives up to the vision and expectations that were in my head, but I now know that all creative people experience that feeling.  

What's important here is that I met my objectives of 1) Finishing a freaking game jam, 2) learning things along the way (I learned a ton actually), and 3) have a nugget of a good game that could be turned into something great in the future.  I achieved all 3 of those things, and I'm learning to use setbacks and imperfect creations as fuel to get better, not as a whip to flog myself with.  

**Link(s) to work:**
1. [NovaForge - Too many links. Just going to post my itch.io submission page](https://torchfire.itch.io/novaforge)
2. [Covid-19 Analytics - Updated stats for the day](https://github.com/BrianLeip/Covid19_Analytics/blob/f66c1831cd5bb0df5ff70d21857e88ea6867734c/Covid19_Analytics.ipynb)
---

## R5-D51: May 16, 2020 - Saturday

**Today's Progress:**  
- Simulation Game Jam (NovaForge)
  - Added the UI Menu's I built previously
  - Created an Elements system, keeps track of how many particles absorbed
- Free Code Camp
  - Completed first 10 exercises in Applied Visual Design section
- Smarter way to learn HTML & CSS
  - Finished ch 5
- Covid-19 (Coronavirus) Analytics
  - Updated stats for the day as usual

**Thoughts:**  
Big day!  Finished the multi-day project to get the UI working and implemented it in NovaForge.  Also got the Element absorbing system started.  Game Jam deadline is tomorrow night, I'm in the homestretch, just gotta push through.  

On top of NovaForge work, I got more done on Free Code Camp and Smarter way to learn HTML and CSS.  May skip these tomorrow to focus 100% on NovaForge on submission day.

**Link(s) to work:**
1. [NovaForge - Added the UI Menu's I built previously](https://github.com/BrianLeip/NovaForge/commit/a553a9fe3a5d1f25bc17697c7363a7e8eb20b0c2)
2. [NovaForge - Created an Elements system, keeps track of how many particles absorbed](https://github.com/BrianLeip/NovaForge/commit/04c972c76fb23ee450ce0bf538cd8d1a888e38f7)
3. [Free Code Camp - Completed first 10 exercises in Applied Visual Design section](https://github.com/BrianLeip/FCC-Responsive-Web-Design/commit/2d9b8a218916a296649903f0ff884b745f3ad40c)
4. [Smarter way to learn HTML & CSS - Finished ch 5](https://github.com/BrianLeip/Smarter-Way-HTML-CSS/commit/993ad9f825bea4a65914e414740e83eb1eea54ec)
5. [Covid-19 Analytics - Updated stats for the day](https://github.com/BrianLeip/Covid19_Analytics/blob/4ad22316b5ba45329369193481710fce7935ec26/Covid19_Analytics.ipynb)
---

## R5-D50: May 15, 2020 - Friday

**Today's Progress:**  
- Simulation Game Jam (NovaForge)
  - Fixed text/font issues with the UI Builder package in my test project.  Buttons, text and labels all working now.
- Free Code Camp
  - Finished the last 14 exercises in the Basic CSS section
- Covid-19 (Coronavirus) Analytics
  - Updated stats for the day as usual

**Thoughts:**  
UI has admittedly never been my strong suit, but I need to focus to get something into NovaForge ASAP.  Only 2 days left so it's time to just get a functioning UI prototype working and move on to other stuff.  Fortunately, the things I'm learning will make UI much easier in the future, and help me in every single project/game that I work on, since everything needs UI.  So despite being time consuming it's vital.  

Also, Feels good to knock out another section of FCC.  Moving forward.

**Link(s) to work:**
1. [UI Builder - Fixed text/font issues with the UI Builder package.  Buttons, text and labels all working now](https://github.com/BrianLeip/Unity-UI-Builder-Test/commit/a44fe37e910906d7861e1eef1bd25f0069f6dfb0)
2. [Free Code Camp - Finished the last 14 exercises in the Basic CSS section](https://github.com/BrianLeip/FCC-Responsive-Web-Design/commit/ca7c9a2c14c1cbdd836fb37b04e1dfee93949a60)
3. [Covid-19 Analytics - Updated stats for the day](https://github.com/BrianLeip/Covid19_Analytics/blob/238a2d28425904ebcd3e298348e7889d33645e47/Covid19_Analytics.ipynb)
---

## R5-D49: May 14, 2020 - Thursday

**Today's Progress:**  
- Simulation Game Jam (NovaForge)
  - Tested out Unity's new UI Builder with their Tanks demo
  - Created my own test project to make UI menus with Unity's UI Builder
    - Got the first buttons working with hover and click animations
- Free Code Camp
  - 10 more exercises in the Basic CSS section
- A Smarter Way to Learn HTML and CSS
  - Finished ch 4
- Covid-19 (Coronavirus) Analytics
  - Updated stats for the day as usual

**Thoughts:**  


**Link(s) to work:**
1. [Tested out Unity's new UI Builder with their Tanks demo](https://github.com/BrianLeip/UI-Builder-Tanks-Demo/commit/aee680c4b2faf3ea400a832e2f898d72eb6ba552)
2. [UI Builder Test - Got the first buttons working with hover and click animations](https://github.com/BrianLeip/Unity-UI-Builder-Test/commit/002a80ed2663d9fa4f7b8840b61dc95584b02754)
3. [Free Code Camp - 10 more exercises in basic CSS section](https://github.com/BrianLeip/FCC-Responsive-Web-Design/commit/ba2d094fecf5fbd5869a829b90ac7d9d14b68af8)
4. [Smarter Way to Learn HTML & CSS - Finished ch 4](https://github.com/BrianLeip/Smarter-Way-HTML-CSS/commit/1db2461db1809582ba81c5c1f82489f4da3cdeec)
5. [Coronavirus Analytics - Updated stats for the day](https://github.com/BrianLeip/Covid19_Analytics/blob/91080a9df17af29474f21208f1eba2f8f8efbbc8/Covid19_Analytics.ipynb)
---

## R5-D48: May 13, 2020 - Wednesday

**Today's Progress:**  
- Simulation Game Jam (NovaForge)
  - None today
- Free Code Camp
  - did a few exercises but forgot to commit them to git
- A Smarter Way to Learn HTML and CSS
  - Started book alongside FCC since it's highly regarded as a good hands-on book to retain info
  - Completed ch 1, 2, 3
- Covid-19 (Coronavirus) Analytics
  - Updated stats for the day as usual

**Thoughts:**  
I'm enjoying this and feeling like I'm progressing , but a part of me wonders if I'm spreading myself too thin.  Currently doing a game jame in Unity/C# and learning new game dev techniques, learning HTML and CSS with both Free Code Camp and Smarter Way to Learn book, and also will be continuing the MongoDB course.  

On second thought, it's all a matter of time.  If I only do 1-2 hours of coding a day, then this is definitely too much.  But if I do 6-10 hours of coding a day, then this is very much manageable.  So I just need to dedicate more time and allocate appropriately.  I'd say 70% game jam given the looming deadline of the 17th, 10% FCC, 10% Smarter way to learn book, 10% MongoDB.  A little progress every day.

**Link(s) to work:**
1. Free Code Camp - did a few exercises but forgot to commit them to git
2. [Smarter Way to Learn HTML & CSS - Completed ch 1, 2, 3](https://github.com/BrianLeip/Smarter-Way-HTML-CSS/commit/af3ec6d7d85ed707244a9d183f9fbce736adecae)
3. [Coronavirus Analytics - Updated stats for the day](https://github.com/BrianLeip/Covid19_Analytics/blob/e6c65377f4b70c23da7c2d848a86a53326e061a5/Covid19_Analytics.ipynb)
---

## R5-D47: May 12, 2020 - Tuesday

**Today's Progress:**  
- Simulation Game Jam (NovaForge)
  - Particle System C# Jobs Test
- Covid-19 (Coronavirus) Analytics
  - Updated stats for the day as usual

**Thoughts:**  
The C# Jobs system definitely has potential to improve the efficiency of the particles but the package is still in preview and unstable.  Time is short before the game jam ends on Sunday so need to shift focus back to other priorities.

**Link(s) to work:**
1. [NovaForge - Particle System C# Jobs Test](https://github.com/BrianLeip/Unity-DOTS-Testing/tree/a9f0295ac952a4434587438344bc8136a60736a0/Particle-Job-System-Test)
2. [Coronavirus Analytics - Updated stats for the day](https://github.com/BrianLeip/Covid19_Analytics/blob/e2964d3c001d44e4e533a734f94c3f5b695edda5/Covid19_Analytics.ipynb)
---

## R5-D46: May 11, 2020 - Monday

**Today's Progress:**  
- Simulation Game Jam (NovaForge)
  - More testing of Unity DOTS system
- Unity Utility Scripts
  - Created custom camera controller script
  - Started a new repo to track all custom scripts in a library
- Covid-19 (Coronavirus) Analytics
  - Updated stats for the day as usual

**Thoughts:**  
Was up very late/early with client work so I didn't have as much time to dedicate to this as I wanted.  But time is running short on the game jam (ends Sunday 5/17) so I need (and want) to carve out more time for this.  The majority of my client work is done for the month so that frees me up a lot more.

**Link(s) to work:**
1. [NovaForge - Improvements to camera controller, more DOTS testing](https://github.com/BrianLeip/NovaForge/commit/bd92d18466dbcd1abaae7682656ca160cf5cf564)
2. [Started Unity Utilities Library with Simple Camera Controller Script](https://github.com/BrianLeip/Unity-Utility-Scripts/blob/11d348b12ce7557c0b4a734231e2a132add6f0da/SimpleCameraControllerBL.cs)
3. [Coronavirus Analytics - Updated stats for the day](https://github.com/BrianLeip/Covid19_Analytics/blob/fe7d86c058c99c6a919e89329ddf5a8d8217b716/Covid19_Analytics.ipynb)

---

## R5-D45: May 10, 2020 - Sunday

**Today's Progress:**  
- Simulation Game Jam (NovaForge)
  - Learned about the Unity DOTS / Job system, started testing it out
- Covid-19 (Coronavirus) Analytics
  - Updated stats for the day as usual

**Thoughts:**  
After testing NovaForge out on my macbook pro and getting terrible performance, making it more efficient is key.  And the DOTS / C# Job System is the best way to make that happen.  
In the Job system test / tutorial project I'm working on, using Jobs and Burst compiler improved FPS from 6 to 350! That's a 58x improvement.  There's a bit of a learning curve here, and it's still in preview mode and volatile, but once I get it down it will unlock huge potential.  

**Link(s) to work:**
1. [NovaForge - Learned about the Unity DOTS / Job system, started testing it out](https://github.com/BrianLeip/Unity-DOTS-Testing/blob/6ceb72ee4daa9281de540aa4a5a34d6febfa2c87/README.md)
2. [Coronavirus Analytics - Updated stats for the day](https://github.com/BrianLeip/Covid19_Analytics/blob/395ae5e274054d878109c3cdeaaec628bcf1921a/Covid19_Analytics.ipynb)

---

## R5-Dxx: May 9, 2020 - Saturday


**Thoughts:**  
After yesterday'g big day, I took 1 day off for some personal and client work today.

---

## R5-D44: May 8, 2020 - Friday

**Today's Progress:**  
- Simulation Game Jam (NovaForge)
  - Tested out URP and HDRP versions of NovaForge to see if it would make it more efficient.  But the opposite happened
  - Made efficiency improvements and nearly doubled the FPS!  75 -> 135
  - Changed the nebulas so that they're in the shape of a cloud insead of a boring sphere.  Can be scaled and rotated too.
  - Space Warps now turn into Stars!
  - Tested and learned Amplify Shader editor tool
  - Added and customized some star shaders
- Free Code Camp
  - Completed 10 more exercises in the Basic CSS section
- Covid-19 (Coronavirus) Analytics
  - Updated stats for the day as usual

**Thoughts:**  
Big progress on NovaForge today.  Spent most of the day on it and love how it's starting to turn out. Gonna keep on moving.

**Link(s) to work:**
1. [NovaForge - Improved efficiency from 75 FPS to 135 FPS](https://github.com/BrianLeip/NovaForge/commit/d079393710737dc01ca38edd81c712dc44b3c418)
2. [NovaForge - Partcile clouds are now in the shape of clouds!  Not boring spheres.  ](https://github.com/BrianLeip/NovaForge/commit/8527edc7a635e28cd0feec9e72f7ff5eb33992b2)
3. [NovaForge - A star is born](https://github.com/BrianLeip/NovaForge/commit/79882dd65fb7ad46f43099d799e687288bcb94fd)
4. [NovaForge - Tested Amplify shader editor and created a custom star fire shader](https://github.com/BrianLeip/NovaForge/commit/0385ef2768a5e601779ead580f2dc392a00318b5)
5. [FCC - Completed 10 more exercises in the Basic CSS section](https://github.com/BrianLeip/FCC-Responsive-Web-Design/commit/e4ad89df79f769d15307bccc42c960d27745dc5f)
6. [Coronavirus Analytics - Updated stats for the day](https://github.com/BrianLeip/Covid19_Analytics/blob/2c3caf9c1cdbeaa3be8c3f1a2b57eb5dfbb7fe79/Covid19_Analytics.ipynb)

---

## R5-D43: May 7, 2020 - Thursday

**Today's Progress:**  
- Simulation Game Jam (NovaForge)
  - Nebulas now have limited number of articles that can be absorbed, then they're shut off
- Free Code Camp
  - Completed 10 exercises in the Basic CSS section
- MongoDB University
  - Set up MongoDB demo database, connected to it through MongoDB Compass and through the shell
- Covid-19 (Coronavirus) Analytics
  - Updated stats for the day as usual

**Thoughts:**  
Feels like I'm starting to make good progress on all fronts.  Want to dedicate even more time to this whenever possible.

**Link(s) to work:**
1. [NovaForge - Nebulas limited number of particle absorption before shutting off](https://github.com/BrianLeip/NovaForge/commit/acfaa8b801013800a4d49ce7372d2e4239da2652)
2. [FCC - Completed 10 exercises in the Basic CSS section](https://github.com/BrianLeip/FCC-Responsive-Web-Design/commit/2dcd6b597aec8fb89e228bc3f26cf8a9b9fc93e9)
3. [MongoDB University - M001: MongoDB Basics](https://university.mongodb.com/courses/M001/about)
4. [Coronavirus Analytics - Updated stats for the day](https://github.com/BrianLeip/Covid19_Analytics/blob/45ac06e01303d77158ca9548bd41ce6b9dc5bd45/Covid19_Analytics.ipynb)

---

## R5-D42: May 6, 2020 - Wednesday

**Today's Progress:**  
- Free Code Camp
  - Completed Basic HTML Section
- Covid-19 (Coronavirus) Analytics
  - Updated stats for the day as usual

**Thoughts:**  
Quick one today, but I knocked out the rest of the Basic HTML section before bed.

**Link(s) to work:**
1. [FCC - Completed Basic HTML section](https://github.com/BrianLeip/FCC-Responsive-Web-Design/blob/513bac28ccfb1863e1d6db8b430ba7c2635c8288/1-Basic-HTML/Basic%20HTML%20-%20Done.PNG)
2. [Coronavirus Analytics - Updated stats for the day](https://github.com/BrianLeip/Covid19_Analytics/blob/a66c6a4855bd8982b1c7e53a8fdda5d3e4a30adc/Covid19_Analytics.ipynb)

---

## R5-D41: May 5, 2020 - Tuesday

**Today's Progress:**  
- Simulation Game Jam (NovaForge)
  - Got Space Warp gravity to increase as it grows
- Free Code Camp
  - Did 10 more exercises on Responsive Web Design course
- MongoDB University
  - Started M001: MongoDB Basics Course
- Covid-19 (Coronavirus) Analytics
  - Updated stats for the day as usual

**Thoughts:**  
Gravity is controlled by MinMaxCurves and it was a lot more difficult to change than originally thought.  Eventually figured it out though.  
Also continued with more FCC exercises, and started a MongoDB course to solidify my NoSQL data query skills.

**Link(s) to work:**
1. [NovaForge - Got Space Warp gravity to increase as it grows](https://github.com/BrianLeip/NovaForge/commit/0a15a588758b794bd58e9878dec5925fa02095a4)
2. [FCC - More exercises in Responsive Web Design Course](https://github.com/BrianLeip/FCC-Responsive-Web-Design/commit/6264bd317a55d1b9cce1e00d4c4b195173a869cb)
3. [MongoDB University - M001: MongoDB Basics](https://university.mongodb.com/courses/M001/about)
4. [Coronavirus Analytics - Updated stats for the day](https://github.com/BrianLeip/Covid19_Analytics/blob/d9b6ed22603bb34107fd182112e116628cdaa153/Covid19_Analytics.ipynb)

---

## R5-D40: May 4, 2020 - Monday

**Today's Progress:**  
- Simulation Game Jam (NovaForge)
  - Got particle collisions working and Space Warps now grow when they absorb particles
- Free Code Camp
  - Started Responsive Web Design course, did 10 exercises

**Thoughts:**  
Got particle collisions working and Space Warps now grow when they absorb particles.  Looks so damn cool!

**Link(s) to work:**
1. [NovaForge - Got particle collisions working and Space Warps now grow when they absorb particles](https://github.com/BrianLeip/NovaForge/commit/492959239805a4d09c45e5e8f601e875e17af0e2)
2. [FCC - Started Responsive Web Design course, did 10 exercises](https://github.com/BrianLeip/FCC-Responsive-Web-Design/commit/866a329869b61b5342c2dd89850e12bbc115df48)
2. Coronavirus Analytics - no update today

---

## R5-D39: May 3, 2020 - Sunday

**Today's Progress:**  
- Simulation Game Jam (NovaForge)
  - Worked on getting Particle collisions working

**Thoughts:**  
Had to do a lot of client work today so not as much time for coding today, but still squeezed some in. 

Spent about an hour working on getting particle collisions working so that the Space Warps can consume the particles and grow.  But still wasn't working so I'll have to dig back in tomorrow and figure it out.

**Link(s) to work:**
1. [NovaForge - Worked on getting Particle collisions working](https://github.com/BrianLeip/NovaForge/commit/a3b15720614b0dca28c30e85899dd7dff23381de)
2. Coronavirus Analytics - no update today

---

## R5-D38: May 2, 2020 - Saturday

**Today's Progress:**  
- Simulation Game Jam (NovaForge)
  - Created black holes with particle force fields (gravity & rotation)
  - Looked into the HDRP VFX Graph as an alternative to DOTS to handle huge num of particles
  - Switched particle system to be GPU based, made new GPU particle material
- Covid-19 (Coronavirus) Analytics
  - Updated stats for the day as usual

**Thoughts:**  
Spent almost all day working on NovaForge and have a great little space sim coming together.  It's amazing how focused and determined I am when working on something I enjoy.

**Link(s) to work:**
1. [NovaForge - Created black holes, particle force fields, converted particle system to GPU based](https://github.com/BrianLeip/NovaForge/commit/703356aa31827885b7f23e8f19c93bd370a96326)
2. [Coronavirus Analytics - Updated stats for the day](https://github.com/BrianLeip/Covid19_Analytics/blob/b43ab3beb8c4d55e1090f9d8bee87944acc63b3f/Covid19_Analytics.ipynb)

---

## R5-D37: May 1, 2020 - Friday

**Today's Progress:**  
- Simulation Game Jam (NovaForge)
  - Set up git repo, fixed many .gitignore issues, created Unity project
  - Created prototype space scene with particle clouds and movement
- Covid-19 (Coronavirus) Analytics
  - Updated stats for the day as usual

**Thoughts:**  
Simulation Game jam started!  

*Theme = "A matter of degree"*   
I brainstormed on different ideas and game mechanics and landed on one that should be pretty fun to make.  Elements (matter) are created stars explode in the raging temperatures (degree) of a supernova.  

*Nova Forge - A supernova simulator where new elements are created*  

Spent the day getting the git repo set up (lots of issues with .gitignore that I eventually worked out), then creating a prototype space scene with particle clouds that you can fly around in.

**Link(s) to work:**
1. [NovaForge - Set up project, created prototype space scene](https://github.com/BrianLeip/NovaForge/commit/3a1baa99d05c506cf8fff305e044b71d7afc02fb)
2. [Coronavirus Analytics - Updated stats for the day](https://github.com/BrianLeip/Covid19_Analytics/blob/c0d3a6ee6c8eb4783b5824840c7537379adcd871/Covid19_Analytics.ipynb)

---

## R5-D36: April 30, 2020 - Thursday

**Today's Progress:**  
- Eye Catching UI In Unity
  - Created fade in and fade out transitions
- Unity DOTS / ECS System
  - Testing out Unity DOTS demos for ECS and Physics
- Covid-19 (Coronavirus) Analytics
  - Updated stats for the day as usual

**Thoughts:**  
*Catch-up for last week of coding Apr 26 - May 1*  
I joined a game jam that starts on May 1st, so I'm doing a little research on Unity tools / libraries to prepare.  The DOTS / ECS system is a rebuild of the entire Unity library that drastically improves performance.  The game jam is a simulation (processor heavy) so I'm looking into this as a potential option for the game jam.

**Link(s) to work:**
1. [Eye-catching UI in Unity - Created fade in and fade out transitions](https://github.com/BrianLeip/UI-In-Unity/tree/52a14fa693314800e9ccd425f381dabc2b1811a2)
2. [Unity DOTS / ECS demos and physics testing](https://github.com/BrianLeip/Unity-ECS-Demo/tree/5599d783706474a777d5247b9b2059758b169444)
3. [Coronavirus Analytics - Updated stats for the day](https://github.com/BrianLeip/Covid19_Analytics/blob/c83d8cc143d0688f21d2cd2a2fcbea1ed38541d1/Covid19_Analytics.ipynb)

---

## R5-D35: April 29, 2020 - Wednesday

**Today's Progress:**  
- Eye Catching UI In Unity
  - Created a slide-in pause menu
- Covid-19 (Coronavirus) Analytics
  - Updated stats for the day as usual

**Thoughts:**  
*Catch-up for last week of coding Apr 26 - May 1*  
Lots of issues with this tutorial - files are too big, tutorial skips important steps...  I'm pushing through by looking at what the goal is (e.g. slide-in pause menu using animation) and then creating it myself.

**Link(s) to work:**
1. [Eye-catching UI in Unity - Created a slide-in pause menu](https://github.com/BrianLeip/UI-In-Unity/tree/f07c173ee5fc2ec8b0f8ce6c5b7fe8e3c39071bb)
2. [Coronavirus Analytics - Updated stats for the day](https://github.com/BrianLeip/Covid19_Analytics/blob/c83d8cc143d0688f21d2cd2a2fcbea1ed38541d1/Covid19_Analytics.ipynb)

---

## R5-Dxx: April 26 to 28, 2020 - Sunday to Tuesday

**Today's Progress:**  
- Covid-19 (Coronavirus) Analytics
  - Updated stats for the day as usual

**Thoughts:**  
*Catch-up for last week of coding Apr 26 - May 1*  
Had a rough few days and needed some time off.  Didn't count this one towards 100 Days Of Code total.  

**Link(s) to work:**
1. [Coronavirus Analytics - Updated stats for Apr 26](https://github.com/BrianLeip/Covid19_Analytics/blob/f118e00149bfb4fcc4cc973c2a895ef834ac2f10/Covid19_Analytics.ipynb)
2. [Coronavirus Analytics - Updated stats for Apr 27](https://github.com/BrianLeip/Covid19_Analytics/blob/ac466efc08407fb096a5d54c60c89697be6fbe80/Covid19_Analytics.ipynb)
3. [Coronavirus Analytics - Updated stats for Apr 28](https://github.com/BrianLeip/Covid19_Analytics/blob/2f74dd39d22cf58243a30d4d5a2b716da7ed97f7/Covid19_Analytics.ipynb))

---

## R5-D34: April 25, 2020 - Saturday

**Today's Progress:**  
- Unity: Eye Catching UI Tutorial
  - Spent an hour or so getting the overly large files compressed, ignored from git, but still usable in the Unity project
  - Loaded the project and tested out the different UI scenarios.  All working according to plan
- Covid-19 (Coronavirus) Analytics
  - Updated stats for the day as usual

**Thoughts:**  
It took an hour or so to fix but I resolved the tutorial's large file issue. Frustrating for a UI tutorial, but I'm considering it practice to get better with git ignoring specific files, compressing files, etc.
Now I can actually start the tutorial!  If they have a recommendation section, let them know the files are too damn big.  

**Link(s) to work:**
1. [Unity: Eye Catching UI Tutorial - Fixed the >60MB file issues, tested out UI](https://github.com/BrianLeip/UI-In-Unity/commit/96a13929fac009cb6d994e9f44c11fb6fd1d194e)
2. [Coronavirus Analytics - Updated stats for the day](https://github.com/BrianLeip/Covid19_Analytics/blob/5323f71fdfe3548aa702396f19dd9910862b29ee/Covid19_Analytics.ipynb)

---

## R5-D33: April 24, 2020 - Friday

**Today's Progress:**  
- Unity: Eye Catching UI Tutorial
  - Finished first 2 course videos, downloaded project files, loaded into project
  - Some of their files are too big for git (>60MB). Hitting a roadblock will need to revisit tomorrow
- Covid-19 (Coronavirus) Analytics
  - Updated stats for the day as usual

**Thoughts:**  
Very frustrating that a tutorial about something as lightweight as UI would use massively large assets that are too big for git.  I'll need to play around to see how to compress or exclude those files so that I can move forward on this.

**Link(s) to work:**
1. [Unity: Eye Catching UI Tutorial - Started](https://github.com/BrianLeip/UI-In-Unity/commit/8237e966ae96439a1d06872b80bf56fe72820e39)
2. [Coronavirus Analytics - Updated stats for the day](https://github.com/BrianLeip/Covid19_Analytics/blob/de2efd23aa11790498e1b214c3a4ba9c5457baaf/Covid19_Analytics.ipynb)

---

## R5-D32: April 23, 2020 - Thursday

**Today's Progress:**  
- UnityMLAgentPenguins
  - Finished this project!!
  - Added all scripts, prefabs, etc
  - Updated scripts to be compatible with MLAgents 0.15.1
  - Trained Penguin Agents Neural Net using TensorFlow to find fish and feed her baby
  - Added the trained NN model to the Penguin prefab
- Covid-19 (Coronavirus) Analytics
  - Updated stats for the day as usual

**Thoughts:**  
This was definitely one of the more challenging but rewarding projects I've worked on.  Challenging because the MLAgents library is evolving rapidly and none of the code from the tutorial works out of the box.  There are also multiple versions of the tutorial, all of which are out of date.  Took a lot of tweaking and refactoring to get it to work, but when it all came together in the end it was very rewarding.

Now that I've gotten my first Unity ML agents project under my belt, this opens up a whole new world to me and I'm excited to dive in.

**Link(s) to work:**
1. [UnityMLAgentPenguins - Finished the project!](https://github.com/BrianLeip/UnityMLAgentPenguins/tree/7807f90acac7e84e6f432b4683bcf1468c26bbae)
2. [Coronavirus Analytics - Updated stats for the day](https://github.com/BrianLeip/CoronaVirus/blob/2930273031e594610085c79b699b1b431393b3ea/Covid19_Analytics.ipynb)

---

## R5-D29 to D31: April 20 to 22, 2020 - Monday to Wednesday

**Today's Progress:**  
- UnityMLAgentPenguins
  - Restarted project to incorporate all recent changes to MLAgent package
    - MLAgents 0.15.1 and Baracuda 0.6.1 packages
  - Added ML Agent Example projects
    - modified them to get them working (missing scripts on the prefabs)
    - tested example projects out, gain better understanding of MLAgent library
- Covid-19 (Coronavirus) Analytics
  - Updated stats for the day as usual

**Thoughts:**  
*Note - Been coding every day but not logging it on here.  Getting everything caught up from Apr 14 to Apr 23.*  

These 3 days sort of blurred together (late nights / early mornings) so I'm combining them together here.

Made great progress on the Unity Machine Learning Agent Penguins tutorial.  This one is especially hard because the MLAgent package is changing rapidly and the tutorial is already out of date. Need to do a lot of tweaks and adjustments to get things to work.  Frustrating, but great for learning experience.

**Link(s) to work:**
1. [UnityMLAgentPenguins - Restarted project for updated versions of MLAgent package](https://github.com/BrianLeip/UnityMLAgentPenguins/tree/27a8cf0d1f527ccfb852afaacbeb5dfa3ca61d22/MLAgentPenguins)
2. [UnityMLAgentPenguins - Added ML Agent example projects, fixed bugs, tested them out](https://github.com/BrianLeip/UnityMLAgentPenguins/tree/e199a32fe7fb607ca300a3fd657a3e6be2f627fc/MLAgentPenguins/Assets/ML-Agents/Examples)
3. [Coronavirus Analytics - Updated stats for Apr 19](https://github.com/BrianLeip/CoronaVirus/blob/020b1fa407c95778624980e0cb015eae9a59f3fb/Covid19_Analytics.ipynb)
4. [Coronavirus Analytics - Updated stats for Apr 20](https://github.com/BrianLeip/CoronaVirus/blob/55e622c7ec7cd4dbbf738496a5db741165dd0d56/Covid19_Analytics.ipynb)
5. [Coronavirus Analytics - Updated stats for Apr 21](https://github.com/BrianLeip/CoronaVirus/blob/c9b5fcfc5cdaa388cff656a86eb874550e2dfc6d/Covid19_Analytics.ipynb)
6. [Coronavirus Analytics - Updated stats for Apr 22](https://github.com/BrianLeip/CoronaVirus/blob/4dc4f946b2bfafb1dc76255f584d3fa5d505eb5b/Covid19_Analytics.ipynb)

---

## R5-Dxx: April 19, 2020 - Sunday

**Today's Progress:**  
n/a

**Thoughts:**  
*Note - Been coding every day but not logging it on here.  Getting everything caught up from Apr 14 to Apr 23.*  

Took the day off today after full day of coding on Sat.  Not counting towards 100 days of code day count.

**Link(s) to work:**


---

## R5-D28: April 18, 2020 - Saturday

**Today's Progress:**  
- Game Jam
  - Spent full day working on a game jam - Tilted Game Jam 20
  - Word prompts: 
    - Colorful
    - BBQ
  - Worked on a team of 3 to create a backyard BBQ game where you cook up meat, fish, or veggies and serve to guests
- Covid-19 (Coronavirus) Analytics
  - Updated stats for the day as usual

**Thoughts:**  
*Note - Been coding every day but not logging it on here.  Getting everything caught up from Apr 14 to Apr 23.*  

Spent the full day coding on this game jam.  To be honest, it turned out pretty crappy, but I konw that you have to allow yourself to create bad shit if you every want to create quality, so I'm not brushing it off.  The next one will be better, and the one after that even better, and so on.  Persistence is key.

**Link(s) to work:**
1. [Tilted Game Jam 20 - Colorful BBQ game](https://github.com/saltyJeff/colorful-bbq/tree/96e75078ddf9f5ac7cc0b796952971bd9b51eac7)
2. [Coronavirus Analytics - Updated stats for the day](https://github.com/BrianLeip/CoronaVirus/blob/6a2f9796a9663ee6f0d0d420e3ea4280f6450ac0/Covid19_Analytics.ipynb)

---

## R5-D27: April 17, 2020 - Friday

**Today's Progress:**  
- LeetCode
  - Completed on Product of Array Except Self!!
- Covid-19 (Coronavirus) Analytics
  - Updated stats for the day as usual

**Thoughts:**  
*Note - Been coding every day but not logging it on here.  Getting everything caught up from Apr 14 to Apr 23.*  

The "Product of Array Except Self" challenge definitely threw me for a loop.  But I was persistent, and worked through it over a couple days.  Full nights rest and a walk to clear my head did wonders.  

**Link(s) to work:**
1. [LeetCode - Completed Product of Array Except Self](https://github.com/BrianLeip/LeetCode/blob/4f0416cd2c08b2ca942ee7518be7053025da8422/238-ProductOfArrayExceptSelf.cpp)
2. [Coronavirus Analytics - Updated stats for the day](https://github.com/BrianLeip/CoronaVirus/blob/6e303f8195a0e1236324d9f034072a9cd30e8cf5/Covid19_Analytics.ipynb)

---

## R5-D26: April 16, 2020 - Thursday

**Today's Progress:**  
- LeetCode
  - Progress on Product of Array Except Self
- Covid-19 (Coronavirus) Analytics
  - Updated stats for the day as usual

**Thoughts:**  
*Note - Been coding every day but not logging it on here.  Getting everything caught up from Apr 14 to Apr 23.*  

The "Product of Array Except Self" challenge definitely threw me for a loop.  But I was persistent, and worked through it over a couple days.  Full nights rest and a walk to clear my head did wonders.  

**Link(s) to work:**
1. [LeetCode - Progress on Product of Array Except Self](https://github.com/BrianLeip/LeetCode/commit/a843bfdd441d87d14874dd3655c2f9a7aa97a9c8)
2. [Coronavirus Analytics - Updated stats for the day](https://github.com/BrianLeip/CoronaVirus/blob/352cef6bdfc918d9a020459d7a4505898e389a43/Covid19_Analytics.ipynb)

---

## R5-D25: April 15, 2020 - Wednesday

**Today's Progress:**  
- LeetCode
  - Started Product of Array Except Self
- Covid-19 (Coronavirus) Analytics
  - Updated stats for the day as usual

**Thoughts:**  
*Note - Been coding every day but not logging it on here.  Getting everything caught up from Apr 14 to Apr 23.*  

The "Product of Array Except Self" challenge definitely threw me for a loop.  But I was persistent, and worked through it over a couple days.  Full nights rest and a walk to clear my head did wonders.  

**Link(s) to work:**
1. [LeetCode - Started Product of Array Except Self](https://github.com/BrianLeip/LeetCode/blob/6a6453e0775808dd4f579e6a79dcce2dba6bf37b/238-ProductOfArrayExceptSelf.cpp)
2. [Coronavirus Analytics - Updated stats for the day](https://github.com/BrianLeip/CoronaVirus/blob/e9f2e1a097279cdc3dcea1c9a1b28e6fcdc88cab/Covid19_Analytics.ipynb)

---

## R5-D24: April 14, 2020 - Tuesday

**Today's Progress:**  
- LeetCode
  - Completed PerformStringShifts
- Covid-19 (Coronavirus) Analytics
  - Updated stats for the day as usual

**Thoughts:**  
*Note - Been coding every day but not logging it on here.  Getting everything caught up from Apr 14 to Apr 23.*  

**Link(s) to work:**
1. [LeetCode - Completed PerformStringShifts](https://github.com/BrianLeip/LeetCode/blob/494d8a0892ac6f873577b699c7d850e9526b2f27/PerformStringShifts.cpp)
2. [Coronavirus Analytics - Updated stats for the day](https://github.com/BrianLeip/CoronaVirus/blob/a250b37e61ef253be2334a93b28202961a2523fc/Covid19_Analytics.ipynb)

---

## R5-D23: April 13, 2020 - Monday

**Today's Progress:**  
- LeetCode
  - Finished Last Stone Weight
- Covid-19 (Coronavirus) Analytics
  - Updated stats for the day as usual

**Thoughts:**  
The LeetCode Last Stone Weight challenge was a tougher one than previous ones.  But it was good practice to create helper functions like "insertSorted" for a C++ vector and "printVector".  Those functions should really already be built in to the vector library already so it's surprising that they're not.  

It might be a good idea for me to start creating a library of my own with helper functions that I create, which will save a lot of time and follow the DRY method (Don't Repeat Yourself).

**Link(s) to work:**
1. [LeetCode - Finished Last Stone Weight](https://github.com/BrianLeip/LeetCode/blob/3ab86fc7beb1392908c52becfa8501cbb82b5ece/1046-LastStoneWeight.cpp)
2. [Coronavirus Analytics - Updated stats for the day](https://github.com/BrianLeip/CoronaVirus/blob/1a7714ff3aa42408439e9e5474d161a95a4e8936/Covid19_Analytics.ipynb)

---

## R5-D22: April 12, 2020 - Sunday

**Today's Progress:**  
- LeetCode
  - Started working on Last Stone Weight
- Covid-19 (Coronavirus) Analytics
  - Updated stats for the day as usual

**Thoughts:**  
Another lighter day, enjoying my weekend for a change.  Plan to get back at in more depth tomorrow.

**Link(s) to work:**
1. [LeetCode - Started working on Last Stone Weight](https://github.com/BrianLeip/LeetCode/commit/484346e66c79b2444fb4bbed6609a8961b9b1674)
2. [Coronavirus Analytics - Updated stats for the day](https://github.com/BrianLeip/CoronaVirus/blob/64c468c46dd4d5d25277301bb3b6bf801429db5b/Covid19_Analytics.ipynb)

---

## R5-D21: April 11, 2020 - Saturday

**Today's Progress:**  
- Unity:
  - Testing out Photon Unity Networking 2 (PUN2) package - multiplayer for Unity games
- Covid-19 (Coronavirus) Analytics
  - Updated stats for the day as usual

**Thoughts:**  
Lighter day than usual; had some personal things to take care of.

**Link(s) to work:**
1. [Testing out Photon Unity Networking 2 (PUN2) package](https://github.com/BrianLeip/PhotonUnityNetworking2-Test/tree/860f4c10c871755cedea0939458664577c9b2dcf)
2. [Coronavirus Analytics - Updated stats for the day](https://github.com/BrianLeip/CoronaVirus/blob/b4e80528bac2d6f5eaf686b49db4eb440a3bda12/Covid19_Analytics.ipynb)

---

## R5-D20: April 10, 2020 - Friday

**Today's Progress:**  
- LeetCode 30 day challenge
  - MinStack
- Covid-19 (Coronavirus) Analytics
  - Updated stats for the day as usual

**Thoughts:**  
Spent most of the day doing client work, errands, and some family game time today, but still carved out time to get today's LeetCode challenge done.  

Felt more confident solving this one, like the things I'm learning are coming together and the incline of the uphill battle is not as steep.  Got a runtime of 28ms which is better than 94% of other solutions.  Seeing my progress and improvement feels good.

**Link(s) to work:**
1. [LeetCode - MinStack](https://github.com/BrianLeip/LeetCode/blob/master/155-MinStack.cpp)
2. [Coronavirus Analytics - Updated stats for the day](https://github.com/BrianLeip/CoronaVirus/blob/9766d4971c8d081a6162ac70163f52463183646c/Covid19_Analytics.ipynb)

---

## R5-D19: April 9, 2020 - Thursday

**Today's Progress:**  
- LeetCode 30 day challenge
  - Backspace String Compare
- Covid-19 (Coronavirus) Analytics
  - Separated the Friends and Family location tracking charts and stats to a separate notebook
  - Added Costa Rica to Friends & Family notebook
  - Updated stats for the day as usual

**Thoughts:**  
I challenged myself to use Regex to solve today's LeetCode challenge and it was tougher than it looked at first.  But powered through and figured it out with very efficient time of O(1).

**Link(s) to work:**
1. [LeetCode - Backspace String Compare](https://github.com/BrianLeip/LeetCode/blob/84b126355673a6a9dc0d70937b082e0f85768be9/844-BackspaceStringCompare.cpp)
2. [Coronavirus - Friends and Family location tracking notebook](https://github.com/BrianLeip/CoronaVirus/blob/4ed27830fdb1aeaa257e6fe7eb8b2b9e3726e4c5/Covid19_FnF_Tracker.ipynb)
3. [Coronavirus Analytics - Updated stats for the day](https://github.com/BrianLeip/CoronaVirus/blob/766e6eb416d870800be4ec5e43ff3d3ed16232cd/Covid19_Analytics.ipynb)

---

## R5-D18: April 8, 2020 - Wednesday

**Today's Progress:**  
- Covid-19 (Coronavirus) Analytics
  - Major overhaul to notebooks and workflow
  - Created a separate ETL notebook to gather the data, wrangle and reformat it, then export to .csv
  - Revised the Analytics notebook so that it now pulls the data created by the ETL notebook
  - Added a few charts and metrics, including tracking US Counties where my friends and family live

**Thoughts:**  
Back in action.  Spent most of my day (9-10 hours or so) revamping the Covid-19 analytics notebook to create a separate ETL data wrangling file that exports .csv files to be used by the analytics notebook.  

Feels good to be back in it, and love seeing the result of exported csv files that I created with Python and Pandas, and then using them for a streamlined analytics notebook. 

**Link(s) to work:**
1. [Coronavirus Analytics - New ETL data wrangling notebook](https://github.com/BrianLeip/CoronaVirus/blob/19fd51e0798b522d0e9dc4b9f5028db5cbd9fc72/Covid19_Data_ETL.ipynb)
2. [Coronavirus Analytics - New Dataset export folder](https://github.com/BrianLeip/CoronaVirus/tree/19fd51e0798b522d0e9dc4b9f5028db5cbd9fc72/Datasets/JH)
3. [Coronavirus Analytics - Revised Analytics notebook](https://github.com/BrianLeip/CoronaVirus/blob/19fd51e0798b522d0e9dc4b9f5028db5cbd9fc72/Covid19_Analytics.ipynb)
2. [Coronavirus Analytics - Updated stats for the day](https://github.com/BrianLeip/CoronaVirus/blob/19fd51e0798b522d0e9dc4b9f5028db5cbd9fc72/Covid19_Analytics.ipynb)

---

## R5-Dxx: April 7, 2020 - Tuesday

**Thoughts:**  
Tough day...needed more time to reflect and regroup.

---
## R5-D17: April 6, 2020 - Monday

**Today's Progress:**  
- LeetCode 30 day challenge:
  - Maximum SubArray

**Thoughts:**  
Forced myself to get another Leetcode challenge done.  This one was a challenge.  I had a solution that worked but was too slow, so I worked on it until I came up with a much faster and more elegant solution.

**Link(s) to work:**
1. [LeetCode - Maximum SubArray](https://github.com/BrianLeip/LeetCode/blob/313ddb910292d6cadc1849aefa9e1b4cf1fe896e/053-MaximumSubarray.cpp)

---
## R5-D16: April 5, 2020 - Sunday

**Today's Progress:**  
- LeetCode 30 day challenge:
  - Best time to buy and sell stock II  
- Covid-19 (Coronavirus) Analytics
  - Updated stats for the day as usual

**Thoughts:**  
Forced myself to get a Leetcode challenge done.

**Link(s) to work:**
1. [LeetCode - Best time to buy and sell stock II](https://github.com/BrianLeip/LeetCode/blob/61c4839c3b1bafd4f3a309bd908edd26f0dacbb9/122-BestTimeToBuyAndSellStock2.cpp)
2. [Coronavirus Analytics - Updated stats for the day](https://github.com/BrianLeip/CoronaVirus/blob/efbfb07e09e5f3801944a7535eaa4554de97e0c8/Covid19_Analytics.ipynb)

---

## R5-Dxx: April 3 & 4, 2020 - Friday & Saturday

**Today's Progress:**  
- Covid-19 (Coronavirus) Analytics
  - Updated stats for the day as usual

**Thoughts:**  
Took a bit of a mental health break after the frustrating experience with the DS and Algorithms exam, and finding out that I was not accepted into the UIUC Masters program.

Being cooped up for too long on Coronavirus quarantine is wearing on me.  

"I feel I need a holiday.  A very long holiday."

**Link(s) to work:**
1. [Coronavirus Analytics - Updated stats for the day](https://github.com/BrianLeip/CoronaVirus/blob/efbfb07e09e5f3801944a7535eaa4554de97e0c8/Covid19_Analytics.ipynb)

---

## R5-D15: April 2, 2020 - Thursday

**Today's Progress:**  
- Data Structures and Algorithms
  - Last day of studying for the Upcoming UIUC Data Structures and Algorithms exam
  - Took exam
- LeetCode
  - Day 2 of 30 challenge: HappyNumber
- CoronaVirus Analytics
  - Updated stats for the day as usual

**Thoughts:**  
Up early and studying Data Structures and Algorithms all day. Took the exam and nailed it on the first 3/4 of it...then somehow bombed the last 1/4.  Got very close to the threshhold so I'm still hopeful that I will get accepted to the Masters program, since the exam is optional anyways.  Would be very painful if I don't... keeping my fingers crossed.

Also completed today's LeetCode challenge and updated CoronaVirus analytics.

**Link(s) to work:**
1. [Studied UIUC C++ Data Structures and Algorithms, took exam](https://github.com/BrianLeip/UIUC-Accel-CS-Code-Env/tree/801cb62b999bef9e4b64e0ba971ec87967008c93)
2. [LeetCode - Happy Number Challenge](https://github.com/BrianLeip/LeetCode/blob/master/202-HappyNumber.cpp)
3. [Coronavirus Analytics - Updated stats for the day](https://github.com/BrianLeip/CoronaVirus/blob/c1dad7c602fc46bb209095b6d97d1823a300931d/Covid19_Analytics.ipynb)

---

## R5-D14: April 1, 2020 - Wednesday

**Today's Progress:**  
- Data Structures and Algorithms
  - More studying for the Upcoming UIUC Data Structures and Algorithms exam
- LeetCode
  - Joined the 30 days of LeetCode challenge to keep improving my algorithms toolkit
  - First challenge: SingleNumber
- CoronaVirus Analytics
  - Added NY Times US County data and created a few charts
  - Updated stats for the day as usual

**Thoughts:**  
Got a lot done today, but still so much more to study for the upcoming DS and Algo exam.  Wishing I had more time.  

It's been months since I've seen my family in MA (has it been years?) and we had a Quarantine game night scheduled today on Zoom so I made sure to carve out time for that.  Really glad I did, it was a lot of fun and a good recharge inbetween study sessions.

**Link(s) to work:**
1. Studied UIUC C++ Data Structures and Algorithms (no link)
2. [LeetCode - SingleNumber Challenge](https://github.com/BrianLeip/LeetCode/blob/master/136-SingleNumber.cpp)
3. [Coronavirus Analytics - Updated stats for the day, added County level data from NY Times](https://github.com/BrianLeip/CoronaVirus/blob/dffddf34df6f6a6c625047d493f92f49ae4152af/Covid19_Analytics.ipynb)

---

## R5-D13: March 31, 2020 - Tuesday

**Today's Progress:**  
- Data Structures and Algorithms
  - More studying for the Upcoming UIUC Data Structures and Algorithms exam

**Thoughts:**  
A lot to study in a short amount of time...a bit overwhelming.  Need to stay focused.

**Link(s) to work:**
1. Studied UIUC C++ Data Structures and Algorithms (no link)
2. [Coronavirus Analytics - Updated stats for the day](https://github.com/BrianLeip/CoronaVirus/blob/5cd84a641cc8593e9414ccdeb8668a62334fe710/Covid19_Analytics.ipynb)

---

## R5-D12: March 30, 2020 - Monday

**Today's Progress:**  
- Data Structures and Algorithms
  - Studied for the Upcoming UIUC Data Structures and Algorithms exam

**Thoughts:**  
Continuing to study.  Unfortunately I can't retake the exams or practice assignments without paying for the course again.  But I saved all of the code in AWS Cloud 9 so I'm going to use that for practice and digging into the details.

**Link(s) to work:**
1. Studied UIUC C++ Data Structures and Algorithms (no link)
2. [Coronavirus Analytics - Updated stats for the day](https://github.com/BrianLeip/CoronaVirus/blob/3c1a4e9045c0c59f4c9029f3b827fbada9c142d8/.ipynb_checkpoints/Covid19_Analytics-checkpoint.ipynb)

---

## R5-D11: March 29, 2020 - Sunday

**Today's Progress:**  
- Data Structures and Algorithms
  - Studied for the Upcoming UIUC Data Structures and Algorithms exam

**Thoughts:**  
It's been about 6 months since I took the 3 UIUC DS and Algo in C++ courses on Coursera, so I need to refresh and solidify some concepts before the exam.

**Link(s) to work:**
1. Studied UIUC C++ Data Structures and Algorithms (no link)
2. [Coronavirus Analytics - Updated stats for the day](https://github.com/BrianLeip/CoronaVirus/blob/48b4045d4e6bcc6540657d385d5d15f7a096670f/Covid19_Analytics.ipynb)

---

## R5-D10: March 28, 2020 - Saturday

**Today's Progress:**  
- Covid19 Simulator:
  - Started working on a new Unity project as a combined Game Jam project and Coronavirus simulator
  - Set up a city, made an isometric camera, Created a person prefab, created script for person movement and turning.
- Unity ML Agent Penguins:
  - Finished getting all the scripts, scenes, and prefabs set up
  - Tested things out.  Oh man...did not go as planned.  Millions of fish everywhere and the penguin bouncing around the screen
  - Dig in and debug it tomorrow
- CoronaVirus Analytics:
  - Updated stats for the day

**Thoughts:**  
Working on some fun and interesting projects.  Excited to see how they pan out, and if they're able to perform useful forecasting (or at least make a fun game out of them).

**Link(s) to work:**
1. [Covid19 Simulator](https://github.com/BrianLeip/Covid19_Simulator/tree/2961ad2b307b74916d481d7f91d8577af569c677)
2. [Unity ML Agent Penguins - too many fish](https://github.com/BrianLeip/UnityMLAgentPenguins/tree/e23237de19c919d7fe002dc69f2e7fb48d7c9646)
3. [Coronavirus Analytics - Updated stats for the day](https://github.com/BrianLeip/CoronaVirus/blob/4cb04d76f796844a711b2a93e58128ffabe1481d/Covid19_Analytics.ipynb)

---

## R5-Dxx: March 27, 2020 - Friday

**Today's Progress:**  
- Came down with a pretty bad stomach bug.  Took day off.

**Thoughts:**  
Was worried it could be Coronavirus at first.  Fortunately it was just a stomach bug.  Took a breather then back at it on Saturday.  Count Saturday as day 10.

**Link(s) to work:**
1. [Coronavirus Analytics - Updated stats for the day](https://github.com/BrianLeip/CoronaVirus/blob/ac41c304f24b1faef31b00cbdd91f0ef2ba463ba/Covid19_Analytics.ipynb)

---

## R5-D09: March 26, 2020 - Thursday

**Today's Progress:**  
- Stanford Algorithms
  - Completed week 1 including challenge questions and programming challenge
- Unity ML Agents
  - Creating some Machine Learning agents in Unity.  Penguins, baby penguins, and fish.
  - About halfway through it so far. Should finish up tomorrow
- CoronaVirus Analytics
  - Updated stats for the day

**Thoughts:**  
Was tired, no matter.  Coded on.  
Excited to finish up this Unity ML Agents project see the results, and then play around and test different scenarios.

**Link(s) to work:**
1. [Stanford Algorithms - Week 1 complete](https://github.com/BrianLeip/Stanford-Algorithms-Cert/tree/c4d819a3eb50682070b26c31adc804204bc77682/01-Divide-Conquer/Week%201)
2. [Unity ML Agents - Halfway thorugh tutorial](https://github.com/BrianLeip/UnityMLAgentPenguins/tree/9450e5c08614c9621f8018f947b0b386e8b40d1d)
3. [Coronavirus Analytics - Updated stats for the day](https://github.com/BrianLeip/CoronaVirus/blob/2563deb10dffd7e583004f854b5e8a0d02595ad4/Covid19_Analytics.ipynb)

---

## R5-D08: March 25, 2020 - Wednesday

**Today's Progress:**  
- Stanford Algorithms
  - Week 1 challenge questions
- Coronavirus
  - Merged the John Hopkins (Global) and Covid Tracking Project (US States) datasets together into one jupyter notebook
  - Updated stats for 3/25
  - I'm predicting that the US will surpass both Italy and China to have the most confirmed Coronavirus cases by Friday 3/27
- Unity
  - Completed a few minigame tutorials and started on the Unity ML-Agent tutorial

**Thoughts:**  
Got a decent amount of coding done today, feels good.  But the looming threat of Coronavirus is threatening all that we hold dear.  Keep moving forward, that's all we can do.

**Link(s) to work:**
1. [Coronavirus Analytics - Combined JH and CTP datasets](https://github.com/BrianLeip/CoronaVirus/blob/170eeb69a3bdf034fd060094bc52f85ced93fb68/Covid19_Analytics.ipynb)

---

## R5-D07: March 24, 2020 - Tuesday

**Today's Progress:**  
- Stanford Algorithms
  - Finished week 1: Divide & conquer
  - Asymptotic Analysis
  - Big Oh Notation with mathematical proofs
  - Big Omega and Theta Notation with mathematical proofs

**Thoughts:**  
Did this on Tue but forgot to log it until Wed AM.  
Week 1 is done.  Course is till highly theoretical, not hands-on.  Hopefully that will change soon.

**Link(s) to work:**
1. [Stanford Algorithms - Week 1 Notes](https://github.com/BrianLeip/Stanford-Algorithms-Cert/blob/master/01-Divide-Conquer/Week%201%20-%20Divide%20%26%20Conquer.pdf)

---

## R5-D06: March 23, 2020 - Monday

**Today's Progress:**  
- Coronavirus Analysis
  - JH changed their live data format so adjusted for this
  - JH also deprecated their historic tracking data (non-global)
  - Created a new jupyter notebook using data from Covid Tracking Project and got the state data and charts caught up to where they were with the JH file

**Thoughts:**  
Spent a good chunk 2-3 hours on this today and got a lot done.  It's frustrating to see that JH is no longer tracking useful historic data but it is what it is.  Found a good alternative with the Covid tracking project.  

As I was going through the new data, I realized that Covid tracking only has US state data, and JH now only has global data.  So rather than using separate files I'll likely merge them together in the future.

**Link(s) to work:**
1. [Coronavirus - JH Global](https://github.com/BrianLeip/CoronaVirus/blob/a6ad81fe794b782a8ab479ec54390118f1569323/CoronaVirus%20-%20John%20Hopkins.ipynb)
2. [Coronavirus - Covid Tracking Project](https://github.com/BrianLeip/CoronaVirus/blob/a6ad81fe794b782a8ab479ec54390118f1569323/CoronaVirus%20-%20Covid%20Tracking%20Project.ipynb)

---

## R5-D05: March 22, 2020 - Sunday

**Today's Progress:**  
- Coronavirus EDA - Refreshed with updated data

**Thoughts:**  
Another difficult personal day with family issues.  Still got in a bit of coding.

**Link(s) to work:**
1. [Coronavirus EDA - Refreshed with updated data](https://github.com/BrianLeip/CoronaVirus/blob/c3c8c3947b4b2df4bc0b93a6cc5b7e500da941a9/CoronaVirus.ipynb)

---

## R5-D04: March 21, 2020 - Saturday

**Today's Progress:**  
- Coronavirus EDA - Added a new US state confirmed cases chart excluding New York to zoom in on the other states

**Thoughts:**  
Tough day today, dealing with some serious family issues.  Despite not wanting to, I still made time for a bit of coding.

**Link(s) to work:**
1. [Coronavirus EDA - Added US state confirmed cases](https://github.com/BrianLeip/CoronaVirus/blob/43062a049a508c343e4e70ae21ecc9e3ff6d69d4/CoronaVirus.ipynb)

---

## R5-D03: March 20, 2020 - Friday

**Today's Progress:**  
- More progress on the Stanford Algorithms and Data Structures course 1
  - Merge sort
  - Recursive calling
  - Calculating big O notation of merge sort vs insertion sort or bubble sort
- Added US State Coronavirus case tracking to my Coronavirus EDA Jupyter notebook

**Thoughts:**  
Most of the Stanford course has been video related so far.  It's good but I'm ready to get hands-on ASAP.  

Also, as Coronavirus spreads like wildfire and CA went on lockdown today, I spent some more time analyzing the John Hopkins University Covid-19 Data.  It's a bit messy (States are mixed with counties and cities), but after some data wrangling I was able to isolate the states and graph it on a chart.  New York is growing at a scary rate, and California is starting to wake up to the seriousness of this.

**Link(s) to work:**
1. [Progress on Stanford Algorithms and Data Structures]()
2. [Coronavirus EDA - Added US States confirmed case tracking](https://github.com/BrianLeip/CoronaVirus/blob/84be1066667a4d630f7209e749ea0e242e81b4b4/CoronaVirus.ipynb)

---

## R5-D02: March 19, 2020 - Thursday

**Today's Progress:**  
- Played around with a 2D map asset in Unity that I'd like to use to model Coronavirus outbreak.

**Thoughts:**  
A little detour from the Algorithms course, but was fun to play around in Unity again and get a feel for what I could create with the Map asset.

**Link(s) to work:**
1. [Unity 2D Maps](https://github.com/BrianLeip/WorldMapsPro2-Tests/commit/437482f0ff7db4e5000381355f5041f311297261)
---

## R5-D01: March 18, 2020 - Wednesday

**Today's Progress:**  
- Started the Stanford  Algorithms and Data Structures course on Coursera

**Thoughts:**  
Even though I've been coding over time, it feels good getting back into the 100 Days of Code flow and committing to doing it every day.  The daily habit is vital, even if it's only a little bit every day, and the 100 Days of Code community on Twitter is great.  Let's do this!

**Link(s) to work:**
1. [Progress on - Divide and Conquer, Sorting and Searching, and Randomized Algorithms](https://github.com/BrianLeip/Stanford-Algorithms-Cert)