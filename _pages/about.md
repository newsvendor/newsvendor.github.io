---
layout: about
title: about
permalink: /
subtitle: Free. Open Source. <a href='https://donate.doctorswithoutborders.org/secure/donate'>Buy me a coffee ☕</a>

profile:
  align: right
  image: newsvendor.png
  address: >


news: false  # includes a list of news items
selected_papers: false # includes a list of papers marked as "selected={true}"
social: false  # includes social icons at the bottom of the page
---

This website offers a **a game that allows you to experience the [newsvendor's problem](https://en.wikipedia.org/wiki/Newsvendor_model).** The game runs within a **[Pluto](https://github.com/fonsp/Pluto.jl)** notebook for **[Julia](https://julialang.org)**.

The game comes with a **[mini case](https://github.com/frankhuettner/newsvendor/blob/main/scenarios/cheers_1_story.md),** which puts you into the shoes of a patisserie owner. Every day, you have to make a choice about how many cakes 🍰🍥🎂 you want to produce. 
     
#### Let's Go!
Setup takes 15 min for installing Julia, Pluto, and some packages (mostly unattendet). It requires about 1 GB disk space. 

1. Download Julia **[from the official website](https://julialang.org/downloads/)** and install it with the standard settings.
2. Copy the code below. 
```
  begin
  # Download the notebook into a temporary directory
  nb = download("https://raw.githubusercontent.com/frankhuettner/newsvendor/main/simulation/newsvendorsimulation.jl", joinpath(mktempdir(), "newsvendorsimulation.jl"))
  # Install Pluto
  import Pkg;	Pkg.add("Pluto")
  # Start Pluto and load the notebook
  import Pluto; Pluto.run(notebook=nb)
  end
 ```
3. Start Julia (e.g. in the Windows Start Menu)
4. Rightclick into the Julia window. This will paste the code that you copied above. Hit the <kbd>Enter</kbd> key to execute the code.
5. Now wait for 10 minutes. Julia will install Pluto and download the simulation. After about 5 minutes, it opens your browser and you see fragments of the simulation. It will install further packages and is finished once the animations stop. Get a ☕ or 🍵 or use your computer for something else while waiting (*do **not** close the Julia window*).
