# tidal 👻
tidal music 下载并使用 gclone 上传到 GoogleTeamDrive

## Installation

Python3.6+的版本

```
pip install -r requirements.txt
```
安装配置gclone
修改main.py
## Usage

```
python3 main.py track the great gig in the sky
python3 main.py album the dark side of the moon
python3 main.py artist pink floyd
python3 main.py url https://tidal.com/browse/track/140538043
python3 main.py getall https://listen.tidal.com/artist/-1-100  #下载https://listen.tidal.com/artist/1 到https://listen.tidal.com/artist/100的所有
```

## Configuration

默认配置文件为 `./config.toml`
如果用其它的配置文件 `--config-file <file>`.

###参数详解###

- `username <username>`: 账户. 
- `password <password>`: 密码.
- `quality <quality>`: 下载质量 (`master` > `lossless` > `high` > `low`). 默认 `master`
- `output-directory <path>`: 下载位置 `./output`
- `by-id`: 通过ID下载. 如, `python3 main.py --by-id 79419393`.
- `lucky`: 自动下载热门搜索结果. 默认 `false`.
- `search-count <number>`: 搜索结果前多少条. 默认 `16`.
- `quiet`: 不看日志. 默认 `false`.
- `nice-format`: 重命名下载后的文件名.如: "Maxwell's Silver Hammer (Remastered).mp3" to "maxwells-silver-hammer-remastered.mp3".
- `full-structure`: 按艺术家和专辑来创建目录。
- `skip-metadata`: 不下载封面信息和标签.

## License

[The Unlicense](https://unlicense.org)
