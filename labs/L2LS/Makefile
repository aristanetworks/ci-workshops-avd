.PHONY: help
help: ## Display help message
	@grep -E '^[0-9a-zA-Z_-]+\.*[0-9a-zA-Z_-]+:.*?## .*$$' $(MAKEFILE_LIST) | sort | awk 'BEGIN {FS = ":.*?## "}; {printf "\033[36m%-30s\033[0m %s\n", $$1, $$2}'

########################################################
# Site 1
########################################################

.PHONY: ping-site-1
ping-site-1: ## Ping Nodes
	ansible-playbook playbooks/ping.yml -i sites/site_1/inventory.yml -e "target_hosts=SITE1_FABRIC"

.PHONY: build-site-1
build-site-1: ## Build Configs
	ansible-playbook playbooks/build.yml -i sites/site_1/inventory.yml -e "target_hosts=SITE1_FABRIC"

.PHONY: deploy-site-1
deploy-site-1: ## Deploy Configs via eAPI
	ansible-playbook playbooks/deploy.yml -i sites/site_1/inventory.yml -e "target_hosts=SITE1_FABRIC"

.PHONY: cvp-site-1
cvp-site-1: ## Deploy Configs via eAPI
	ansible-playbook playbooks/cvp1.yml -i sites/site_1/inventory.yml

########################################################
# Site 2
########################################################

.PHONY: ping-site-2
ping-site-2: ## Ping Nodes
	ansible-playbook playbooks/ping.yml -i sites/site_2/inventory.yml -e "target_hosts=SITE2_FABRIC"

.PHONY: build-site-2
build-site-2: ## Build Configs
	ansible-playbook playbooks/build.yml -i sites/site_2/inventory.yml -e "target_hosts=SITE2_FABRIC"

.PHONY: deploy-site-2
deploy-site-2: ## Deploy Configs via eAPI
	ansible-playbook playbooks/deploy.yml -i sites/site_2/inventory.yml -e "target_hosts=SITE2_FABRIC"

.PHONY: cvp-site-2
cvp-site-2: ## Deploy Configs via eAPI
	ansible-playbook playbooks/cvp2.yml -i sites/site_2/inventory.yml

########################################################
# WAN & Hosts - Lab Prep
########################################################

.PHONY: preplab
preplab: ## Deploy Configs via eAPI
	ansible-playbook playbooks/preplab.yml -i extra_configs/inventory.yml -e "target_hosts=LAB"

########################################################
# Fast forward CICD
########################################################

.PHONY: cicd-ff
cicd-ff: ## Copy complete files for CICD
	cp -a complete/site_1/group_vars/. sites/site_1/group_vars/ && \
	cp -a complete/site_2/group_vars/. sites/site_2/group_vars/ && \
	cp -a complete/global_vars/. global_vars/
