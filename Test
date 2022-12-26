locals {
  app_name              = var.app_name
  environment_code      = var.environment_code
  name_prefix           = "${local.environment_code}_${local.app_name}_"
  vpc_name              = var.vpc_name
  front_end_subnet_name = var.front_end_subnet_name
  app_subnet_name       = var.app_subnet_name

  //AppStream Image Builder values
  image_builder_base_image_name = var.image_builder_base_image_name
  image_builder_instance_type   = var.image_builder_instance_type

  //AppStream Fleet values
  desired_fleet_instances_count            = var.desired_fleet_instances_count
  fleet_type                               = var.fleet_type
  fleet_max_user_duration_in_seconds       = var.fleet_max_user_duration_in_seconds
  fleet_disconnect_timeout_in_seconds      = var.fleet_disconnect_timeout_in_seconds
  fleet_idle_disconnect_timeout_in_seconds = var.fleet_idle_disconnect_timeout_in_seconds
  fleet_image_name                         = var.fleet_image_name
  fleet_instance_type                      = var.fleet_instance_type

  // default tags
  tag_buc              = var.tag_buc
  tag_support_group    = var.tag_support_group
  tag_app_group_email  = var.tag_app_group_email
  tag_environment_type = var.tag_environment_type
  tag_customer_crmid   = var.tag_customer_crmid

  //mapping tag keys to FCS standard and organizing tags into maps: 
  default_tags = tomap({
    "AppGroupEmail"   = local.tag_app_group_email
    "BUC"             = local.tag_buc
    "CustomerCRMID"   = local.tag_customer_crmid
    "EnvironmentType" = local.tag_environment_type
    "SupportGroup"    = local.tag_support_group
  })

}
