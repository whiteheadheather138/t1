代发 wailian999

[Q82] 字符长度与字节长度
来源：http://baike.fktsv.cn/Article/details/giijagoso.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/gbgxclspb.sHtML

[Q83] 大小写转换
来源：http://www.m.share.tarul.cn/Article/details/gcozkruio.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.vehdjk.com/Article/details/gbfegfuck.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.fktsv.cn/Article/details/gldsvuzkf.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.sjlbkw.cn/Article/details/gascagtsm.sHtML

[Q85] 数值取整
来源：http://www.share.sjlbkw.cn/Article/details/grrsfrkyr.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.bbcook.cn/Article/details/gomnecvwh.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.bbcook.cn/Article/details/gpjgwxsbs.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.epnwcf.com/Article/details/gbxvqldto.sHtML

[Q87] JSON 字段做条件
来源：http://wap.yfazqb.com/Article/details/gvlbkzcue.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.sjlbkw.cn/Article/details/gpuzvwzup.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.tarul.cn/Article/details/ghzcjjwhg.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.fktsv.cn/Article/details/gxmaubawy.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.epnwcf.com/Article/details/gztsozfhl.sHtML

[Q89] 判断表是否存在
来源：http://blog.vehdjk.com/Article/details/gtiodjelm.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.tarul.cn/Article/details/geyakeicn.sHtML

[Q90] 生成序号列
来源：http://mobile.vehdjk.com/Article/details/gzeswarce.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.fktsv.cn/Article/details/gpjtbrqvc.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/ggkgujavk.sHtML

R. Bash 专题
来源：http://baike.epnwcf.com/Article/details/gazaanqjm.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gjqghgdxh.sHtML

[R01] shebang 与严格模式
来源：http://www.share.yfazqb.com/Article/details/gidzvpcnl.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.sjlbkw.cn/Article/details/gpoirbnsx.sHtML

set -euo pipefail
来源：http://wap.vehdjk.com/Article/details/gvkxywtif.sHtML

[R02] 变量赋值与使用
来源：http://www.share.tarul.cn/Article/details/goqktnzmy.sHtML

name="Tom"; echo "$name"
来源：http://m.share.bbcook.cn/Article/details/gnmlqhtus.sHtML

[R03] 只读变量
来源：http://blog.vehdjk.com/Article/details/gwbcbiiok.sHtML

readonly PI=3.14
来源：http://www.blog.epnwcf.com/Article/details/gvorakleu.sHtML

[R04] 位置参数
来源：http://www.m.share.sjlbkw.cn/Article/details/gjqfeatba.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.bbcook.cn/Article/details/gvtxmqevg.sHtML

[R05] 参数默认值
来源：http://3g.sjlbkw.cn/Article/details/gyukbumyh.sHtML

name="${1:-default}"
来源：http://baike.yfazqb.com/Article/details/ggxkjaidy.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.epnwcf.com/Article/details/gsavvsosq.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.tarul.cn/Article/details/gpulcwuxx.sHtML

[R07] if 判断文件
来源：http://mobile.epnwcf.com/Article/details/glloeuxya.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.tarul.cn/Article/details/gawumcelw.sHtML

[R08] 数值比较
来源：http://baike.fktsv.cn/Article/details/ggbuoyjus.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.yfazqb.com/Article/details/gqwgvurln.sHtML

[R09] 字符串比较
来源：http://www.share.yfazqb.com/Article/details/gsmnoziug.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.tarul.cn/Article/details/gdxatzjxw.sHtML

[R10] 正则匹配
来源：http://www.blog.epnwcf.com/Article/details/goegcgjab.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.sjlbkw.cn/Article/details/godwweons.sHtML

[R11] case 多分支
来源：http://www.m.share.vehdjk.com/Article/details/gedblvtpm.sHtML

case "$1" in
来源：http://mobile.fktsv.cn/Article/details/gisksafon.sHtML

