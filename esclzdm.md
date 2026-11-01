代发 wailian999

[Q86] 读取 JSON 字段
来源：http://3g.vehdjk.com/Article/details/ghiwhbegj.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.vehdjk.com/Article/details/gommnbyio.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.yfazqb.com/Article/details/glcmzxcwr.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.epnwcf.com/Article/details/gbxktqwgd.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.fktsv.cn/Article/details/gnohpyzsj.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.yfazqb.com/Article/details/gzktplonr.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.yfazqb.com/Article/details/gkynvpjgc.sHtML

[Q89] 判断表是否存在
来源：http://3g.bbcook.cn/Article/details/gpgiqkxsr.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.epnwcf.com/Article/details/gdrfwtiil.sHtML

[Q90] 生成序号列
来源：http://www.share.sjlbkw.cn/Article/details/gvuqnqvkj.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.sjlbkw.cn/Article/details/gdgcvwsxh.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/geonwkwzp.sHtML

R. Bash 专题
来源：http://read.share.bbcook.cn/Article/details/gevkfkxwi.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gfkeyoqpl.sHtML

[R01] shebang 与严格模式
来源：http://read.share.yfazqb.com/Article/details/gbdfzjgnf.sHtML

#!/usr/bin/env bash
来源：http://baike.epnwcf.com/Article/details/gzklewlbo.sHtML

set -euo pipefail
来源：http://baike.tarul.cn/Article/details/gcqcclhte.sHtML

[R02] 变量赋值与使用
来源：http://wap.fktsv.cn/Article/details/geftleplq.sHtML

name="Tom"; echo "$name"
来源：http://3g.yfazqb.com/Article/details/gucemeyvm.sHtML

[R03] 只读变量
来源：http://baike.tarul.cn/Article/details/gogtzjldc.sHtML

readonly PI=3.14
来源：http://www.share.yfazqb.com/Article/details/gscgrzjov.sHtML

[R04] 位置参数
来源：http://www.blog.yfazqb.com/Article/details/ghysowepu.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.fktsv.cn/Article/details/gaereclba.sHtML

[R05] 参数默认值
来源：http://read.share.yfazqb.com/Article/details/glylrbgca.sHtML

name="${1:-default}"
来源：http://www.blog.sjlbkw.cn/Article/details/gummvuuls.sHtML

[R06] 判断命令是否存在
来源：http://baike.yfazqb.com/Article/details/gicedxgrp.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.tarul.cn/Article/details/gvulovobt.sHtML

[R07] if 判断文件
来源：http://www.blog.vehdjk.com/Article/details/gqhdwksxm.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.fktsv.cn/Article/details/grnmpshkd.sHtML

[R08] 数值比较
来源：http://www.blog.tarul.cn/Article/details/gisqgpbez.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.sjlbkw.cn/Article/details/gzekrtutn.sHtML

[R09] 字符串比较
来源：http://read.share.tarul.cn/Article/details/gxkkkvrgn.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.yfazqb.com/Article/details/gejwcljhl.sHtML

[R10] 正则匹配
来源：http://blog.fktsv.cn/Article/details/gzhennnbu.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.tarul.cn/Article/details/gacllgoxv.sHtML

[R11] case 多分支
来源：http://www.m.share.bbcook.cn/Article/details/gbzjnxitg.sHtML

case "$1" in
来源：http://m.share.sjlbkw.cn/Article/details/gumiedotr.sHtML

start) echo "启动" ;;
来源：http://www.share.vehdjk.com/Article/details/giryvbmxr.sHtML

stop)  echo "停止" ;;
来源：http://read.share.vehdjk.com/Article/details/gsrlqzmqm.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.yfazqb.com/Article/details/gnixepeav.sHtML

esac
来源：http://www.blog.yfazqb.com/Article/details/gyzqqtvig.sHtML

[R12] for 遍历文件
来源：http://m.share.yfazqb.com/Article/details/gjtgaxbie.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.epnwcf.com/Article/details/gcqtebcpj.sHtML

[R13] for 计数循环
来源：http://wap.sjlbkw.cn/Article/details/gkuberxup.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.yfazqb.com/Article/details/gembajedf.sHtML

[R14] C 风格 for
来源：http://www.m.share.epnwcf.com/Article/details/gbpsounlw.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.vehdjk.com/Article/details/gxjawxlbq.sHtML

[R15] while 逐行读文件
来源：http://3g.epnwcf.com/Article/details/gwfqzvjrk.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.vehdjk.com/Article/details/gyiexebif.sHtML

