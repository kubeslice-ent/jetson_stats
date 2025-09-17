@Library('jenkins-library@opensource-helm-multiarch') _
dockerImagePipeline(
  script: this,
  services: ['jetson_stats'],
  dockerfiles: ['Dockerfile'],
  pushed: true,
  run_unit_tests: 'false',
  buildArgumentsList: [
    [ENV: 'production', PLATFORM: 'linux/arm64,linux/amd64']
]
)
