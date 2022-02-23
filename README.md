# kata-hyperledger-fabric
learn DApp by doing

- https://mycoralhealth.medium.com/start-your-own-hyperledger-blockchain-the-easy-way-5758cb4ed2d1
- https://mycoralhealth.medium.com/build-a-dapp-on-hyperledger-the-easy-way-178c39e503fa
- https://hyperledger-fabric.readthedocs.io


-------- podman support ----

- https://github.com/hyperledger/fabric-samples/pull/596

this does not work. 
- curl -sSL https://raw.githubusercontent.com/hyperledger/fabric/main/scripts/bootstrap.sh | bash -s 

solution:

podman pull docker.io/hyperledger/fabric-tools:2.4
docker tag hyperledger/fabric-tools:2.4 hyperledger/fabric-tools:latest

podman pull docker.io/hyperledger/fabric-peer:2.4
podman tag hyperledger/fabric-peer:2.4 hyperledger/fabric-peer:latest

podman pull docker.io/hyperledger/fabric-orderer:2.4
podman tag hyperledger/fabric-orderer:2.4 hyperledger/fabric-orderer:latest


