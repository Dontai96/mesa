# Flockers

This is an implementation of Craig Reynolds's Boids flocker model. Agents (simulated birds) try to fly towards the average position of their neighbors and in the same direction as them, while maintaining a minimum distance. This produces flocking behavior.

This model tests Mesa's continuous space feature and uses numpy arrays to represent vectors. It also demonstrates how to create custom visualization components.

## How to Run

Launch the model:
```
    $ python run.py
```

Then open your browser to [http://127.0.0.1:8521/](http://127.0.0.1:8521/) and press Reset, then Run.

## Files

* [flockers/model.py](flockers/model.py): Core model file; contains the BoidModel class.
* [flockers/boid.py](flockers/boid.py): The Boid agent class.
* [flockers/SimpleContinuousModule.py](flockers/SimpleContinuousModule.py): Defines ``SimpleCanvas``, the Python side of a custom visualization module for drawing agents with continuous positions.
* [flockers/simple_continuous_canvas.js](flockers/simple_continuous_canvas.js): JavaScript side of the ``SimpleCanvas`` visualization module; takes the output genereated by the Python ``SimpleCanvas`` element and draws it in the browser window via HTML5 canvas.
* [flockers/server.py](flockers/server.py): Sets up the visualization; uses the SimpleCanvas element defined above
* [run.py](run.py) Launches the visualization.
* [Flocker Test.ipynb](Flocker Test.ipynb): Tests the model in a Jupyter notebook.

## Further Reading

*none*
