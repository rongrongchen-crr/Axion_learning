# Axion_learning
Document the processing of '.spk' and '.raw' data specific to the Axion device, such Axis data.

# Import Data

## Tools
The required AxIS Navigator raw files can be downloaded from [AxionFileLoader](https://github.com/axionbio/AxionFileLoader).

其中，Raw数据是使用Axion设备记录的原始数据，spk数据主要是针对记录过程中的spike信号的数据

## Load A Raw数据

```matlab
  FIledata = AxisFile('Filename.raw');
  # 加载一个raw数据结构，其中包含数据采集时
  # 输入到 AxIS 的文件名和其他实验注释（RecordingName、Investigator 和 Description）、板条形码、板图以及与文件关联的任何标签事件

  RecordingName = FileData.RecordingName;
  Investigator = FileData.Investigator;
  Description = FileData.Description;
  Barcode = FileData.Barcode;

```

