package(default_visibility = ["//visibility:public"])

load("//tools/springboot:springboot.bzl",
        "springboot",
        "add_boot_jetty_starter",
        "add_boot_web_starter",
        "add_boot_actuator_starter"
)

app_deps = [
  "@commons_logging_commons_logging//jar",
  "@com_fasterxml_classmate//jar",
  "@org_hibernate_hibernate_validator//jar",
  "@com_fasterxml_jackson_core_jackson_annotations//jar",
  "@com_fasterxml_jackson_core_jackson_core//jar",
  "@com_fasterxml_jackson_core_jackson_databind//jar",
  "@org_jboss_logging_jboss_logging//jar",
  "@org_slf4j_jcl_over_slf4j//jar",
  "@org_slf4j_jul_to_slf4j//jar",
  "@org_slf4j_log4j_over_slf4j//jar",
  "@ch_qos_logback_logback_classic//jar",
  "@ch_qos_logback_logback_core//jar",
  "@org_slf4j_slf4j_api//jar",
  "@org_yaml_snakeyaml//jar",
  "@org_springframework_spring_webmvc//jar",
  "@javax_validation_validation_api//jar",
]

# Convenience Methods for Adding Entire Starters
add_boot_jetty_starter(app_deps)
add_boot_web_starter(app_deps)
add_boot_actuator_starter(app_deps)

# Build the app
springboot(
    name = "spring-boot-sample-jetty",
    boot_app_class = "hello.Application",
    deps = app_deps
)
