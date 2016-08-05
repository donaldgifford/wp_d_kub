# wp_d_kub
Test repo for building a pipeline using chef -> packer-> docker->dockerhub->kubernetes(minikub)

The idea is to write all the code in chef which will then be committed with a
packer.json file to some CI tool to create a docker artifact from it that gets pushed
to the dockerhub. From there running minikub on my laptop ill pull down the three
images(wordpress, apache/nginx, mysql, maybe haproxy as well).

Using wp to demonstrate tiers in application in kubernetes with the pipeline
