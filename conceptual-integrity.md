# Conceptual Integrity
Is the principle that anywhere you look in your system, you can tell that the design is part of the same overall design.
This includes low-level issues such as formatting and identifier naming, but also issues such as how modules and classes
are designed, etc.

# Metrics
- List of design patterns and styles to be used.
- Afferent coupling (Ca): value.
  The number of types outside this assembly that depend on types within this assembly.
  High afferent coupling indicates that the concerned assemblies have many responsibilities.
- Efferent coupling (Ce): The number of types outside this assembly used by child types of this assembly.
  High efferent coupling indicates that the concerned assembly is dependent.
  Notice that types declared in third-party assemblies are taken into account.
  
# General Metrics
- Efferent coupling (Ce): < 0.2 (deprecated metric in sonar)
- Afferent coupling (Ca): < 0.2 (Package Tangle in Sonar Qube) 

# Tools
- SonarQube