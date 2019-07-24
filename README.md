# VEP
https://useast.ensembl.org/info/docs/tools/vep/script/index.html

install VEP
sudo docker pull ensemblorg/ensembl-vep
sudo docker run -t -i ensemblorg/ensembl-vep ./vep

mkdir vep_data
chmod a+rwx vep_data    
sudo docker run -t -i -v vep_data:/opt/vep/.vep ensemblorg/ensembl-vep perl INSTALL.pl --NO_HTSLIB
