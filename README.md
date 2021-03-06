# Template for creating a blockchain infrastructure in Azure
This template creates an infrastrucutre for blockchain in Azure. Orchestrator of this deployment is Ansible. It requires Ansible 2.4 or newer. Worker of this deployment are ARM templates in json. Azure credentials are stored in credentials file and authentication requires [service principal](https://docs.microsoft.com/en-us/azure/active-directory/develop/active-directory-application-objects).

* [ansible-template-1dc](https://github.com/luberan/blockchain-ansible-template/tree/master/ansible-template-1dc) creates the infrastructure in one Azure datacenter.
* [ansible-template-2dc](https://github.com/luberan/blockchain-ansible-template/tree/master/ansible-template-2dc) creates the infrastructure in multiple Azure datacenters.
* [ethereum-original-arm-template](https://github.com/luberan/blockchain-ansible-template/tree/master/ethereum-original-arm-template) is the original template downloaded from [Azure Marketplace](https://azuremarketplace.microsoft.com/en-us/marketplace/apps/microsoft-azure-blockchain.azure-blockchain-service?tab=Overview).

Besides the infrastructure it also deploys go-ethereum client to all nodes and starts mining on mining nodes. It also includes "admin" webpage for checking status of the infrastructure.