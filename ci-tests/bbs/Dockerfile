FROM kanapi-sbs:ci
MAINTAINER Jacek Danecki <jacek.m.danecki@gmail.com>
RUN mkdir /kanapi_build/kanapi
COPY kanapi /kanapi_build/kanapi
ENV CI="true"
RUN mkdir -p ${HOME}/ci_src; cd /kanapi_build/kanapi/kanapi_system/kanapi-bbs; ./install all-sbs verbose
CMD ["/bin/bash"]
