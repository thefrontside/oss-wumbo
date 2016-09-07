Yee-haw! It's time for the weekly Frontside OSS roundup! And with Rob out on vacation, he's helpless to stop me from stocking the update with a corral-full of tired cowboy tropes. So strap on your chaps buckaroos, it's time to herd some open source!

This week we've got updates from Chris, Stephanie, Charles and Alex who've been working in myriad different areas of the Frontside open source world.

Chris has been focused on the x-form library and its supporting substructures. `x-form` is a complete form solution that provides a data model for the entire form submission process, from clean/dirty states, to validation, to change buffering. It's an exciting problem that has flummoked the JS world for years and years, and he's in the process of making it an easy thing.

Meanwhile, Stephanie has been working on the website to so that visitors can look at the content we produce by category. That way, if they want to focus on blogs, welp, we'll show 'em blogs. Podcast's your thing? We can show you those too.

Charles on the other hand has been chasing microstates dragon, getting microstates to play well within other microstates. That means, if you have a state machine that represents a Promise, you could take a bunch of those Promise state machines and say, put them in a list.

Which brings us to Alex. Alex has been taking all the lessons learned over the past year from our studies in immutability and diligantly applying them to the impagination library. It's gonna defy previous definitions of robustness and flexibility.

### Chris

 Last week, I attended ElixirConf and stoked the flames of my relentless pursuit of having too many side-projects. While I was there, I also started working on a small library called `ChangeBuffer` that will hopefully serve as the future foundation of `x-form`.

 In the next few weeks I hope to hammer down the `ChangeBuffer` library and write out docs for `x-form`.

### Stephanie

The acceptance tests are passing, mirage is working, and the images are now being rendered using Faker. I'm debating what the next step is, perhaps that should be creating routes for the filters. We also need to have the hard conversation of what the data set will look like- how will we pull podcasts, blogs, and talks in?


### Charles

I got the nested microstates working! I got the nested microstates working! The British are coming! I got the nested microstates working!

What this means will become clear since I'm signed up to give a lunch and learn on Friday on just what the hell microstates are at the low-level, but suffice it to say that it's a really huge blocker that got wiped off my plate. What remains now is to document it, merge it, and then open it up so that others can begin to add other core features like states for `Number`, `Bool`, `Date`, etc...

While I'm not going to commit to finishing my blog post on microstates, I will commit to finishing two of the tech-demos for the blog post and if all those things happen, then that will be enough!
