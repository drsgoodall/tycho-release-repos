tycho-release-repos
===================

This is an example set of projects showing how to maintain a single p2 release repository by rebuilding from individual p2 release repositories.

com.example.bundle-1.0.0 and com.example.bundle-2.0.0 are two versions of the same project. The first is version 1.0.0 and the second is identical but version 2.0.0. Install each of these in your local maven repo using "mvn package install".

The release-repo project can then be built using "mvn package". release-repo/repository will then contain a p2 repository combining both versions of com.example.bundle.