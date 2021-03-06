---
title: "Fetching Exercises"
slug: "fetching-exercises"
category: "process"
ordinal: 10
---

First configure the command-line client:

```bash
exercism configure --key=YOUR_API_KEY
```

Note that there must be no spaces alongside `=` in the above command.
`configure --key = YOURKEY` or `configure --key= YOURKEY` will not work.

Your API key can be found in [your exercism.io account settings](http://exercism.io/account).

By default an exercism directory will be created for you in your home
directory the first time you fetch problems. There are some optional configuration
flags, see `exercism help configure` for more details.

The configuration is written to `~/.exercism.json`. This can be configured
using an environment variable named `EXERCISM_CONFIG_FILE`.

To fetch the first problem in each track, issue the command:

```bash
exercism fetch
```

Or you can fetch your current problems in a single track, for example Haskell:

```bash
exercism fetch haskell
```

To check which languages are available, and what to call them on the command line,
use the command:

```bash
exercism tracks
```

The program will download the exercises to the configured project directory.

Note that the code will be put in that directory even if you are somewhere else on the filesystem when calling `exercism fetch`.

To start working on an exercise, go find the downloaded files.

```bash
cd path/to/exercism/project # or whatever
```

You can work on them using your usual editor, tools, and environment. Read the <a class="link-side-menu" href="#sidr">getting started guide</a> of your language to find out how to run the tests.

As soon as you have submitted code to an exercise, `exercism fetch` will provide you with access to the next exercise.

If you need to update your downloaded files for an exercise, delete the files and fetch the exercises for that language again. The newer versions of the files will be downloaded.

If you're no longer working on the exercise, you may need to run `exercism restore` in order to re-download your solutions as well as the exercise files.

<a class="secondary-button" href="submitting-exercises.html">Submitting Exercises</a>
