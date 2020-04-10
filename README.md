This project tests the public availability of fuse-eap artifacts through the redhat GA repository. 
Most relevant are the feature packs because they have transitive dependencies on everything else that is in the product distro.

We assume, that if a pom for a given artifact is accessible, the associated binary is accessible too.

When this runs in a CI environment, make sure that no other (perhaps even internal) repos leak into the config.
This would nullify the intended verification result.  
