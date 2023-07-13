# 1. clone codes.
```bash
cd ~/work
git clone https://github.com/zaazbb/hidparser.git
```

# 2. modify codes from lufa. (no need normally)
```bash
# see www.lufa-lib.org
wget http://www.github.com/abcminiuser/lufa/archive/LUFA-210130.zip
unzip lufa-LUFA-210130.zip
cp lufa-LUFA-210130/LUFA/Drivers/USB/Class/Common/HIDClassCommon.h lufa-LUFA-210130/LUFA/Drivers/USB/Class/Common/HIDParser.c lufa-LUFA-210130/LUFA/Drivers/USB/Class/Common/HIDParser.h lufa-LUFA-210130/LUFA/Drivers/USB/Class/Common/HIDReportData.h hidparser
# modify codes to independent other lufa codes.
```

# 3. build
```bash
cd hidparser
mkdir build
cd build
cmake .. -DCOMPILEPATH=${compiler-path}/bin
camke --build .
```

