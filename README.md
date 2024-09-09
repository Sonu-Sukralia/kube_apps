sudo k3s ctr images import /tmp/airflow-custom.tar

udo k3s ctr images list

sudo scp airflow-custom.tar pis@192.168.29.25:/tmp/airflow-custom.tar

docker save -o airflow-custom.tar airflow-custom:1.0.0

sudo k3s ctr images list | grep airflow-custom

sudo k3s crictl images