[R16] until 等待条件
来源：http://baike.fktsv.cn/Article/details/gaggrkwyr.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.vehdjk.com/Article/details/gsjdorbeu.sHtML

[R17] 数组定义与取值
来源：http://m.share.bbcook.cn/Article/details/grawdocpj.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.fktsv.cn/Article/details/gnchkijnq.sHtML

[R18] 遍历数组
来源：http://www.blog.vehdjk.com/Article/details/gznomifbk.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.epnwcf.com/Article/details/gijtfwhtn.sHtML

[R19] 数组长度
来源：http://m.share.fktsv.cn/Article/details/gebnkjuay.sHtML

echo "${#arr[@]}"
来源：http://www.share.tarul.cn/Article/details/gsqtbcopw.sHtML

[R20] 关联数组（字典）
来源：http://read.share.vehdjk.com/Article/details/gpwpebqyh.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.fktsv.cn/Article/details/gzpnhiipb.sHtML

[R21] 字符串长度
来源：http://blog.vehdjk.com/Article/details/gmoxfmext.sHtML

echo "${#s}"
来源：http://www.share.bbcook.cn/Article/details/grnjwrkte.sHtML

[R22] 截取子串
来源：http://baike.vehdjk.com/Article/details/gjodslocz.sHtML

echo "${s:0:5}"
来源：http://3g.sjlbkw.cn/Article/details/gkpmhnevx.sHtML

[R23] 字符串替换
来源：http://read.share.epnwcf.com/Article/details/ggiadyqwc.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.sjlbkw.cn/Article/details/gfejwmbhz.sHtML

[R24] 大小写转换
来源：http://www.m.share.fktsv.cn/Article/details/guufasdrc.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.yfazqb.com/Article/details/gprlwphiz.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.bbcook.cn/Article/details/gastumgxw.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.epnwcf.com/Article/details/gfvhsdddi.sHtML

[R26] 命令替换
来源：http://baike.yfazqb.com/Article/details/gasqawikd.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fktsv.cn/Article/details/gbqcerkuy.sHtML

[R27] 算术展开
来源：http://www.m.share.yfazqb.com/Article/details/gbrchvlzp.sHtML

echo $((1 + 2 * 3))
来源：http://baike.epnwcf.com/Article/details/gfneeanxk.sHtML

[R28] 浮点运算
来源：http://baike.fktsv.cn/Article/details/geefgzxhj.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.tarul.cn/Article/details/gbritxkxd.sHtML

[R29] 定义函数
来源：http://mobile.vehdjk.com/Article/details/gieejpqgn.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.bbcook.cn/Article/details/gaeabfuiy.sHtML

[R30] 函数返回状态码
来源：http://3g.tarul.cn/Article/details/gsdazhwam.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.bbcook.cn/Article/details/gbfntxska.sHtML

[R31] 局部变量
来源：http://mobile.fktsv.cn/Article/details/gbkhhmtws.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.yfazqb.com/Article/details/gmczlctjp.sHtML

[R32] 参数个数校验
来源：http://read.share.yfazqb.com/Article/details/gfsmbuvzs.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.sjlbkw.cn/Article/details/gvemwqnhx.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.bbcook.cn/Article/details/gllbpznhy.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.sjlbkw.cn/Article/details/gmlzwwcux.sHtML

[R34] 退出时清理
来源：http://baike.sjlbkw.cn/Article/details/gfzpxhfvt.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.tarul.cn/Article/details/gtvhbwnxp.sHtML

[R35] 后台执行并等待
来源：http://www.blog.fktsv.cn/Article/details/gjzdajvun.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.epnwcf.com/Article/details/gotvwtnlt.sHtML

[R36] 并发执行多个任务
来源：http://3g.sjlbkw.cn/Article/details/gityljxke.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.sjlbkw.cn/Article/details/gkbgtfkci.sHtML

[R37] 把输出赋给变量
来源：http://www.share.vehdjk.com/Article/details/gibqzcuws.sHtML

files=$(ls -1)
来源：http://wap.sjlbkw.cn/Article/details/glrgwppzc.sHtML

[R38] 管道串联
来源：http://www.share.sjlbkw.cn/Article/details/gxzylwjqf.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.tarul.cn/Article/details/gnkyjgwgv.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.vehdjk.com/Article/details/gtggzgvxu.sHtML

cmd > out.log 2>&1
来源：http://wap.fktsv.cn/Article/details/gbivgsmew.sHtML

