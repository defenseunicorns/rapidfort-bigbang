# rapidfort-bigbang
Integrate RapidFort with BigBang


AWS info:

terraform {
  backend "s3" {
    bucket         = "rapidfort-bigbang-tf-state"
    key            = "infra/terraform.tfstate"
    region         = "us-west-2"
    dynamodb_table = "rapidfort-bb-infra-terraform-state-lock"
  }