start) echo "启动" ;;
来源：http://www.share.sjlbkw.cn/Article/details/gzbmkfshr.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.epnwcf.com/Article/details/goiythafw.sHtML

*)     echo "未知命令" ;;
来源：http://3g.epnwcf.com/Article/details/gsjowjtaj.sHtML

esac
来源：http://wap.epnwcf.com/Article/details/gufydadvv.sHtML

[R12] for 遍历文件
来源：http://mobile.epnwcf.com/Article/details/gqhjwkahk.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.yfazqb.com/Article/details/gbmorbubt.sHtML

[R13] for 计数循环
来源：http://www.m.share.bbcook.cn/Article/details/guqqqpwki.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.vehdjk.com/Article/details/gcgyfjmek.sHtML

[R14] C 风格 for
来源：http://blog.vehdjk.com/Article/details/ghslifcge.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.yfazqb.com/Article/details/gkqlmldih.sHtML

[R15] while 逐行读文件
来源：http://www.blog.tarul.cn/Article/details/gtbaesxtt.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.yfazqb.com/Article/details/gjpqtkwyx.sHtML

[R16] until 等待条件
来源：http://www.m.share.fktsv.cn/Article/details/gocqrsgiy.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.yfazqb.com/Article/details/gektvgsfr.sHtML

[R17] 数组定义与取值
来源：http://www.share.fktsv.cn/Article/details/gaggtsgye.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.vehdjk.com/Article/details/ghyandzdy.sHtML

[R18] 遍历数组
来源：http://m.share.epnwcf.com/Article/details/gurgzpmih.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.yfazqb.com/Article/details/gmxpgwebz.sHtML

[R19] 数组长度
来源：http://www.blog.tarul.cn/Article/details/gsgyqgktz.sHtML

echo "${#arr[@]}"
来源：http://baike.yfazqb.com/Article/details/gbdmbzepy.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.tarul.cn/Article/details/gpwydrpao.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.tarul.cn/Article/details/gbufkcwvy.sHtML

[R21] 字符串长度
来源：http://baike.tarul.cn/Article/details/gxbrhkivn.sHtML

echo "${#s}"
来源：http://www.blog.sjlbkw.cn/Article/details/gjymudgef.sHtML

[R22] 截取子串
来源：http://www.share.vehdjk.com/Article/details/gbmmkjpkz.sHtML

echo "${s:0:5}"
来源：http://blog.yfazqb.com/Article/details/gmdbsfxhk.sHtML

[R23] 字符串替换
来源：http://www.share.fktsv.cn/Article/details/gmcbhmywx.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.epnwcf.com/Article/details/gzwxkwzmi.sHtML

[R24] 大小写转换
来源：http://read.share.bbcook.cn/Article/details/gjddzlsxz.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.fktsv.cn/Article/details/gfbomhmej.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.epnwcf.com/Article/details/ggejswfbu.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.yfazqb.com/Article/details/ghhnuahxg.sHtML

[R26] 命令替换
来源：http://3g.tarul.cn/Article/details/gacncnpdf.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.epnwcf.com/Article/details/gjtyjkyat.sHtML

[R27] 算术展开
来源：http://m.share.fktsv.cn/Article/details/ggotqgibh.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.sjlbkw.cn/Article/details/gubijnrem.sHtML

[R28] 浮点运算
来源：http://www.m.share.bbcook.cn/Article/details/gzgqkwhio.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.sjlbkw.cn/Article/details/gymytzjku.sHtML

[R29] 定义函数
来源：http://www.m.share.vehdjk.com/Article/details/grecpkoba.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.vehdjk.com/Article/details/gmgebyxkn.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.vehdjk.com/Article/details/gnezznlvs.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.tarul.cn/Article/details/gfnlnbxet.sHtML

[R31] 局部变量
来源：http://www.m.share.sjlbkw.cn/Article/details/gvsfbvicv.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.epnwcf.com/Article/details/gftdcyeqs.sHtML

