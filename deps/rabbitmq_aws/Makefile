PROJECT = rabbitmq_aws
PROJECT_DESCRIPTION = A minimalistic AWS API interface used by rabbitmq-autocluster (3.6.x) and other RabbitMQ plugins
PROJECT_REGISTERED = rabbitmq_aws

define PROJECT_ENV
[]
endef

LOCAL_DEPS = crypto inets ssl xmerl public_key
BUILD_DEPS = rabbit_common
# We do not depend on rabbit therefore can't run the broker.
DEP_PLUGINS = rabbit_common/mk/rabbitmq-build.mk
TEST_DEPS = meck

include ../../rabbitmq-components.mk
include ../../erlang.mk
