
META_DIR := ../..
DIR := TOOL/Net
TEST_CLASS := TOOLNet
JAVA := /usr/bin/java

.PHONY: all clean run

all:
	$(MAKE) -C $(META_DIR) $(DIR)

clean:
	$(RM) *.class

run:
	$(MAKE) -C $(META_DIR) run

test:	all
	cd $(META_DIR) && $(JAVA) $(DIR)/$(TEST_CLASS)

%.class: %.java
	$(MAKE) -C $(META_DIR) $(DIR)/$@
