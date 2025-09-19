# pixl-convention-1

Event popup data
- Place event folders under `Events/` with any images or assets you want to show.
- Edit `Events/index.json` to list the events in the slideshow.

index.json format
- Either a top-level array or `{ "events": [...] }`
- Each event supports the following fields:
	- title: string
	- tag: string (e.g., location or category)
	- desc: short description
	- distance: string (optional)
	- hours: string (optional)
	- spot: string (optional)
	- hero: string (image path relative to project root, e.g., `Events/Foo/bar.avif`)

Notes
- If `Events/index.json` is missing or empty, the event popup hides itself.
- Large images are fine; they are used as CSS backgrounds and will be scaled to fit.