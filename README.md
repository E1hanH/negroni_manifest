	repo init -u git@github.com:E1hanH/negroni_manifest.git -b main

	mkdir .repo/local_manifests && wget https://raw.githubusercontent.com/E1hanH/negroni_manifest/main/default.xml -O .repo/local_manifests/negroni

	repo sync

	repo forall -c 'git lfs pull'