# Maven-CrashCourse
in this course i am not much going to explain about theory but practically how we can implement a maven project

# MavenWebProject:
================
File->New->Other->maven project->Next->Next->Enter the name as "webapp-jee5" in the filter section;

choose that artificate and create a maven webproject;

Note:Some times servlet-api maven depencies came along with the project wont work;For resolving the issue you can delete those
maven dependencies and new ones;


if you want to add any remote repository to your eclipse just go through following steps and add the reposiitory to find more archetypes:
File->New->Other->maven project->Next->Next->Configure->Add Remote Catlog->

* Catalog File:
https://repo.maven.apache.org/maven2/

Description:
RemoteReposiotry(you can give any convinient name);

#For creating standalone maven project:
=======================================
File->New->Other->maven project->Next->Next->type "maven-archetype-quickstart" filter the archetypes and select the archetype and
create your standalone maven project;
