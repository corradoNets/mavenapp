---
config:
  node: "linux && prod"

build:
  type: "s2i" #available: maven, npm, mobile_android, mobile_ios, no_build
  skiptest: true
  loglevel: "info" # available: info, debug, error

#build:
#  type: "maven" #available: maven, npm, mobile_android, mobile_ios, no_build
#  jdk_version: "8"
#  mvn_version: "3.3.3"
#  skiptest: true
#  loglevel: "info" # available: info, debug, error
#  pre_action:
#    type: sh # available: bat, powershell, sh
#    command: "ls -la"
#  post_action:
#    type: sh # available: bat, powershell, sh
#    command: "ls -la"

#configuration_file:
#  repo_name: "CONFIGURATION-FILES"
#  tag_version: "prod" # available: prod , v1.0.0 , v1.0.0-rc0

quality:
  sonar:
    active: false

deployment:
  openshift:
    active: true

notification:
    #email: "c.colombo@netswgroup.com" # available: indirizzo email
    #when : always # available: always
