	repo init -u https://github.com/LineageOS/android.git -b lineage-20.0 --git-lfs

	mkdir .repo/local_manifests && wget https://raw.githubusercontent.com/E1hanH/negroni_manifest/main/default.xml -O .repo/local_manifests/negroni.xml

	repo sync

	repo forall -c 'git lfs pull'
