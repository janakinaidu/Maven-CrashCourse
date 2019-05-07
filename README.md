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


#How to add RemoteCatalog
========================
Go to Eclipse ==> Windows ==> Preferences ==>Maven ==>Click on 'Remote catalog'
    
      Catalog      https://repo.maven.apache.org/maven2/
      Description: myRemoteRepo
      
 you can give any name fro description;click on verify to test the artificats and ok.
 
 Note If you want to practice maven projects in parallel with your projects exisitng in your office,then you might face some build issues that existing  repository will not accept your current versions of artifcats/groupid versions.so it is better to add
 a new settings.xml file for your practice and you can find it in files section.and give a path where you want to store the jar files.
 like below:
 
    <settings xmlns="http://maven.apache.org/SETTINGS/1.0.0"
      xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
      xsi:schemaLocation="http://maven.apache.org/SETTINGS/1.0.0
                          https://maven.apache.org/xsd/settings-1.0.0.xsd">
      <interactiveMode/>
      <offline/>
      <pluginGroups/>
      <servers/>
      <mirrors/>
      <proxies/>
      <profiles/>
      <activeProfiles/>
	  <localRepository>D:\settings\customrepo</localRepository>
    </settings>
    
    Here i choosed the path as : D:\settings\customrepo to store the dependecies.
    
    
For More information regarding pom.xml file properties refer below link:
https://maven.apache.org/settings.html

Note:
-----
 ->After creating a maven project,If you are not found src/amin/resources folder, righclick on your project and go to  'new' 
   and click on 'source folder' and now add 'src/main/resource' as a folder name;
   
->if you are not found even 'src/main/java' folder then you can rightclick on your project and click on properties search for 
   'project facets' makesure select java and others if you require ,click on Apply and ok.Now you will get project structure as you    expected.
   
->And sometimes this will be resolved by:rightclick on your project--->properties-->buildpath-configure buildpath-->
   in 'Orders and Export' tab just check the Maven Dependencies option.
   so finally issue will be resolved by any of the above options.