[R32] 参数个数校验
来源：http://baike.sjlbkw.cn/Article/details/gtxjkznnc.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.bbcook.cn/Article/details/gonsyjmgw.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.yfazqb.com/Article/details/gkujekwlb.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.bbcook.cn/Article/details/gesmaawld.sHtML

[R34] 退出时清理
来源：http://www.blog.vehdjk.com/Article/details/gxfdallcv.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.vehdjk.com/Article/details/gcohwxjij.sHtML

[R35] 后台执行并等待
来源：http://read.share.bbcook.cn/Article/details/gurieinrm.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fktsv.cn/Article/details/gukxbasqo.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fktsv.cn/Article/details/gvzgmjixi.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.yfazqb.com/Article/details/gsusyofbz.sHtML

[R37] 把输出赋给变量
来源：http://m.share.bbcook.cn/Article/details/goymbnfoc.sHtML

files=$(ls -1)
来源：http://read.share.fktsv.cn/Article/details/gopzgtxoo.sHtML

[R38] 管道串联
来源：http://baike.bbcook.cn/Article/details/gxgohqsds.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.bbcook.cn/Article/details/gikfzbxmj.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.fktsv.cn/Article/details/gmozjqoxb.sHtML

cmd > out.log 2>&1
来源：http://wap.tarul.cn/Article/details/goejhamdi.sHtML

[R40] 追加写日志
来源：http://blog.fktsv.cn/Article/details/ggdauwedk.sHtML

echo "log" >> out.log
来源：http://blog.bbcook.cn/Article/details/gncqhogqf.sHtML

[R41] 丢弃输出
来源：http://www.share.sjlbkw.cn/Article/details/gdjvsyzux.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.tarul.cn/Article/details/gmqcmbvfe.sHtML

[R42] 输入重定向
来源：http://www.share.vehdjk.com/Article/details/gwwsltjfu.sHtML

wc -l < a.txt
来源：http://3g.bbcook.cn/Article/details/guqjddteq.sHtML

[R43] 按名字查找文件
来源：http://www.share.vehdjk.com/Article/details/gfnmbrlgf.sHtML

find . -name "*.log" -type f
来源：http://blog.yfazqb.com/Article/details/gikkhhxre.sHtML

[R44] 按修改时间查找
来源：http://wap.bbcook.cn/Article/details/gubgovijg.sHtML

find . -mtime -7 -type f
来源：http://3g.epnwcf.com/Article/details/gzcgilojp.sHtML

[R45] 批量删除
来源：http://www.m.share.vehdjk.com/Article/details/gesrjnoeb.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fktsv.cn/Article/details/gfuogcnha.sHtML

[R46] 递归替换文件内容
来源：http://www.share.vehdjk.com/Article/details/gfaxhlgij.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.vehdjk.com/Article/details/gbkezgnex.sHtML

[R47] sed 单行替换
来源：http://baike.bbcook.cn/Article/details/golijrxzo.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fktsv.cn/Article/details/gzqmjxgny.sHtML

[R48] awk 取指定列
来源：http://3g.tarul.cn/Article/details/gzjxfjshy.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.bbcook.cn/Article/details/gsnuusblu.sHtML

[R49] awk 带条件
来源：http://baike.sjlbkw.cn/Article/details/gpyfypavj.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.epnwcf.com/Article/details/guketknul.sHtML

[R50] awk 求和
来源：http://mobile.tarul.cn/Article/details/gcupbjgjc.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fktsv.cn/Article/details/goyunemka.sHtML

[R51] 排序去重取前几
来源：http://read.share.bbcook.cn/Article/details/gvixlkrzm.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.sjlbkw.cn/Article/details/gbawvjwio.sHtML

[R52] 统计行数
来源：http://read.share.fktsv.cn/Article/details/gawsiyatw.sHtML