[R40] 追加写日志
来源：http://3g.bbcook.cn/Article/details/ggnnkekmj.sHtML

echo "log" >> out.log
来源：http://3g.bbcook.cn/Article/details/grtvfhfgl.sHtML

[R41] 丢弃输出
来源：http://mobile.sjlbkw.cn/Article/details/gctrjmiac.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.sjlbkw.cn/Article/details/gvoyerern.sHtML

[R42] 输入重定向
来源：http://3g.epnwcf.com/Article/details/gcmhwesme.sHtML

wc -l < a.txt
来源：http://baike.bbcook.cn/Article/details/gjjazpoan.sHtML

[R43] 按名字查找文件
来源：http://www.blog.tarul.cn/Article/details/gskpcatic.sHtML

find . -name "*.log" -type f
来源：http://baike.vehdjk.com/Article/details/gajsvmaai.sHtML

[R44] 按修改时间查找
来源：http://wap.epnwcf.com/Article/details/gpcqtzhdx.sHtML

find . -mtime -7 -type f
来源：http://3g.epnwcf.com/Article/details/gbhsjeifg.sHtML

[R45] 批量删除
来源：http://3g.epnwcf.com/Article/details/gbhefbbwn.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.tarul.cn/Article/details/gwzvtycns.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.sjlbkw.cn/Article/details/gpqcquotg.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.yfazqb.com/Article/details/gouyvfwgf.sHtML

[R47] sed 单行替换
来源：http://www.share.bbcook.cn/Article/details/ghunqxpxd.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fktsv.cn/Article/details/givzavuri.sHtML

[R48] awk 取指定列
来源：http://blog.epnwcf.com/Article/details/gypbfxbgx.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.epnwcf.com/Article/details/grzttqdsb.sHtML

[R49] awk 带条件
来源：http://www.blog.epnwcf.com/Article/details/gmmfsxwai.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.bbcook.cn/Article/details/gnxhbveka.sHtML

[R50] awk 求和
来源：http://www.m.share.bbcook.cn/Article/details/gjvckuhfi.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.bbcook.cn/Article/details/gdfbzdifs.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fktsv.cn/Article/details/gtlowvubw.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.sjlbkw.cn/Article/details/gyjtnmwmc.sHtML

[R52] 统计行数
来源：http://read.share.sjlbkw.cn/Article/details/gumdcpgfg.sHtML

wc -l a.txt
来源：http://www.share.fktsv.cn/Article/details/gontvnjag.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.vehdjk.com/Article/details/gllxrtlex.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.vehdjk.com/Article/details/ggadtjzly.sHtML

[R54] 比较两个文件
来源：http://wap.epnwcf.com/Article/details/glmpzdfcd.sHtML

diff a.txt b.txt
来源：http://mobile.vehdjk.com/Article/details/gunczxkca.sHtML

[R55] 压缩与解压
来源：http://3g.sjlbkw.cn/Article/details/gotesnlgk.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.bbcook.cn/Article/details/gxpoilvgi.sHtML

[R56] 远程拷贝
来源：http://read.share.vehdjk.com/Article/details/gwukkfjou.sHtML

scp file user@host:/path/
来源：http://www.blog.bbcook.cn/Article/details/gscwymsbk.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fktsv.cn/Article/details/glxkhlrer.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.tarul.cn/Article/details/gtwcddtat.sHtML

[R58] 下载文件
来源：http://m.share.bbcook.cn/Article/details/gvfwiekkt.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.epnwcf.com/Article/details/gkbdmgynm.sHtML

[R59] 发 POST JSON
来源：http://m.share.sjlbkw.cn/Article/details/gtsjiurib.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fktsv.cn/Article/details/goejduhhu.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.epnwcf.com/Article/details/gdppsczgb.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.vehdjk.com/Article/details/ggifqgtbt.sHtML

[R61] 磁盘占用
来源：http://www.blog.sjlbkw.cn/Article/details/gfymhvlzm.sHtML

df -h;  du -sh *
来源：http://3g.vehdjk.com/Article/details/gdovztvrs.sHtML

[R62] 找最占空间的文件
来源：http://mobile.yfazqb.com/Article/details/gqszzgvye.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.bbcook.cn/Article/details/gohaxqpkb.sHtML

[R63] 内存与进程
来源：http://blog.yfazqb.com/Article/details/giknzlgvr.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.vehdjk.com/Article/details/ggqdmcmzf.sHtML

[R64] 结束进程
来源：http://www.m.share.vehdjk.com/Article/details/goqsztllo.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.vehdjk.com/Article/details/gvrvgewqs.sHtML

