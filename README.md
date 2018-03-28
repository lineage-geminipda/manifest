LineageOS 14.1 for Planet Gemini PDA
------------------------------------

Create directories

	$ mkdir cm-14.1
	$ cd cm-14.1

the local manifests:

	$ repo init -u git://github.com/LineageOS/android.git -b cm-14.1
	$ git clone https://github.com/lineage-geminipda/local_manifest -b cm-14.1 .repo/local_manifests

Then sync up with this command:

	$ repo sync --force-sync -q

-------------
 
_Building from source_
---------------

	$ . build/envsetup.sh
	$ lunch lineage_geminipda-userdebug
	$ make bacon