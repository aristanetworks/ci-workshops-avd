.PHONY: help
help: ## Display help message
	@grep -E '^[0-9a-zA-Z_-]+\.*[0-9a-zA-Z_-]+:.*?## .*$$' $(MAKEFILE_LIST) | sort | awk 'BEGIN {FS = ":.*?## "}; {printf "\033[36m%-30s\033[0m %s\n", $$1, $$2}'

########################################################
# Campus A
########################################################

.PHONY: ping-campus-a
ping-campus-a: ## Ping Nodes
	ansible-playbook playbooks/ping.yml -i sites/campus_a/inventory.yml -e "target_hosts=CAMPUS_A_FABRIC"

.PHONY: build-campus-a
build-campus-a: ## Build Configs
	ansible-playbook playbooks/build.yml -i sites/campus_a/inventory.yml -e "target_hosts=CAMPUS_A_FABRIC"

.PHONY: eapi-campus-a
eapi-campus-a: ## Deploy Configs via eAPI
	ansible-playbook playbooks/eapi.yml -i sites/campus_a/inventory.yml -e "target_hosts=CAMPUS_A_FABRIC"

.PHONY: deploy-campus-a
deploy-campus-a: ## Deploy Configs via CloudVision Static Configuration Studio
	ansible-playbook playbooks/deploy.yml -i sites/campus_a/inventory.yml -e "target_hosts=CAMPUS_A_FABRIC"

.PHONY: validate-campus-a
validate-campus-a: ## Validate network state
	ansible-playbook playbooks/validate.yml -i sites/campus_a/inventory.yml -e "target_hosts=CAMPUS_A_FABRIC"


########################################################
# Hosts - Lab Prep
########################################################

.PHONY: preplab
preplab: ## Deploy Preparation Configs via eAPI
	ansible-playbook playbooks/preplab.yml -i extra_configs/inventory.yml -e "target_hosts=LAB"