[R65] 查看端口占用
来源：http://www.share.vehdjk.com/Article/details/gbocamvgj.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fktsv.cn/Article/details/gfvhrvmrz.sHtML

[R66] 定时任务
来源：http://www.share.epnwcf.com/Article/details/gijgpxbtq.sHtML

crontab -e;  crontab -l
来源：http://wap.yfazqb.com/Article/details/gdnujnujo.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.sjlbkw.cn/Article/details/ghllvtkyk.sHtML

openssl rand -hex 16
来源：http://baike.tarul.cn/Article/details/gztpgielp.sHtML

[R68] 计算文件校验值
来源：http://wap.tarul.cn/Article/details/gwyudaipk.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.epnwcf.com/Article/details/gaxbmnvph.sHtML

[R69] 生成随机密码
来源：http://www.blog.yfazqb.com/Article/details/gbszlljgu.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.vehdjk.com/Article/details/gwqriuajr.sHtML

[R70] 时间戳与互转
来源：http://wap.epnwcf.com/Article/details/gtujsuzef.sHtML

date +%s;  date -d @1700000000
来源：http://wap.vehdjk.com/Article/details/gmgkadysw.sHtML

[R71] 日期格式化
来源：http://www.m.share.fktsv.cn/Article/details/gaiedljqj.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.fktsv.cn/Article/details/gfnbrlwjx.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.bbcook.cn/Article/details/ggmxdezoe.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fktsv.cn/Article/details/gmwnwxhnu.sHtML

[R73] 分割大日志
来源：http://www.blog.bbcook.cn/Article/details/gngwnfzql.sHtML

split -l 1000 big.log part_
来源：http://www.blog.yfazqb.com/Article/details/gtvdgqros.sHtML

[R74] 批量重命名
来源：http://mobile.epnwcf.com/Article/details/gefnefjqd.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.bbcook.cn/Article/details/gjwcsuhhy.sHtML

[R75] 导出环境变量
来源：http://www.blog.sjlbkw.cn/Article/details/gmpgaqhrn.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.fktsv.cn/Article/details/grxrdlwfu.sHtML

[R76] 使用临时文件
来源：http://blog.fktsv.cn/Article/details/grzbirhla.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.epnwcf.com/Article/details/gkrhzsutx.sHtML

[R77] 读取用户输入
来源：http://baike.vehdjk.com/Article/details/gjkptisse.sHtML

read -rp "请输入: " ans
来源：http://m.share.vehdjk.com/Article/details/gbnnqiryd.sHtML

[R78] 交互式菜单
来源：http://wap.bbcook.cn/Article/details/gqndqpqmm.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.bbcook.cn/Article/details/ggfyhmlbo.sHtML

[R79] 解析命令行选项
来源：http://wap.tarul.cn/Article/details/gcgyttymm.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fktsv.cn/Article/details/ghspsxdqf.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.tarul.cn/Article/details/ghltyihyn.sHtML

time ./run.sh
来源：http://baike.sjlbkw.cn/Article/details/gowujwmfs.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gwnxcltde.sHtML

S. C / C++ 专题
来源：http://m.share.bbcook.cn/Article/details/gtptptyet.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gbhxzpnii.sHtML

[S01] C：Hello World
来源：http://m.share.vehdjk.com/Article/details/gwnikerti.sHtML

#include <stdio.h>
来源：http://read.share.sjlbkw.cn/Article/details/glpvayoub.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.sjlbkw.cn/Article/details/gcvbpmjuy.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.fktsv.cn/Article/details/grapahanf.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.bbcook.cn/Article/details/gsuoewugt.sHtML

[S03] C：读入整数
来源：http://www.m.share.fktsv.cn/Article/details/gldgzhjib.sHtML

int x; scanf("%d", &x);
来源：http://read.share.vehdjk.com/Article/details/giopghntg.sHtML

[S04] C：字符串复制
来源：http://m.share.epnwcf.com/Article/details/gznuxuujt.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.yfazqb.com/Article/details/gxvxksdej.sHtML

[S05] C：字符串长度
来源：http://www.m.share.fktsv.cn/Article/details/grtqgxfek.sHtML

strlen(s)
来源：http://3g.yfazqb.com/Article/details/gbhjxknja.sHtML

[S06] C：字符串比较
来源：http://m.share.fktsv.cn/Article/details/glvjkvmhg.sHtML

strcmp(a, b) == 0
来源：http://m.share.fktsv.cn/Article/details/gubwzpagf.sHtML

