Hi, i'm the project 1

Ideas from : https://stackoverflow.com/questions/32203610/how-to-integrate-uml-diagrams-into-gitlab-or-github

For adding a plantuml diagram automatically generated and manageble under versionning follow this steps :
  - Create a diagram.puml file in your github repo : ex : https://github.com/14FRS851/Articles/blob/master/Project1/diagram.puml
  - Go to www.plantuml.com/plantuml/uml/
  - Create a diagram with the url of raw content (Suppress the "blob" in the url). Ex : https://raw.githubusercontent.com/14FRS851/Articles/blob/master/Project1/diagram.puml
  - See syntax :
''' Plantuml
@startuml
; For the file in 
!includeurl https://raw.githubusercontent.com/14FRS851/Articles/master/Project1/diagram.puml
@enduml

  - Copy the image URL from PlantUML.com's image (the image autogerated under the text description) : Ex : http://www.plantuml.com/plantuml/png/5Smz2W9130RGtbFe1JOCA8ZLsbYBdY1cmkx8_2p95xo-MhtkpGusHAkxG-bI8sjOtQ_0vXSYuy-q5Apn2bUJqQ4Taun6wNXxFC-dH5T3aQfEZHrgTBVnLa6YN7WnRjFspsVj-USN
  
  Then include it in the md file
  
  ![PlantUML model](http://www.plantuml.com/plantuml/png/5Smz2W9130RGtbFe1JOCA8ZLsbYBdY1cmkx8_2p95xo-MhtkpGusHAkxG-bI8sjOtQ_0vXSYuy-q5Apn2bUJqQ4Taun6wNXxFC-dH5T3aQfEZHrgTBVnLa6YN7WnRjFspsVj-USN)
  
  And bonus, we can hage the vector image too bu chnaging png in svg :
  
  ![PlantUML model](http://www.plantuml.com/plantuml/svg/5Smz2W9130RGtbFe1JOCA8ZLsbYBdY1cmkx8_2p95xo-MhtkpGusHAkxG-bI8sjOtQ_0vXSYuy-q5Apn2bUJqQ4Taun6wNXxFC-dH5T3aQfEZHrgTBVnLa6YN7WnRjFspsVj-USN)