wc -l a.txt
来源：http://www.blog.yfazqb.com/Article/details/gytcajhvm.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.epnwcf.com/Article/details/gjryacayi.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.sjlbkw.cn/Article/details/gjkswroos.sHtML

[R54] 比较两个文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gdenkxfug.sHtML

diff a.txt b.txt
来源：http://wap.yfazqb.com/Article/details/gejqhaygu.sHtML

[R55] 压缩与解压
来源：http://www.m.share.tarul.cn/Article/details/gayvkqhxv.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.yfazqb.com/Article/details/grnpyuozu.sHtML

[R56] 远程拷贝
来源：http://mobile.vehdjk.com/Article/details/gmiblsdha.sHtML

scp file user@host:/path/
来源：http://wap.vehdjk.com/Article/details/gkbqdehtp.sHtML

[R57] 远程执行命令
来源：http://mobile.bbcook.cn/Article/details/gckntproo.sHtML

ssh user@host 'uptime'
来源：http://www.share.bbcook.cn/Article/details/gbxvwzvln.sHtML

[R58] 下载文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gftcdcscq.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.tarul.cn/Article/details/gmrhvkxvq.sHtML

[R59] 发 POST JSON
来源：http://read.share.epnwcf.com/Article/details/grwpjmgda.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.sjlbkw.cn/Article/details/gacijrfkk.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fktsv.cn/Article/details/girariqab.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.sjlbkw.cn/Article/details/gwmppzptl.sHtML

[R61] 磁盘占用
来源：http://www.m.share.yfazqb.com/Article/details/gpiaizpec.sHtML

df -h;  du -sh *
来源：http://www.m.share.tarul.cn/Article/details/gwovjpzbh.sHtML

[R62] 找最占空间的文件
来源：http://read.share.sjlbkw.cn/Article/details/gispaabdu.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fktsv.cn/Article/details/gjsjvlmmm.sHtML

[R63] 内存与进程
来源：http://www.blog.sjlbkw.cn/Article/details/gnbcwavfk.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.bbcook.cn/Article/details/gufvxuicp.sHtML

[R64] 结束进程
来源：http://blog.fktsv.cn/Article/details/gjztcrxsv.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.vehdjk.com/Article/details/gpzumecuy.sHtML

[R65] 查看端口占用
来源：http://www.share.sjlbkw.cn/Article/details/gqmlkmvcq.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.sjlbkw.cn/Article/details/gfzghedmy.sHtML

[R66] 定时任务
来源：http://www.share.bbcook.cn/Article/details/gejsuvphp.sHtML

crontab -e;  crontab -l
来源：http://wap.sjlbkw.cn/Article/details/gpxqzpwzb.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fktsv.cn/Article/details/grfanlyby.sHtML

openssl rand -hex 16
来源：http://m.share.sjlbkw.cn/Article/details/gcixdgbji.sHtML

[R68] 计算文件校验值
来源：http://wap.tarul.cn/Article/details/glgbbdrrp.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fktsv.cn/Article/details/gjmckxezc.sHtML

[R69] 生成随机密码
来源：http://www.blog.tarul.cn/Article/details/gtennrixo.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.tarul.cn/Article/details/gotcmvtmc.sHtML

[R70] 时间戳与互转
来源：http://wap.epnwcf.com/Article/details/gqiejpqlk.sHtML

date +%s;  date -d @1700000000
来源：http://blog.bbcook.cn/Article/details/gkebrrywd.sHtML

[R71] 日期格式化
来源：http://www.share.tarul.cn/Article/details/gxviatwwj.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.sjlbkw.cn/Article/details/gjkzwyfim.sHtML

[R72] 等待端口就绪
来源：http://www.blog.bbcook.cn/Article/details/gklwtztux.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.tarul.cn/Article/details/gweqynttw.sHtML

[R73] 分割大日志
来源：http://wap.vehdjk.com/Article/details/grwwiudap.sHtML

