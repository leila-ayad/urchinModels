# urchinModels

###What it is###

Simplified predator-prey interaction

The reason for writing this model, at this time, is to show how a healthy, thriving kelp forest, can quickly become an urchin barren when the sunflower sea stars population drops. It models the predator-prey relationship between bull kelp, purple urchin and sunflower sea star in the kelp forest environment. Change the number of sunflower sea stars to zero to show how urchin can eat the entire kelp forest in just a few years. This shows the problem happening in many of the pacific kelp forests, where sea star populations have dropped to essentially zero.

There are many complex interactions that this model currently does not take into account.

1. Natural lifespan of the kelp, urchins or sea stars
2. Actual reproductive rate/success of offspring of kelp, urchins or sea stars
3. Bathymetry data to inform the movement of sea stars and urchins
4. Bathymetry data to inform where kelp can grow
5. Likelihood of death of kelp, urchins or sea stars by means other than predation
6. Actual rate of predation of urchins to kelp and sea stars to urchins

###How it works###

Urchins and seastars wander through the kelp forest consuming their respective prey. Urchin wander randomly, consuming kelp when they are located on the same patch. Seastars wander randomly until they are within 2 patches of an urchin, then their behavior changes to face the angle the sea urchin is moving. Kelp are stationary on their patch.

In this model, one tick represents one day. The rate that the urchin and sea stars move through the environment is estimated to achieve the rate the urchin would eat kelp and sea stars would be urchin in a single day.

After 365 ticks (or 365 days), the kelp, urchin and seastar all respawn. Kelp and urchin respawn relative to how many turtles of that type exist when the model reaches 365 ticks. The number of sea stars, which are immortal in this model with no predators, increases by 2 every 365 ticks if there are sea stars in the model.
