load("@bazel_tools//tools/build_defs/repo:http.bzl", "http_archive")

RULES_JVM_EXTERNAL_TAG = "4.3"
RULES_JVM_EXTERNAL_SHA = "6274687f6fc5783b589f56a2f1ed60de3ce1f99bc4e8f9edef3de43bdf7c6e74"

http_archive(
    name = "rules_jvm_external",
    sha256 = RULES_JVM_EXTERNAL_SHA,
    strip_prefix = "rules_jvm_external-%s" % RULES_JVM_EXTERNAL_TAG,
    url = "https://github.com/bazelbuild/rules_jvm_external/archive/%s.zip" % RULES_JVM_EXTERNAL_TAG,
)

load("@rules_jvm_external//:defs.bzl", "maven_install")

maven_install(
    artifacts = [
        "javax.servlet:javax.servlet-api:3.1.0",
        "org.apache.commons:commons-text:1.9",
        "mysql:mysql-connector-java:5.1.42",
        "com.mchange:c3p0:0.9.5.2",
        "org.jboss.weld:weld-core:1.1.33.Final",
        "org.apache.logging.log4j:log4j-core:2.3",
        "com.nqzero:permit-reflect:0.3",
        "org.jboss.arquillian.config:arquillian-config-spi:1.7.0.Alpha12",
	    "org.jboss.arquillian.container:arquillian-container-impl-base:1.7.0.Alpha12",
	    "org.jboss.shrinkwrap.descriptors:shrinkwrap-descriptors-api-base:2.0.0",
	    "org.jboss.shrinkwrap:shrinkwrap-impl-base:1.2.6",
	    "org.mockito:mockito-core:2.28.2",  
	    "com.google.errorprone:error_prone_annotations:2.7.1",  
	    "org.webjars.bowergithub.webcomponents:webcomponentsjs:2.0.0-beta.3",
	    "org.webjars.bowergithub.webcomponents:shadycss:1.9.1", 
	    "org.semver:api:0.9.33",
    ],
    repositories = [
        "https://repo1.maven.org/maven2",
    ],
)