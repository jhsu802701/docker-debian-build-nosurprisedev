FROM debian:<CODE_NAME>

MAINTAINER No Surprise Dev

COPY usr_local_bin/* /usr/local/bin/

# sync: needed to avoid "text file busy" error
# wait: needed because the next command may be skipped without this command
RUN chmod +x /usr/local/bin/*; sync; wait; /usr/local/bin/<ABBREV>-root; wait
USER <REGULAR_USER>

WORKDIR /home/<REGULAR_USER>
