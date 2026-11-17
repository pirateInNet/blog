+++
title = "My first try with Motion Canvas"
date = 2026-10-10

[taxonomies]
categories = ["programming"]
tags = ["JavaScript/TypeScript", "vedio making"]

[extra]
toc = true
+++

documenting my journey learning how to use that tool.

<!-- more -->

firstly

## why I will use MotionCanvas?
ok, I said in [About me](../about-me/), that to learn something, you should explain it,
& animated vids is really good for explaining things.


## why specifically that tool?
- [a vid shows why](https://www.youtube.com/watch?v=4kjEwvrDKlg&t=37s)

## the roadmap to learn it
- Learn X in Y minutes
	- [Where X=JavaScript](https://learnxinyminutes.com/javascript/)
	- [Where X=TypeScript](https://learnxinyminutes.com/typescript/)
1. [x] **JavaScript basics:** Use MDN’s [JavaScript Guide](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide).
	- [x] variables
	- [x] functions
	- [x] arrays
	- [x] objects
	- [x] imports/exports (Modules).
2. [x] **TypeScript essentials:** Use the [TypeScript Handbook](https://www.typescriptlang.org/docs/handbook/); focus on “Everyday Types” and “Object Types.”
	- [x] setup TypeScript workspace or just use a typescript playground
		- [x] `clear && sudo apt install npm nodejs -y`
		- [x] `npm init`
		- [x] `npm install typescript --save-dev`
		- `cat package.json`
		```json
		{
		  "name": "test",
		  "version": "1.0.0",
		  "description": "TypeScript test",
		  "main": "index.js",
		  "scripts": {
		    "test": "echo \"Error: no test specified\" && exit 1"
		  },
		  "author": "YBD",
		  "license": "ISC",
		  "devDependencies": {
		    "typescript": "^7.0.2"
		  }
		}
		```
		- `micro index.ts`
		- `npx tcs index.ts` to run the TypeScript file
		- `node index.js`
	- [x] basic types
	- [x] functions
	- [x] interfaces.
3. [x] **JSX basics:** Use the Motion Canvas [documentation and examples](https://canvascommons.io/docs/quickstart?language=tsx#programming-an-animation) to see JSX in context; you don’t need to learn React first.
	- [x] Learn how tags and expressions describe visual elements.
4. [x] **Animation basics:** Follow the code examples in the [Motion Canvas tutorial series](https://slama.dev/motion-canvas/).
	- [x] setup it, (damn, npm install takes too much time)
	```sh
	$ npm init @canvas-commons@latest
	Need to install the following packages:
	  @canvas-commons/create@0.4.0
	Ok to proceed? (y) y
	✔ Project name … my-animation-1
	✔ Project path … my-animation-1
	✔ Language › TypeScript (Recommended)
	✔ How would you like to render your animation? › Image sequence, Video (WebCodecs)

	√ Scaffolding complete. You can now run:
	  cd my-animation-1
	  npm install
	  npm start
	$ npm config set fetch-timeout 600000
	$ npx get-pnpm # only if you want to use pnpm
	```
	- [x] Practice position
	- [x] scale
	- [x] opacity
	- [x] timing
	- [x] and easing.
5. [x] **Motion Canvas API:** Use the [Motion Canvas docs](https://canvascommons.io/docs/) alongside the tutorial examples.
	- [x] scenes
	- [x] shapes
	- [x] text
	- [x] layout
	- [x] signals
	- [x] effects
	- [x] references
6. [x] **Project workflow:** Use the setup and project guides in the Motion Canvas docs.
	- [x] Learn to run the preview, organize scenes, sync audio, and export.
	- `ffmpeg -framerate 60 -i %06d.png -c:v libx264 -pix_fmt yuv420p -crf 18 out.mp4`

7. [x] **make something on your own**
    - [x] 1 vid
    - [x] put it in YT
    - [x] put the code in GitHub


## what I made using it
### bubble sort explaining
***
#### code :

```python
# bubble sort
# 1 - make a random array
from random import randint as rn

array = []
for i in range(0, rn(5, 10)):
    array.append(rn(0, 100))
print(f"""
the array is {array}
length is {len(array)}
""")
# 2 - sort it
end_point = len(array) - 1
step = 1
while end_point != 0 and len(array) > 1:
    for i in range(0, end_point):
        if array[i] > array[i + 1]:
            array[i], array[i + 1] = array[i + 1], array[i]
        print(f"step {step}:{array} & end_point = {end_point}")
        step += 1
    end_point -= 1
```
#### Explaining :
- [YT](https://www.youtube.com/watch?v=TJwa8Q3H8rQ)
- [GitHub](https://github.com/pirateInNet/canvas-commons_Work/tree/main/my-animation-1)

***

all that was just for relearning how to learn by myself, It's fucked up