split -l 1000 big.log part_
来源：http://m.share.tarul.cn/Article/details/grcujvwnh.sHtML

[R74] 批量重命名
来源：http://m.share.sjlbkw.cn/Article/details/glxbckafm.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.tarul.cn/Article/details/gulawpbvn.sHtML

[R75] 导出环境变量
来源：http://baike.bbcook.cn/Article/details/ghmicnqbc.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.sjlbkw.cn/Article/details/gyksfpejq.sHtML

[R76] 使用临时文件
来源：http://3g.tarul.cn/Article/details/gxeieowpy.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.sjlbkw.cn/Article/details/gjmvnhfuv.sHtML

[R77] 读取用户输入
来源：http://baike.vehdjk.com/Article/details/gyfxzjunj.sHtML

read -rp "请输入: " ans
来源：http://wap.vehdjk.com/Article/details/gxamammin.sHtML

[R78] 交互式菜单
来源：http://baike.tarul.cn/Article/details/glbeltafq.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.epnwcf.com/Article/details/ganzzkpmk.sHtML

[R79] 解析命令行选项
来源：http://www.share.sjlbkw.cn/Article/details/ghuyjwdpn.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.fktsv.cn/Article/details/gqkuovynj.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.sjlbkw.cn/Article/details/gmzomqsuz.sHtML

time ./run.sh
来源：http://m.share.tarul.cn/Article/details/gatvskeej.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/ghazsjwbv.sHtML

S. C / C++ 专题
来源：http://www.blog.sjlbkw.cn/Article/details/gcwfoadih.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/guojdxpcf.sHtML

[S01] C：Hello World
来源：http://3g.yfazqb.com/Article/details/giicqczgf.sHtML

#include <stdio.h>
来源：http://www.m.share.yfazqb.com/Article/details/giphiswfu.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fktsv.cn/Article/details/gpklsojck.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.epnwcf.com/Article/details/gbqmhxqyo.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.epnwcf.com/Article/details/gqbogtbml.sHtML

[S03] C：读入整数
来源：http://www.share.sjlbkw.cn/Article/details/gjjcijope.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.bbcook.cn/Article/details/guzknehnw.sHtML

[S04] C：字符串复制
来源：http://www.share.tarul.cn/Article/details/gyqakfqyh.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.bbcook.cn/Article/details/gwsirekjd.sHtML

[S05] C：字符串长度
来源：http://read.share.epnwcf.com/Article/details/gjldypenp.sHtML

strlen(s)
来源：http://www.share.epnwcf.com/Article/details/gbuskadps.sHtML

[S06] C：字符串比较
来源：http://www.blog.sjlbkw.cn/Article/details/gvaeclopz.sHtML

strcmp(a, b) == 0
来源：http://mobile.yfazqb.com/Article/details/gzsjzuwfv.sHtML

[S07] C：数组遍历求和
来源：http://m.share.sjlbkw.cn/Article/details/gvoyvcgtn.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.epnwcf.com/Article/details/glxqcwrex.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.epnwcf.com/Article/details/gfgcfvmnf.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.bbcook.cn/Article/details/gureirqbu.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.yfazqb.com/Article/details/goxpozvcp.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fktsv.cn/Article/details/gtzqxrmcp.sHtML

[S10] C：指针与解引用
来源：http://3g.vehdjk.com/Article/details/gpsfubbbb.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.bbcook.cn/Article/details/gmubfdjaz.sHtML

[S11] C：逐行读文件
来源：http://read.share.vehdjk.com/Article/details/gegvpjpvv.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.sjlbkw.cn/Article/details/gedxavdkv.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.yfazqb.com/Article/details/gdixbnuat.sHtML

fclose(f);
来源：http://3g.epnwcf.com/Article/details/gvxwwuuzj.sHtML

