provider "aws" {
profile = "default"
region = "AsiaPacific(Mumbai)ap-south-1"
}
resource"aws_s3_bucket" "tf_course"{
bucket = "sanilawsbucket"
}
acl = "public"
}
resource "aws_s3_bucket" {
bucket = "sanilawsbucket.hashicorp.com"
acl = "public read"
policy = file("policy.json")
website {
index_document = "index.html"
error-document = "rror.html"
}
}
resource "aws_s3_bucket"
bucket = "sanilawsbucket"
acl ="private"
versioning {
enabled = "true"
}
} 
