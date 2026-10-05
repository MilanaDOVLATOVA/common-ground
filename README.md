# Common Ground

**Live site:** https://milanadovlatova.github.io/common-ground/

An axonometric site model where nobody designs the landscape. People walking between doors wear paths into the grass, and the places where they stop grow benches and then trees. Move a door, plant a hedge or add a bus stop, and the landscape redraws itself around the new routes.

It opens already running: a campus block with a new library (in gold), a studio hall, labs, a café, a bus stop and two crossings, surrounded by white context massing in the style of an architectural axonometric. People are articulated figures that walk, sit on benches and sit on the grass; cars, a bus and traffic lights run on the street.

## The rules, in plain language

1. **Walk to a door.** Everyone goes from one door to another by the shortest way.
2. **Follow the footprints.** Worn grass is easier to walk on, so busy paths get busier. Paths nobody uses grow back.
3. **Rest where it's lively.** People stop beside busy paths, in shade, near seats and food. Where many stop, a bench appears, then a tree.

On the street, each car keeps a safe gap to the one ahead and stops at red lights, so queues form on their own. When the bus stops, a wave of people gets off and floods the paths.

**What emerges:** a network of desire paths nobody drew, benches and trees gathering where people linger, and corners nobody uses. The gold layer on the ground shows where people are walking right now; the worn grass shows where they have walked for a while.

## Move things and watch the flow change

Everything on the site can be dragged: doors, the food kiosk, benches, picnic tables, seat walls, trees, bike racks and lamp posts. People re-route within seconds, and the gold flow layer shows the change straight away; the worn paths follow more slowly. You can also place new furniture from the palette:

| Furniture | What it does |
|---|---|
| Door | A new destination; on the street edge it becomes a bus stop |
| Food kiosk | A new destination that also draws people to rest nearby |
| Bench, picnic table, seat wall | Places to sit; picnic tables draw the most people |
| Tree | Shade, which draws people who stop to rest |
| Hedge | A barrier people have to walk around |
| Bike rack, lamp post | Obstacles that bend the paths |

## How it fits the design process

This is a site-planning and landscape tool. Before drawing paths, let people find them: see where the routes want to go, where people will gather, and which corners will be left empty. Then test a change, such as moving the library door or adding a crossing, and see how the ground responds.

## Controls

| Action | How |
|---|---|
| Move anything by dragging it | Move tool, key M |
| Place a door, food kiosk, bench, picnic table, seat wall, tree, hedge, bike rack or lamp post | Palette, keys D, K, B, P, W, T, G, R, L |
| Erase | Key X |
| Number of people, how often they stop, how strongly they follow paths, grass regrowth, number of cars, speed | Sliders |
| Turn the view a quarter turn | Q and E, or the view buttons |
| Zoom | Scroll |
| Pause, clear the ground, download an image, record a 10 s teaser, hide the panel | Buttons, or Space and H |

## Things to try

- Drag the food kiosk into the middle of the lawn.
- Drag the library door to the other side of the building.
- Drag a tree or seat wall into the busiest route.
- Add a second bus stop on the street edge with the Door tool.

## Sources and techniques

- Desire paths and stigmergy: walkers leave traces that guide later walkers, like ant trails. Helbing, D., Keltsch, J. and Molnár, P. (1997). "Modelling the evolution of human trail systems." *Nature* 388.
- William H. Whyte, *The Social Life of Small Urban Spaces* (1980): people sit where other people pass, and shade and seating draw them.
- *The Nature of Code*, autonomous agents and flow-field following. Each door has a shortest-route field computed with Dijkstra's algorithm.
- Car following: each car adjusts its speed to the gap ahead, a simplified version of traffic models like Treiber's Intelligent Driver Model.
- Drawn in three.js with an orthographic (axonometric) camera; figures, cars and furniture are instanced meshes animated every frame.

## Making it with Claude

<!-- Write this in your own words: which choices were yours, what you changed after seeing it run, and how you'd explain the four rules without the screen. -->

## Running it

A single `index.html` with no build step. Open it in a browser, or host it with GitHub Pages: Settings, then Pages, then deploy from the `main` branch root.
