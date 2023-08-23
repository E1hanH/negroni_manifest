	repo init -u git@github.com:E1hanH/negroni_manifest.git -b main

	mkdir .repo/local_manifests && wget https://github.com/E1hanH/negroni_manifest/blob/main/default.xml -O .repo/local_manifests/negroni.xml

	repo sync

	repo forall -c 'git lfs pull'