[S07] C：数组遍历求和
来源：http://mobile.epnwcf.com/Article/details/gxgxxturx.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.sjlbkw.cn/Article/details/gwghofohz.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.vehdjk.com/Article/details/gegchxehy.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.vehdjk.com/Article/details/gtbabwyak.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.sjlbkw.cn/Article/details/gqwncfwen.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.epnwcf.com/Article/details/gcstnhmmd.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.yfazqb.com/Article/details/gytzctphz.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.epnwcf.com/Article/details/gezuvqzvt.sHtML

[S11] C：逐行读文件
来源：http://read.share.sjlbkw.cn/Article/details/gjatodggg.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.epnwcf.com/Article/details/gptkcqqhh.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.yfazqb.com/Article/details/gwlixauye.sHtML

fclose(f);
来源：http://wap.fktsv.cn/Article/details/gswvgozfk.sHtML

[S12] C：写文件
来源：http://mobile.yfazqb.com/Article/details/gseqtljav.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.epnwcf.com/Article/details/gzdgxgzny.sHtML

[S13] C：宏定义
来源：http://www.share.tarul.cn/Article/details/gzwzytkda.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.yfazqb.com/Article/details/gdapfbdft.sHtML

[S14] C：枚举
来源：http://m.share.epnwcf.com/Article/details/gsqkxhbed.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.sjlbkw.cn/Article/details/gimswfmfw.sHtML

[S15] C：类型转换
来源：http://wap.yfazqb.com/Article/details/gyfmknzve.sHtML

(double) a / b
来源：http://www.blog.sjlbkw.cn/Article/details/goprijyip.sHtML

[S16] C：位操作置位
来源：http://blog.yfazqb.com/Article/details/gdcmzkcbz.sHtML

x |= (1 << 3);
来源：http://www.share.vehdjk.com/Article/details/ghuwqicij.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.sjlbkw.cn/Article/details/giwceziie.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fktsv.cn/Article/details/gprhkrpaa.sHtML

[S18] C：命令行参数
来源：http://www.blog.bbcook.cn/Article/details/gyhrdulyh.sHtML

int main(int argc, char **argv)
来源：http://www.share.vehdjk.com/Article/details/gcrxbqmff.sHtML

[S19] C：快速排序
来源：http://www.m.share.sjlbkw.cn/Article/details/gbavstxhx.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.epnwcf.com/Article/details/gnqklofze.sHtML

[S20] C：二分查找
来源：http://read.share.yfazqb.com/Article/details/govzfjgzc.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.epnwcf.com/Article/details/gdogcytzl.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.sjlbkw.cn/Article/details/ghusdxcox.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.tarul.cn/Article/details/gvhgfiwhl.sHtML

[S22] C：字符串转数字
来源：http://wap.yfazqb.com/Article/details/gkcqghsvx.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.sjlbkw.cn/Article/details/gtcvtrutb.sHtML

[S23] C：随机数
来源：http://blog.vehdjk.com/Article/details/gvrsjetzm.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.epnwcf.com/Article/details/gwvwkzpwr.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.sjlbkw.cn/Article/details/gdjipnylq.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.bbcook.cn/Article/details/gcmveiakp.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.tarul.cn/Article/details/goykvlfbc.sHtML

memcpy(dst, src, n);
来源：http://baike.sjlbkw.cn/Article/details/grcwdadsz.sHtML

[S26] C：内存清零
来源：http://read.share.vehdjk.com/Article/details/geeszfirw.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.tarul.cn/Article/details/gqxqwgswx.sHtML

[S27] C：定义常量
来源：http://mobile.bbcook.cn/Article/details/gtrgrmxgs.sHtML

const double PI = 3.14159;
来源：http://blog.vehdjk.com/Article/details/gbojgvgcj.sHtML

[S28] C：静态变量
来源：http://blog.fktsv.cn/Article/details/glpqhprur.sHtML

static int counter = 0;
来源：http://baike.bbcook.cn/Article/details/gaknlfyuo.sHtML

[S29] C：变参函数
来源：http://blog.sjlbkw.cn/Article/details/gmgrwgoac.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.tarul.cn/Article/details/gwohsbkvv.sHtML

[S30] C：头文件保护
来源：http://blog.vehdjk.com/Article/details/gexrxzygz.sHtML

#ifndef X_H
来源：http://baike.epnwcf.com/Article/details/gbyzusshg.sHtML

#define X_H
来源：http://www.m.share.tarul.cn/Article/details/gwkwoebha.sHtML