[S12] C：写文件
来源：http://mobile.tarul.cn/Article/details/glckkpiie.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.vehdjk.com/Article/details/ghxfrpndm.sHtML

[S13] C：宏定义
来源：http://read.share.yfazqb.com/Article/details/gpxzjpufh.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.vehdjk.com/Article/details/gbqucpzzw.sHtML

[S14] C：枚举
来源：http://www.share.sjlbkw.cn/Article/details/gdxwgqsqb.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.yfazqb.com/Article/details/gmvebqodv.sHtML

[S15] C：类型转换
来源：http://baike.epnwcf.com/Article/details/gmfajbdgh.sHtML

(double) a / b
来源：http://3g.sjlbkw.cn/Article/details/gxoasfazv.sHtML

[S16] C：位操作置位
来源：http://3g.epnwcf.com/Article/details/gthbrdjyo.sHtML

x |= (1 << 3);
来源：http://m.share.tarul.cn/Article/details/gshrijolw.sHtML

[S17] C：安全拼接字符串
来源：http://wap.epnwcf.com/Article/details/giskqetoc.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.tarul.cn/Article/details/gquoqndov.sHtML

[S18] C：命令行参数
来源：http://m.share.bbcook.cn/Article/details/gsvymxqez.sHtML

int main(int argc, char **argv)
来源：http://mobile.tarul.cn/Article/details/guojyegqy.sHtML

[S19] C：快速排序
来源：http://blog.bbcook.cn/Article/details/gubmfwjvz.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.bbcook.cn/Article/details/ginotgoqr.sHtML

[S20] C：二分查找
来源：http://m.share.epnwcf.com/Article/details/ggfwpiodu.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.epnwcf.com/Article/details/gtjmvgfny.sHtML

[S21] C：字符类别判断
来源：http://baike.sjlbkw.cn/Article/details/gvpsjzpij.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.sjlbkw.cn/Article/details/gqkrantix.sHtML

[S22] C：字符串转数字
来源：http://3g.tarul.cn/Article/details/gvsugodgj.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.bbcook.cn/Article/details/gfvjwppex.sHtML

[S23] C：随机数
来源：http://baike.epnwcf.com/Article/details/gjythuqca.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.tarul.cn/Article/details/gejceifrj.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.bbcook.cn/Article/details/gbzyvuxhz.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.yfazqb.com/Article/details/gitlatuto.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.tarul.cn/Article/details/grqkgnrek.sHtML

memcpy(dst, src, n);
来源：http://www.share.vehdjk.com/Article/details/gunorfolm.sHtML

[S26] C：内存清零
来源：http://www.blog.tarul.cn/Article/details/gvotttash.sHtML

memset(a, 0, sizeof a);
来源：http://wap.bbcook.cn/Article/details/gbqudqjlb.sHtML

[S27] C：定义常量
来源：http://3g.epnwcf.com/Article/details/gfbvoitno.sHtML

const double PI = 3.14159;
来源：http://www.blog.fktsv.cn/Article/details/gujzithlo.sHtML

[S28] C：静态变量
来源：http://www.blog.sjlbkw.cn/Article/details/gycbttyxo.sHtML

static int counter = 0;
来源：http://m.share.vehdjk.com/Article/details/gnnagxoxo.sHtML

[S29] C：变参函数
来源：http://mobile.yfazqb.com/Article/details/gwoalbuld.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.sjlbkw.cn/Article/details/giuvbsroz.sHtML

[S30] C：头文件保护
来源：http://3g.fktsv.cn/Article/details/gomrxnhuj.sHtML

#ifndef X_H
来源：http://wap.bbcook.cn/Article/details/gygdewspq.sHtML

#define X_H
来源：http://blog.epnwcf.com/Article/details/gymizyzqm.sHtML

#endif
来源：http://read.share.yfazqb.com/Article/details/gxdomfiep.sHtML

[S31] C++：Hello World
来源：http://www.blog.vehdjk.com/Article/details/gejpnlxpw.sHtML

