FROM britesnow/base-node:23-02-10
 
RUN apt-get -y update && \
    apt-get install -y ffmpeg 

# install libvips (for sharp) - But, not needed apparently since sharp download its version.
# && apt-get install -y libvips-dev 

## -Dev takes quite a bit of space. Need to see if 
# && apt-get install -y libopencv-dev
