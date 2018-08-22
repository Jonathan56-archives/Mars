# Mars
A project aiming to optimize spacecrafts payload and schedule to create a human settlement on Mars.

```python
List of inputs:
# Duration and quantity to reach
nb_synodic_period = 50
synodics = range(0, nb_synodic_period)
nb_people_to_reach = 1000000
mass_per_people = 10

# Spaceship constraints [kg]
cargo_capacity = 1000
one_way_propellant = 10
spaceship_growth_factor = 2
max_spaceship_to_mars_at_first = 5

# Production rate per factory [kg/cycle]
prod_per_factory_per_cycle = {}
prod_per_factory_per_cycle['propellant'] = 10
prod_per_factory_per_cycle['cement'] = 100
prod_per_factory_per_cycle['steel'] = 100
prod_per_factory_per_cycle['food'] = 100
prod_per_factory_per_cycle['water'] = 100
prod_per_factory_per_cycle['powerplant'] = 10
prod_per_factory_per_cycle['steel_factory'] = 10
prod_per_factory_per_cycle['cement_factory'] = 10
kW_per_mass_of_powerplant = 10
birth_per_person_per_cycle = 0.1

# Weight of a factory [kg/factory]
mass_per_factory = {}
mass_per_factory['propellant'] = 100
mass_per_factory['cement'] = 200
mass_per_factory['steel'] = 200
mass_per_factory['food'] = 100
mass_per_factory['water'] = 100
mass_per_factory['power'] = 100
mass_per_factory['powerplant'] = 100
mass_per_factory['steel_factory'] = 100
mass_per_factory['cement_factory'] = 100

# Weight of resources to sustain human life [kg/person]
mass_required_per_person = {}
mass_required_per_person['food'] = 1
mass_required_per_person['water'] = 1
mass_required_per_person['cement'] = 1
mass_required_per_person['steel'] = 1
mass_required_per_person['power'] = 1
mass_required_per_person['other'] = 0.1

# Power required to produce resources [kW/factory]
power_per_factory = {}
power_per_factory['propellant'] = 10
power_per_factory['cement'] = 10
power_per_factory['steel'] = 10
power_per_factory['food'] = 1
power_per_factory['water'] = 5
power_per_factory['powerplant'] = 10
power_per_factory['cement_factory'] = 10
power_per_factory['steel_factory'] = 10


# Ressource required to produce another ressource [kg/kg]
mass_r1_to_produce_r2 = {}
mass_r1_to_produce_r2['steel'] = {}
mass_r1_to_produce_r2['steel']['powerplant'] = 1
mass_r1_to_produce_r2['steel']['steel_factory'] = 1
mass_r1_to_produce_r2['steel']['cement_factory'] = 1
mass_r1_to_produce_r2['cement'] = {}
mass_r1_to_produce_r2['cement']['powerplant'] = 1
mass_r1_to_produce_r2['cement']['steel_factory'] = 1
mass_r1_to_produce_r2['cement']['cement_factory'] = 1
mass_r1_to_produce_r2['propellant'] = {}
mass_r1_to_produce_r2['propellant']['steel'] = 0.001
mass_r1_to_produce_r2['propellant']['cement'] = 0.001
mass_r1_to_produce_r2['water'] = {}
mass_r1_to_produce_r2['water']['propellant'] = 0.01
mass_r1_to_produce_r2['other'] = {}
mass_r1_to_produce_r2['other']['steel_factory'] = 100
mass_r1_to_produce_r2['other']['cement_factory'] = 100

# Set of resources
resource_names = ['propellant', 'cement', 'steel', 'people',
                 'food', 'water', 'steel_factory',
                 'propellant_factory', 'cement_factory',
                 'food_factory', 'water_factory', 'powerplant',
                 'powerplant_factory', 'other',
                  'factory_steel_factory', 'factory_cement_factory']
```
