TEIID Connector Arche Type
================

This maven project is the result of being created when the Teiid Connector Archetype is generated.  

When the project is generated, you should have ended up with the following structure:

-  connector-${connector-name}
	|-	kits
		|-	wildfly
			|-	docs
				|-	teiid-extensions
					|-	datasources
						|-	${connector-type}	
							|-	${connector-type}-ds.cli
							|-  ${connector-type}-ds.xml		
			|-	modules
				|-	${package}
					|-	main
						|-	module.xml
		|-	wildfly-dist.xml 
	| -	pom.xml
	| -	src
		|-	main
			|-	java
				|-	${package}
					|-	${connector-name}ConnectionImpl.java
					|-	${connector-name}ManagedConnectionFactory.java
					|-	${connector-name}Plugin.java
					|-	${connector-name}ResourceAdapter.java
			|-	rar
				|-	META-INF
					|-	MANIFEST.MF
					|-	ra.xml
			|-	resources
				|-	${package}
						|-	i18n.properties


Ready to begin adding your custom code.

NOTE:  The MANIFEST.MF will need to have its dependencies updated.  Example, adding
the translator dependency. 

