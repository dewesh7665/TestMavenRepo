mvn deploy:deploy-file 
		#this specifies the artificat and will (=should) match with your dependency-declaration in pom.xml	
		-DgroupId=com.google.android.apps 
		-DartifactId=analytics 
		-Dversion=1.3.1 \ 
		-Dpackaging=jar \ #deploy as jar 
		-Dfile="libGoogleAnalytics.jar" \ #source file to deploy
		-Durl=file:../../dev/mavenrepo/releases #target folder to deploy
		
		
		
$ mvn install:install-file \
    -DgroupId=com.actionbarsherlock \
    -DartifactId=actionbarsherlock \
    -Dversion=4.3.2-SNAPSHOT \
    -DgeneratePom=true \
    -Dpackaging=aar \
    -Dfile=build/libs/actionbarsherlock-4.3.2-SNAPSHOT.aar \
    -DlocalRepositoryPath=/path/to/myapp/libs
    
    
mvn deploy:deploy-file 
		-DgroupId=com.lbr.libs
		-DartifactId=feedlibrary 
		-Dversion=1.0.0 \ 
		-Dpackaging=aar \ #deploy as aar 
		-Dfile="app-release.aar" \ #source file to deploy
		-Durl=file:///Users/Dewesh_MAC/Desktop/Work/Projects/Android/FeedLibraryGit #target folder to deploy