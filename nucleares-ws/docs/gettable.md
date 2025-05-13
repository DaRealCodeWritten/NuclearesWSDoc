# Gettable Variables
## Time Variables
### `TIME`
Returns the time of day in-game<br>  
Format: `string`

### `TIME_DAY`
Returns the days since start of save in-game<br>  
Format: `float`

### `TIME_STAMP`
Returns the time of day as a timestamp<br>  
Format: `float`

## Core Variables
### `CORE_TEMP`
Returns core temperature<br>  
Format: `float`

### `CORE_TEMP_OPERATIVE`
Returns the ideal core temperature given the core operative mode  
Format: `float`

### `CORE_TEMP_RESIDUAL`
Returns true or false if the core temperature is residual  
Format: `string, bool`

### `CORE_PRESSURE`
Returns core pressure in BARs  
Format: `float`

### `CORE_INTEGRITY`
Returns core integrity as a percentage  
Format: `float`

### `CORE_WEAR`
Returns core wear as a percentage  
Format: `float`

### `CORE_STATE`
Returns whether the core is reactive or not  
`NOREACTIVO`: Core is not reactive  
`REACTIVO`: Core is reactive  
Format: `string`

### `CORE_STATE_CRITICALITY`
Returns the core's reactivity from -5 to 5  
`-5`: Core is very subcritical  
`0`: Core is critical (No reactivity change)  
`5`: Core is very supercritical

### `CORE_CRITICAL_MASS_REACHED`
Returns whether the core has reached critical mass  
Format: `string, bool`

### `CORE_CRITICAL_MASS_REACHED_COUNTER`
Returns how many times the core has reached critical mass (Number of startups)  
Format: `int`

### `CORE_IMMINENT_FUSION`
Returns whether the core is about to melt down (Meltdown timer)  
Format: `string, boolean`

### `CORE_READY_FOR_START`
Returns whether the core is ready to start (Ready to begin operations)  
Format: `string, boolean`

### `CORE_STEAM_PRESENT`
Returns whether there is steam in the core  
Format: `string, boolean`

### `CORE_HIGH_STEAM_PRESENT`
Returns whether there is a lot of steam in the core  
Format: `string, boolean`

## Coolant Variables
### `COOLANT_CORE_STATE`
Returns the state of the primary circuits as a string  
`CIRCULANDO`: Primary circuit is circulating   
`INMOVIL`: Primary circuit is not circulating  
Format: `string`

### `COOLANT_CORE_PRESSURE`
Returns the pressure of the core coolant in BARs  
Format: `float`

### `COOLANT_CORE_VESSEL_TEMPERATURE`
Returns the temperature of the coolant measured in the core  
Format: `float`

### `COOLANT_CORE_QUANTITY_IN_VESSEL`
Returns the volume of coolant in the core, in liters  
Format: `float`

### `COOLANT_CORE_PRIMARY_LOOP_LEVEL`
Returns the overall primary circuit coolant level as a percentage  
Format: `float`

### `COOLANT_CORE_FLOW_SPEED`
Returns the average primary circuit flow speed as a percentage of the max  
Format: `float`

### `COOLANT_CORE_ORDERED_SPEED`
Returns the ordered flow speed for the primary circuit as an average of the max  
Format: `float`

### `COOLANT_CORE_FLOW_REACHED_SPEED`
Returns whether all pumps in the primary circuit have reached their ordered speed  
Format: `string, bool`

### `COOLANT_CORE_CIRCULATION_PUMP_X_STATUS`
Returns the status of the given pump (X), where X is 0, 1, or 2 (A, B, C respectively)  
`0`: Inactive  
`1`: Active, no speed reached  
`2`: Active, speed reached  
`3`: Requires maintenance  
`4`: Not installed  
`5`: Insufficient energy   
Format: `int`

### `COOLANT_CORE_CIRCULATION_PUMP_X_DRY_STATUS`
Returns the dry status of the given pump (X), where X is 0, 1, or 2 (A, B, C respectively)  
`1`: Pump is dry (no water to pump)  
`4`: Pump is not dry (Inactive, or has water)  
Format: `int`

### `COOLANT_CORE_CIRCULATION_PUMP_X_OVERLOAD_STATUS`
Returns the overload status of the given pump (X), where X is 0, 1, or 2 (A, B, C respectively)  
`1`: Pump is overloaded  
`4`: Pump is inactive or not overloaded  
Format: `int`

### `COOLANT_CORE_CIRCULATION_PUMP_X_ORDERED_SPEED`
Returns the ordered speed of the given pump (X), where X is 0, 1, or 2 (A, B, C respectively)  
Format: `int`

### `COOLANT_CORE_CIRCULATION_PUMP_X_SPEED`
Returns the actual speed of the given pump (X), where X is 0, 1, or 2 (A, B, C respectively)  
Format: `int`

## Rods Variables
### `RODS_STATUS`