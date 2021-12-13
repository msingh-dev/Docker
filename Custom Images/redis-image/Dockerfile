# Use an existing docker image as Base

FROM alpine

# Download and install a dependency
RUN apk add --update redis

# Tell the image what to do when it starts
#as a container
CMD [ "redis-server" ]


# Series of Steps happened in background:

# 1. Download alpine image
# --------------------------------------------
# 2. Get Image from the previous Steps
# 3. Create a container out of it. 
# 4. Run "apk add --update redis" in it.
# 5. Take snapshot of that container's FS.
# 6. Shutdown that temporary container.
# 7. Get Image ready for the next instruction.
# ----------------------------------------------
# 8.  Get image from the last step.
# 9. Create a contianer out of it. 
# 10. Tell container it should run 'redis-server' when started.
# 11. Shutdown that temporary container.
# 12. Get Image ready fro next instruction.
# 13. No more steps !
# 14. Output is th eimage generated from previous step.

