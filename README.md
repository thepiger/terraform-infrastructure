# terraform-infrastructure
Repository di risorse terraform
Per utilizzare le risorse in questa repository bisogna istanziarle come moduli all'interno del nostro progetto

module "frontend" {
  source = "git::git@github.com:gruntwork-io/infrastructure-modules.git//frontend-app?ref=v0.0.1"

# importante #
ogni volta che aggiungiamo un modulo al progetto, prima di fare il plan o l'apply, bisogna lanciare:
  terraform get