#include <iostream>
来源：http://www.share.bbcook.cn/Article/details/ggququnzz.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fktsv.cn/Article/details/gyafbcwjc.sHtML

[S32] C++：字符串
来源：http://blog.bbcook.cn/Article/details/gdkpmxost.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.sjlbkw.cn/Article/details/gopvdzjnl.sHtML

[S33] C++：vector 增删
来源：http://mobile.sjlbkw.cn/Article/details/gkumdjzmb.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.epnwcf.com/Article/details/ghwyqpygm.sHtML

[S34] C++：遍历 vector
来源：http://3g.sjlbkw.cn/Article/details/gxkjvtqia.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.epnwcf.com/Article/details/ghrekxeeg.sHtML

[S35] C++：map
来源：http://m.share.sjlbkw.cn/Article/details/gkviamfgt.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.sjlbkw.cn/Article/details/gfqmdxuwo.sHtML

[S36] C++：unordered_map
来源：http://baike.yfazqb.com/Article/details/gdgbyfjcw.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.yfazqb.com/Article/details/gpruqtujr.sHtML

[S37] C++：set
来源：http://read.share.sjlbkw.cn/Article/details/gcdrybmod.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.bbcook.cn/Article/details/gitcoosuz.sHtML

[S38] C++：排序
来源：http://wap.vehdjk.com/Article/details/gkjcgnwst.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.epnwcf.com/Article/details/gnayjydgn.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.fktsv.cn/Article/details/gnuqljnss.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.bbcook.cn/Article/details/gzrckwodl.sHtML

[S40] C++：查找元素
来源：http://baike.fktsv.cn/Article/details/ghndiqcpz.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.fktsv.cn/Article/details/gguhcovpl.sHtML

[S41] C++：类与构造函数
来源：http://3g.fktsv.cn/Article/details/gbaalsxgy.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.vehdjk.com/Article/details/gduovffsw.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.sjlbkw.cn/Article/details/gxirtdskc.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.tarul.cn/Article/details/gnzwghofr.sHtML

[S43] C++：智能指针
来源：http://3g.sjlbkw.cn/Article/details/giugxrhec.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.fktsv.cn/Article/details/gmgircrpb.sHtML

[S44] C++：引用传参
来源：http://www.blog.epnwcf.com/Article/details/gjesyodne.sHtML

void inc(int &x) { ++x; }
来源：http://wap.epnwcf.com/Article/details/gqvxgdbmf.sHtML

[S45] C++：lambda
来源：http://www.share.vehdjk.com/Article/details/grdqqwzzb.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.yfazqb.com/Article/details/ggrsvaayr.sHtML

[S46] C++：函数模板
来源：http://www.blog.epnwcf.com/Article/details/gmvbsecoi.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.vehdjk.com/Article/details/gzpitstoj.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.tarul.cn/Article/details/gjsqapepp.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.epnwcf.com/Article/details/gssuytjii.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.tarul.cn/Article/details/gefteoior.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.vehdjk.com/Article/details/ghybxmpln.sHtML

while (std::getline(in, line)) { }
来源：http://baike.yfazqb.com/Article/details/gweufxbfb.sHtML

[S49] C++：写文件
来源：http://mobile.fktsv.cn/Article/details/gsnrgudlv.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.sjlbkw.cn/Article/details/glptlwybp.sHtML

[S50] C++：格式化数字
来源：http://3g.epnwcf.com/Article/details/gtutsmily.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.sjlbkw.cn/Article/details/gjucvepzx.sHtML

[S51] C++：显式类型转换
来源：http://www.share.bbcook.cn/Article/details/gxscubkmq.sHtML

static_cast<double>(a) / b
来源：http://3g.yfazqb.com/Article/details/gdkcblmoe.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.yfazqb.com/Article/details/ghziktyvl.sHtML


<!-- 参考信息 -->