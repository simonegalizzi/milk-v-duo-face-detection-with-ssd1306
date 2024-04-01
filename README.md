# milk-v-duo-face-detection-with-ssd1306
The test program will pull the camera data, add the face detection algorithm, and use tools such as VLC to pull the stream in real time to view the effect with display 1306 128x32
SDK_VER: musl_riscv64
TDL SDK library path: /home/simo/host-tools/cvitek-tdl-sdk-cv180x/lib
TDL SDK include path: /home/simo/host-tools/cvitek-tdl-sdk-cv180x/include
Middleware include path: /home/simo/host-tools/cvitek-tdl-sdk-cv180x/sample/3rd/middleware/v2/include
Middleware library path: /home/simo/host-tools/cvitek-tdl-sdk-cv180x/sample/3rd/middleware/v2/lib
IVE library path: /home/simo/host-tools/cvitek-tdl-sdk-cv180x/sample/3rd/ive/lib
IVE include path: /home/simo/host-tools/cvitek-tdl-sdk-cv180x/sample/3rd/ive/include
TPU library path: /home/simo/host-tools/cvitek-tdl-sdk-cv180x/sample/3rd/tpu/lib

Download toolchain:

wget https://sophon-file.sophon.cn/sophon-prod-s3/drive/23/03/07/16/host-tools.tar.gz
tar xvf host-tools.tar.gz
cd host-tools
export PATH=$PATH:$(pwd)/gcc/riscv64-linux-musl-x86_64/bin

compile:

git clone https://github.com/milkv-duo/cvitek-tdl-sdk-cv180x.git
cd cvitek-tdl-sdk-cv180x

move font,i2c-dev,ssd1306,linux_i2c to ../host-tools/cvitek-tdl-sdk-cv180x/sample/3rd/tpu/lib

compie sample:

cd sample
./compile_sample.sh
