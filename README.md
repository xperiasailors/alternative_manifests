# alternative_manifests
This is an attempt to create a set of modular/minimalist repo manifests to build mer-hybris/droid-hal.  

To use (assuming you already have repo installed), copy the files in manifests to your .repo/manifests directory, and likewise copy the files in local_manifests to your .repo/local_manifests directory (create the directory if needed).

Then, initialize repo to the cm12.1 tree as normal:

repo init -u https://github.com/CyanogenMod/android.git -b cm-12.1

and then overwride the default manifest:
repo init -m manifest_default_hybris_cm_12_1.xml

The files in the local_manifests will automatically be picked up by repo (no action needed).