#endif
来源：http://mobile.tarul.cn/Article/details/gnplgrzii.sHtML

[S31] C++：Hello World
来源：http://baike.sjlbkw.cn/Article/details/gwdlmnfft.sHtML

#include <iostream>
来源：http://wap.fktsv.cn/Article/details/gawmpgavh.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.bbcook.cn/Article/details/goxpjkwhg.sHtML

[S32] C++：字符串
来源：http://www.share.vehdjk.com/Article/details/gtzrpoblr.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.bbcook.cn/Article/details/gzoravpfj.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fktsv.cn/Article/details/gdaouufdy.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.yfazqb.com/Article/details/gonmclyjy.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fktsv.cn/Article/details/gvnoosqgq.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.epnwcf.com/Article/details/gnbsoikyk.sHtML

[S35] C++：map
来源：http://www.m.share.fktsv.cn/Article/details/genlyjcfl.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fktsv.cn/Article/details/gnrooaker.sHtML

[S36] C++：unordered_map
来源：http://www.share.epnwcf.com/Article/details/gbrewauej.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.vehdjk.com/Article/details/gnmpgukgu.sHtML

[S37] C++：set
来源：http://www.blog.vehdjk.com/Article/details/gpstsxqmx.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.tarul.cn/Article/details/gpywhcgxt.sHtML

[S38] C++：排序
来源：http://read.share.fktsv.cn/Article/details/gzrwvdbhg.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fktsv.cn/Article/details/goxxqqaqj.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.epnwcf.com/Article/details/gxzgacidy.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fktsv.cn/Article/details/gikvtlwzt.sHtML

[S40] C++：查找元素
来源：http://baike.epnwcf.com/Article/details/gixdtovbd.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.bbcook.cn/Article/details/ggwwqctfa.sHtML

[S41] C++：类与构造函数
来源：http://blog.bbcook.cn/Article/details/gnkzymcuc.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.vehdjk.com/Article/details/gpzlbdjzs.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.epnwcf.com/Article/details/gneexurfh.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.bbcook.cn/Article/details/gxygwrooh.sHtML

[S43] C++：智能指针
来源：http://m.share.bbcook.cn/Article/details/gifvnieya.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.fktsv.cn/Article/details/glngalmeh.sHtML

[S44] C++：引用传参
来源：http://wap.vehdjk.com/Article/details/gltacpdnp.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.yfazqb.com/Article/details/gdecitors.sHtML

[S45] C++：lambda
来源：http://www.share.bbcook.cn/Article/details/gzsqnzhmm.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.vehdjk.com/Article/details/gtwhdnutp.sHtML

[S46] C++：函数模板
来源：http://www.blog.vehdjk.com/Article/details/gzwsjsvaw.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.tarul.cn/Article/details/goezojsgx.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.tarul.cn/Article/details/gbqdmkfyb.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.vehdjk.com/Article/details/geiyiiytu.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.yfazqb.com/Article/details/ghwnphskq.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.sjlbkw.cn/Article/details/gpdifcpfb.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.vehdjk.com/Article/details/gbolbiszk.sHtML

[S49] C++：写文件
来源：http://read.share.epnwcf.com/Article/details/ggzxtggom.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.yfazqb.com/Article/details/glddblwaf.sHtML

[S50] C++：格式化数字
来源：http://www.share.sjlbkw.cn/Article/details/gefbwpeby.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.yfazqb.com/Article/details/ghpuqjpnk.sHtML

[S51] C++：显式类型转换
来源：http://3g.tarul.cn/Article/details/giuunocty.sHtML

static_cast<double>(a) / b
来源：http://www.share.vehdjk.com/Article/details/gfhqvxasf.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.vehdjk.com/Article/details/gpwogssal.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.tarul.cn/Article/details/givdrjbgt.sHtML

[S53] C++：移动语义
来源：http://baike.epnwcf.com/Article/details/gwssfmjus.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.yfazqb.com/Article/details/gruyjlssx.sHtML

[S54] C++：异常处理
来源：http://3g.epnwcf.com/Article/details/giatyyfxj.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.bbcook.cn/Article/details/ghcbbzhfu.sHtML

[S55] C++：结构化绑定
来源：http://baike.bbcook.cn/Article/details/gbganukoj.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.tarul.cn/Article/details/gahfvupmd.sHtML

[S56] C++：optional
来源：http://baike.epnwcf.com/Article/details/ghweyadsq.sHtML


<!-- 参考信息 -->