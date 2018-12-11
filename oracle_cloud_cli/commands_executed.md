cat /dev/null > ~/.bash_history
curl -LSs https://raw.githubusercontent.com/fnproject/cli/master/install | sh
docker info
systemctl start docker
sudo systemctl start docker
sudo systemctl enable docker
sudo docker info
sudo groupadd docker
sudo usermod -aG docker opc
exit
oci
oci setup config
cat /home/opc/.oci/config
cat /home/opc/.oci/oci_api_key.pem
cat /home/opc/.oci/oci_api_key_public.pem
oci
oci compute instanse list
oci compute instanse list --compartment-id=ocid1.compartment.oc1..aaaaaaaaeaxlfmsduxm4jve2njhd76zkjdqemzz5mkvgrfugpjypzm3xnjha
oci compute instance list --compartment-id=ocid1.compartment.oc1..aaaaaaaaeaxlfmsduxm4jve2njhd76zkjdqemzz5mkvgrfugpjypzm3xnjha
which oci
oci config
vi ~/.oci/oci_cli_rc
oci setup oci-cli-rc
vi ~/.oci/oci_cli_rc
oci compute instance list
vi ~/.oci/oci_cli_rc
oci compute instance list
oci ce cluster create-kubeconfig --cluster-id=ocid1.cluster.oc1.phx.aaaaaaaaafstsnzymizgemldmjrwcyrwhe3wentbgjrdqyjwgc2dmmjwgftd --file=/home/opc/.kube/config
cat /home/opc/.kube/config
mkdir -p /home/opc/.kube/
oci ce cluster create-kubeconfig --cluster-id=ocid1.cluster.oc1.phx.aaaaaaaaafstsnzymizgemldmjrwcyrwhe3wentbgjrdqyjwgc2dmmjwgftd --file=/home/opc/.kube/config
kubectl get nodes -o wide