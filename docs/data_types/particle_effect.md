# Particle Effect
[Data Type](../data_types.md)

A data type that's either a [string](string.md) which defines only the particle type or an [object](object.md) which defines the particle type and its additional parameters.
!!! note
    
  Refer to the [Minecraft Fandom Wiki: Particles (Particle IDs)](https://minecraft.fandom.com/wiki/Particles#Particle_IDs) page for a list of **vanilla** particle type IDs that you can use.
### Fields

 | Field | Type | Default | Description | 
|---|---|---|---|
 | `type` | [Identifier](identifier.md) |   | The namespace and ID of the particle type. | 
 | `params` | [String](string.md) |   | The additional parameter for the particle type. | 

