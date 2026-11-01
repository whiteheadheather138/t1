代发 wailian999

[Q80] 字符串截取
来源：http://www.share.yfazqb.com/Article/details/gcbncldhb.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.epnwcf.com/Article/details/gqjxtvdcs.sHtML

[Q81] 字符串替换
来源：http://www.blog.bbcook.cn/Article/details/gzoyuowle.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.tarul.cn/Article/details/guwugxist.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.tarul.cn/Article/details/glcuzzhfv.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.tarul.cn/Article/details/gmaoqmuzp.sHtML

[Q83] 大小写转换
来源：http://www.share.fktsv.cn/Article/details/gqeaypicv.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.epnwcf.com/Article/details/glevjyjcl.sHtML

[Q84] 去除首尾空格
来源：http://m.share.fktsv.cn/Article/details/govytutcp.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.vehdjk.com/Article/details/gjexeqxwc.sHtML

[Q85] 数值取整
来源：http://m.share.fktsv.cn/Article/details/gjkmhxhyx.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.tarul.cn/Article/details/ghprogaqc.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.yfazqb.com/Article/details/gglckcgut.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.bbcook.cn/Article/details/gdgvtgjib.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.tarul.cn/Article/details/gncqrzirf.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.sjlbkw.cn/Article/details/gycqmkbkv.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.sjlbkw.cn/Article/details/gfbdiubfp.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.fktsv.cn/Article/details/grlthjbwo.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.epnwcf.com/Article/details/geoivsxcd.sHtML

[Q89] 判断表是否存在
来源：http://m.share.epnwcf.com/Article/details/guwgdzoab.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.tarul.cn/Article/details/garjewbxb.sHtML

[Q90] 生成序号列
来源：http://m.share.bbcook.cn/Article/details/gunkhospz.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.vehdjk.com/Article/details/ghxdrtzym.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gcyrpzozp.sHtML

R. Bash 专题
来源：http://baike.sjlbkw.cn/Article/details/gjxzdyqvw.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gqkrfzamf.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.yfazqb.com/Article/details/guappsqzv.sHtML

#!/usr/bin/env bash
来源：http://m.share.vehdjk.com/Article/details/grrbrqhnh.sHtML

set -euo pipefail
来源：http://blog.yfazqb.com/Article/details/grhegoqhm.sHtML

[R02] 变量赋值与使用
来源：http://blog.tarul.cn/Article/details/gocixgiwa.sHtML

name="Tom"; echo "$name"
来源：http://www.share.tarul.cn/Article/details/gwaziurcv.sHtML

[R03] 只读变量
来源：http://www.share.sjlbkw.cn/Article/details/gksdocjlp.sHtML

readonly PI=3.14
来源：http://baike.sjlbkw.cn/Article/details/gewqnagnb.sHtML

[R04] 位置参数
来源：http://www.m.share.epnwcf.com/Article/details/gvdecijef.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.yfazqb.com/Article/details/gkinzdsts.sHtML

[R05] 参数默认值
来源：http://3g.fktsv.cn/Article/details/gkybjczuv.sHtML

name="${1:-default}"
来源：http://blog.fktsv.cn/Article/details/gjijnxzyx.sHtML

[R06] 判断命令是否存在
来源：http://3g.epnwcf.com/Article/details/gxvaixnhv.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.sjlbkw.cn/Article/details/gaygoqese.sHtML

[R07] if 判断文件
来源：http://3g.yfazqb.com/Article/details/gnjbbdrcd.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.sjlbkw.cn/Article/details/gwczfvvuq.sHtML

[R08] 数值比较
来源：http://3g.fktsv.cn/Article/details/gszrxcmyv.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.bbcook.cn/Article/details/gngjcrnmf.sHtML

[R09] 字符串比较
来源：http://baike.sjlbkw.cn/Article/details/godjtdvpu.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.epnwcf.com/Article/details/gagnjctzk.sHtML

[R10] 正则匹配
来源：http://www.m.share.tarul.cn/Article/details/ghpsysclg.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.fktsv.cn/Article/details/gaxydyomb.sHtML

[R11] case 多分支
来源：http://www.share.fktsv.cn/Article/details/gqstmoyel.sHtML

case "$1" in
来源：http://blog.yfazqb.com/Article/details/grkqhlzon.sHtML

start) echo "启动" ;;
来源：http://3g.fktsv.cn/Article/details/gyukyycjh.sHtML

stop)  echo "停止" ;;
来源：http://baike.epnwcf.com/Article/details/grkfsqctz.sHtML

*)     echo "未知命令" ;;
来源：http://3g.tarul.cn/Article/details/gkmlguibf.sHtML

esac
来源：http://www.share.bbcook.cn/Article/details/ghvkigaxd.sHtML

[R12] for 遍历文件
来源：http://blog.yfazqb.com/Article/details/guolbopye.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.vehdjk.com/Article/details/gaprfsoog.sHtML

[R13] for 计数循环
来源：http://read.share.yfazqb.com/Article/details/gqdssagjp.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.epnwcf.com/Article/details/gutdarivb.sHtML

[R14] C 风格 for
来源：http://blog.vehdjk.com/Article/details/ghrqntzee.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.bbcook.cn/Article/details/gufccnlqq.sHtML

[R15] while 逐行读文件
来源：http://3g.sjlbkw.cn/Article/details/gfzcrzczh.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.tarul.cn/Article/details/gnvrachrz.sHtML

[R16] until 等待条件
来源：http://3g.yfazqb.com/Article/details/ghznyyulh.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.tarul.cn/Article/details/glmcxgsst.sHtML

[R17] 数组定义与取值
来源：http://www.share.yfazqb.com/Article/details/gjxzbvhai.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.sjlbkw.cn/Article/details/gjsalpsnk.sHtML

[R18] 遍历数组
来源：http://wap.yfazqb.com/Article/details/gcodphayo.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.vehdjk.com/Article/details/gdisncjvp.sHtML

[R19] 数组长度
来源：http://wap.yfazqb.com/Article/details/gejiwenkp.sHtML

echo "${#arr[@]}"
来源：http://baike.yfazqb.com/Article/details/gslhiomgs.sHtML

[R20] 关联数组（字典）
来源：http://mobile.sjlbkw.cn/Article/details/ggobdzeym.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.vehdjk.com/Article/details/gocqnafzn.sHtML

[R21] 字符串长度
来源：http://read.share.yfazqb.com/Article/details/gjefehowa.sHtML

echo "${#s}"
来源：http://m.share.tarul.cn/Article/details/genykrbjm.sHtML

[R22] 截取子串
来源：http://wap.tarul.cn/Article/details/guhgxknpf.sHtML

echo "${s:0:5}"
来源：http://mobile.fktsv.cn/Article/details/glpsqyqyb.sHtML

[R23] 字符串替换
来源：http://blog.vehdjk.com/Article/details/gxgqrkpyb.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.tarul.cn/Article/details/gxbhnvxht.sHtML

[R24] 大小写转换
来源：http://blog.fktsv.cn/Article/details/gybcktpzs.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.vehdjk.com/Article/details/gclvojref.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.tarul.cn/Article/details/gscgabfqg.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.tarul.cn/Article/details/glxfwpjyr.sHtML

[R26] 命令替换
来源：http://blog.sjlbkw.cn/Article/details/gkajrhntq.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.epnwcf.com/Article/details/ggccbednq.sHtML

[R27] 算术展开
来源：http://mobile.tarul.cn/Article/details/gfrplvrfh.sHtML

echo $((1 + 2 * 3))
来源：http://3g.bbcook.cn/Article/details/gvxjstwuo.sHtML

[R28] 浮点运算
来源：http://read.share.sjlbkw.cn/Article/details/gktstzvpl.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.tarul.cn/Article/details/gyzepnqhz.sHtML

[R29] 定义函数
来源：http://www.share.fktsv.cn/Article/details/gybnydkqv.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.yfazqb.com/Article/details/gsdhsztkb.sHtML

[R30] 函数返回状态码
来源：http://baike.bbcook.cn/Article/details/gumgtxjdi.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fktsv.cn/Article/details/guudnoyps.sHtML

[R31] 局部变量
来源：http://mobile.vehdjk.com/Article/details/grjronynq.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.sjlbkw.cn/Article/details/gsothzcuc.sHtML

[R32] 参数个数校验
来源：http://www.m.share.sjlbkw.cn/Article/details/gedfnbswx.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.vehdjk.com/Article/details/gzrxcauim.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.epnwcf.com/Article/details/gmlynkhxl.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.vehdjk.com/Article/details/gebzbgley.sHtML

[R34] 退出时清理
来源：http://mobile.fktsv.cn/Article/details/gmbjcggan.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fktsv.cn/Article/details/gmqjicklm.sHtML

[R35] 后台执行并等待
来源：http://read.share.tarul.cn/Article/details/gjespwkml.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.tarul.cn/Article/details/gwhtjsxhw.sHtML

[R36] 并发执行多个任务
来源：http://wap.fktsv.cn/Article/details/gaksxsmkq.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.tarul.cn/Article/details/gupgkjlrn.sHtML

[R37] 把输出赋给变量
来源：http://m.share.sjlbkw.cn/Article/details/gkxadypow.sHtML

files=$(ls -1)
来源：http://www.share.fktsv.cn/Article/details/gstfgzkxu.sHtML

[R38] 管道串联
来源：http://mobile.epnwcf.com/Article/details/galzngvaa.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fktsv.cn/Article/details/gzlsmcrnq.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.sjlbkw.cn/Article/details/grrfdubrq.sHtML

cmd > out.log 2>&1
来源：http://baike.tarul.cn/Article/details/gyapmoqgq.sHtML

[R40] 追加写日志
来源：http://www.blog.bbcook.cn/Article/details/ghjhgwvvi.sHtML

echo "log" >> out.log
来源：http://3g.vehdjk.com/Article/details/glkesohye.sHtML

[R41] 丢弃输出
来源：http://www.share.sjlbkw.cn/Article/details/gweagssxs.sHtML

cmd >/dev/null 2>&1
来源：http://baike.epnwcf.com/Article/details/geryfgvlm.sHtML

[R42] 输入重定向
来源：http://wap.yfazqb.com/Article/details/gvrvchomi.sHtML

wc -l < a.txt
来源：http://www.m.share.bbcook.cn/Article/details/gwmnadueo.sHtML

[R43] 按名字查找文件
来源：http://blog.yfazqb.com/Article/details/gwefpcadz.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.vehdjk.com/Article/details/guxrrkaks.sHtML

[R44] 按修改时间查找
来源：http://m.share.epnwcf.com/Article/details/gszfwszlp.sHtML

find . -mtime -7 -type f
来源：http://wap.sjlbkw.cn/Article/details/gppfrnjui.sHtML

[R45] 批量删除
来源：http://3g.fktsv.cn/Article/details/guilpkgzf.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.yfazqb.com/Article/details/gwdvremou.sHtML

[R46] 递归替换文件内容
来源：http://m.share.vehdjk.com/Article/details/gcccnmwfe.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.bbcook.cn/Article/details/ggputqmlh.sHtML

[R47] sed 单行替换
来源：http://read.share.bbcook.cn/Article/details/gnutbntcu.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fktsv.cn/Article/details/gvisxtdqv.sHtML

[R48] awk 取指定列
来源：http://www.m.share.yfazqb.com/Article/details/gbprvcvcp.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.bbcook.cn/Article/details/gvzsjaqnd.sHtML

[R49] awk 带条件
来源：http://wap.vehdjk.com/Article/details/geqxpfcss.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.epnwcf.com/Article/details/gaoqdxbmw.sHtML

[R50] awk 求和
来源：http://www.m.share.bbcook.cn/Article/details/glitergim.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.epnwcf.com/Article/details/gitcjuebe.sHtML

[R51] 排序去重取前几
来源：http://mobile.vehdjk.com/Article/details/gtfhoegzh.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.vehdjk.com/Article/details/gcqrbdkmc.sHtML

[R52] 统计行数
来源：http://m.share.epnwcf.com/Article/details/gqxwvysnq.sHtML

wc -l a.txt
来源：http://www.m.share.yfazqb.com/Article/details/gpxoxjlcv.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.sjlbkw.cn/Article/details/gstaqnzrm.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.bbcook.cn/Article/details/gxqlplwdj.sHtML

[R54] 比较两个文件
来源：http://blog.bbcook.cn/Article/details/gkyugqhcs.sHtML

diff a.txt b.txt
来源：http://mobile.epnwcf.com/Article/details/gysfnszjr.sHtML

[R55] 压缩与解压
来源：http://3g.fktsv.cn/Article/details/gxpmyyzcm.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.vehdjk.com/Article/details/gsqovymdf.sHtML

[R56] 远程拷贝
来源：http://www.share.epnwcf.com/Article/details/gjvdysvjg.sHtML

scp file user@host:/path/
来源：http://www.blog.epnwcf.com/Article/details/gzhgenaid.sHtML

[R57] 远程执行命令
来源：http://baike.sjlbkw.cn/Article/details/glwbtncdd.sHtML

ssh user@host 'uptime'
来源：http://m.share.tarul.cn/Article/details/gkjbagyqw.sHtML

[R58] 下载文件
来源：http://baike.fktsv.cn/Article/details/gghajxcsq.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.tarul.cn/Article/details/glvlzekle.sHtML

[R59] 发 POST JSON
来源：http://mobile.yfazqb.com/Article/details/glamzncbe.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.sjlbkw.cn/Article/details/gdxgotjhm.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fktsv.cn/Article/details/gmomwsmsl.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.vehdjk.com/Article/details/gkgelfdcb.sHtML

[R61] 磁盘占用
来源：http://www.blog.bbcook.cn/Article/details/gyqcuwwfd.sHtML

df -h;  du -sh *
来源：http://blog.fktsv.cn/Article/details/gxsowyonv.sHtML

[R62] 找最占空间的文件
来源：http://wap.yfazqb.com/Article/details/ggsxorkti.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.epnwcf.com/Article/details/gzfiscdec.sHtML

[R63] 内存与进程
来源：http://www.share.tarul.cn/Article/details/gplsyulkw.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.fktsv.cn/Article/details/gdadunaog.sHtML

[R64] 结束进程
来源：http://baike.vehdjk.com/Article/details/gwypbznhv.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.fktsv.cn/Article/details/gbjbpsroq.sHtML

[R65] 查看端口占用
来源：http://www.share.vehdjk.com/Article/details/gyckqmmje.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.yfazqb.com/Article/details/gtslmidmz.sHtML

[R66] 定时任务
来源：http://m.share.fktsv.cn/Article/details/gaicodxkz.sHtML

crontab -e;  crontab -l
来源：http://read.share.epnwcf.com/Article/details/gcimaehvp.sHtML

[R67] 生成随机十六进制串
来源：http://baike.tarul.cn/Article/details/glpaxxbqq.sHtML

openssl rand -hex 16
来源：http://m.share.epnwcf.com/Article/details/guyxndlvf.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.sjlbkw.cn/Article/details/gvedkaxyk.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.sjlbkw.cn/Article/details/gqtadhgnw.sHtML

[R69] 生成随机密码
来源：http://m.share.fktsv.cn/Article/details/gjdvduowh.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.yfazqb.com/Article/details/gexfpbnzn.sHtML

[R70] 时间戳与互转
来源：http://www.share.fktsv.cn/Article/details/gbhhznipg.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.vehdjk.com/Article/details/gxydxqxnd.sHtML

[R71] 日期格式化
来源：http://baike.sjlbkw.cn/Article/details/galqpuclb.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.sjlbkw.cn/Article/details/guduwbigy.sHtML

[R72] 等待端口就绪
来源：http://blog.sjlbkw.cn/Article/details/gzphifjhp.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.bbcook.cn/Article/details/gscrjliis.sHtML

[R73] 分割大日志
来源：http://www.m.share.epnwcf.com/Article/details/grwpvpgov.sHtML

split -l 1000 big.log part_
来源：http://m.share.vehdjk.com/Article/details/gxtcifccx.sHtML

[R74] 批量重命名
来源：http://www.share.tarul.cn/Article/details/gjfcissuo.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.epnwcf.com/Article/details/gbrzlplhg.sHtML

[R75] 导出环境变量
来源：http://blog.tarul.cn/Article/details/gyvajkeqt.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.bbcook.cn/Article/details/gipmcyggt.sHtML

[R76] 使用临时文件
来源：http://www.blog.vehdjk.com/Article/details/gtrixnqrx.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.vehdjk.com/Article/details/gmiaanzvd.sHtML

[R77] 读取用户输入
来源：http://www.share.yfazqb.com/Article/details/glttsgasv.sHtML

read -rp "请输入: " ans
来源：http://mobile.epnwcf.com/Article/details/gwcgorugm.sHtML

[R78] 交互式菜单
来源：http://www.blog.sjlbkw.cn/Article/details/gelxmyepm.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.vehdjk.com/Article/details/ggmlvebrv.sHtML

[R79] 解析命令行选项
来源：http://wap.bbcook.cn/Article/details/gwnogpleq.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.epnwcf.com/Article/details/gyfvoikdf.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.epnwcf.com/Article/details/grmnqjeqm.sHtML

time ./run.sh
来源：http://baike.vehdjk.com/Article/details/gmentzhsy.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gxydizykr.sHtML

S. C / C++ 专题
来源：http://mobile.fktsv.cn/Article/details/gyjbcadoz.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gfhredkmg.sHtML

[S01] C：Hello World
来源：http://www.share.vehdjk.com/Article/details/grxdfsgak.sHtML

#include <stdio.h>
来源：http://wap.bbcook.cn/Article/details/gaavwvfnn.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.bbcook.cn/Article/details/gtqmbqpfk.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.epnwcf.com/Article/details/gpnxgvwax.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.tarul.cn/Article/details/gqbzdbvft.sHtML

[S03] C：读入整数
来源：http://m.share.sjlbkw.cn/Article/details/gqqmwtxpa.sHtML

int x; scanf("%d", &x);
来源：http://wap.vehdjk.com/Article/details/gcihtiffv.sHtML

[S04] C：字符串复制
来源：http://m.share.bbcook.cn/Article/details/gnzobyuii.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.bbcook.cn/Article/details/gfduibtny.sHtML

[S05] C：字符串长度
来源：http://blog.tarul.cn/Article/details/gpgjibsxb.sHtML

strlen(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gvlbtceui.sHtML

[S06] C：字符串比较
来源：http://wap.epnwcf.com/Article/details/gpdtbxmua.sHtML

strcmp(a, b) == 0
来源：http://www.blog.sjlbkw.cn/Article/details/gtyfmpvsv.sHtML

[S07] C：数组遍历求和
来源：http://blog.fktsv.cn/Article/details/gkrsbxebh.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.tarul.cn/Article/details/gjiynhzjl.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.sjlbkw.cn/Article/details/gnuadzzao.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.tarul.cn/Article/details/glkzoiwfr.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fktsv.cn/Article/details/gahujmhcw.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fktsv.cn/Article/details/gnsnjdejf.sHtML

[S10] C：指针与解引用
来源：http://3g.fktsv.cn/Article/details/ghndqedyp.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.yfazqb.com/Article/details/ghxqvcqdw.sHtML

[S11] C：逐行读文件
来源：http://m.share.bbcook.cn/Article/details/gmiwwgaqw.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.tarul.cn/Article/details/gonvufrsv.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.fktsv.cn/Article/details/gdqkgafds.sHtML

fclose(f);
来源：http://read.share.bbcook.cn/Article/details/gqqzhmnmu.sHtML

[S12] C：写文件
来源：http://www.m.share.epnwcf.com/Article/details/gcyxqslvh.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.yfazqb.com/Article/details/gcsshgfef.sHtML

[S13] C：宏定义
来源：http://mobile.fktsv.cn/Article/details/gwcjrgutz.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.sjlbkw.cn/Article/details/gtklnftxv.sHtML

[S14] C：枚举
来源：http://www.m.share.vehdjk.com/Article/details/gddljwjdn.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.tarul.cn/Article/details/gpcqztmtv.sHtML

[S15] C：类型转换
来源：http://www.m.share.bbcook.cn/Article/details/gmpsnaosi.sHtML

(double) a / b
来源：http://m.share.yfazqb.com/Article/details/gefmxzkbf.sHtML

[S16] C：位操作置位
来源：http://www.blog.bbcook.cn/Article/details/grqrwhurw.sHtML

x |= (1 << 3);
来源：http://m.share.tarul.cn/Article/details/gunxqdvjw.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.epnwcf.com/Article/details/gwomccilu.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.bbcook.cn/Article/details/guiyxbznl.sHtML

[S18] C：命令行参数
来源：http://3g.tarul.cn/Article/details/gnjxpmvfk.sHtML

int main(int argc, char **argv)
来源：http://read.share.fktsv.cn/Article/details/gntbkdyvi.sHtML

[S19] C：快速排序
来源：http://www.share.epnwcf.com/Article/details/gigyydkbj.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.vehdjk.com/Article/details/gzevwjhhv.sHtML

[S20] C：二分查找
来源：http://www.share.bbcook.cn/Article/details/gojpdsxjq.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.yfazqb.com/Article/details/gbqevdkyf.sHtML

[S21] C：字符类别判断
来源：http://read.share.fktsv.cn/Article/details/gqpyqqlho.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.sjlbkw.cn/Article/details/gyjcsvtxt.sHtML

[S22] C：字符串转数字
来源：http://www.blog.yfazqb.com/Article/details/gqdhymjgp.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.fktsv.cn/Article/details/gqvjaydgq.sHtML

[S23] C：随机数
来源：http://m.share.tarul.cn/Article/details/guehnezzp.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.yfazqb.com/Article/details/gehxcvsaf.sHtML

[S24] C：获取本地时间
来源：http://wap.bbcook.cn/Article/details/glfmrhxpp.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.vehdjk.com/Article/details/gebibxujs.sHtML

[S25] C：内存拷贝
来源：http://m.share.yfazqb.com/Article/details/goqmazyld.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.vehdjk.com/Article/details/gojwvtnam.sHtML

[S26] C：内存清零
来源：http://www.m.share.epnwcf.com/Article/details/gmznudbff.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fktsv.cn/Article/details/gvygbgrmz.sHtML

[S27] C：定义常量
来源：http://baike.sjlbkw.cn/Article/details/guqxcktzv.sHtML

const double PI = 3.14159;
来源：http://read.share.tarul.cn/Article/details/gxiyymbit.sHtML

[S28] C：静态变量
来源：http://blog.tarul.cn/Article/details/gxxewbgev.sHtML

static int counter = 0;
来源：http://www.m.share.bbcook.cn/Article/details/glybwtmpu.sHtML

[S29] C：变参函数
来源：http://3g.bbcook.cn/Article/details/gikqcjukl.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.vehdjk.com/Article/details/gbbomwhlu.sHtML

[S30] C：头文件保护
来源：http://www.blog.epnwcf.com/Article/details/gdymumeqd.sHtML

#ifndef X_H
来源：http://m.share.bbcook.cn/Article/details/guqilenyy.sHtML

#define X_H
来源：http://m.share.epnwcf.com/Article/details/gcymoavwy.sHtML

#endif
来源：http://3g.yfazqb.com/Article/details/gboxvzrxt.sHtML

[S31] C++：Hello World
来源：http://www.share.vehdjk.com/Article/details/gouqmfzou.sHtML

#include <iostream>
来源：http://www.blog.bbcook.cn/Article/details/gdeztvcxn.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.epnwcf.com/Article/details/gsxbhnsko.sHtML

[S32] C++：字符串
来源：http://www.share.tarul.cn/Article/details/gzdkraioc.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.fktsv.cn/Article/details/gxarefxvg.sHtML

[S33] C++：vector 增删
来源：http://www.share.yfazqb.com/Article/details/giswwhzds.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.fktsv.cn/Article/details/gcdwjdxge.sHtML

[S34] C++：遍历 vector
来源：http://mobile.tarul.cn/Article/details/gvnihxhjy.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fktsv.cn/Article/details/gsqnorkem.sHtML

[S35] C++：map
来源：http://www.blog.sjlbkw.cn/Article/details/gvkefpyki.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.sjlbkw.cn/Article/details/ghqnckprg.sHtML

[S36] C++：unordered_map
来源：http://baike.fktsv.cn/Article/details/gpaqqrkfp.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.vehdjk.com/Article/details/gvpqbahuq.sHtML

[S37] C++：set
来源：http://baike.bbcook.cn/Article/details/gfioghtwc.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.vehdjk.com/Article/details/grhoczszt.sHtML

[S38] C++：排序
来源：http://www.blog.epnwcf.com/Article/details/gicojjtuf.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.sjlbkw.cn/Article/details/gobilsyyu.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.yfazqb.com/Article/details/gmbfthwjp.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.bbcook.cn/Article/details/gpavnlzpn.sHtML

[S40] C++：查找元素
来源：http://3g.yfazqb.com/Article/details/gqkefdvax.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.tarul.cn/Article/details/gdcphcnpg.sHtML

[S41] C++：类与构造函数
来源：http://read.share.vehdjk.com/Article/details/gawyrlcah.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.vehdjk.com/Article/details/gqlgnrgzn.sHtML

[S42] C++：继承与虚函数
来源：http://blog.vehdjk.com/Article/details/gdpqcvqby.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.bbcook.cn/Article/details/germauujx.sHtML

[S43] C++：智能指针
来源：http://wap.tarul.cn/Article/details/gejvrfvom.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.tarul.cn/Article/details/gckcreoto.sHtML

[S44] C++：引用传参
来源：http://blog.vehdjk.com/Article/details/glyikbudb.sHtML

void inc(int &x) { ++x; }
来源：http://3g.yfazqb.com/Article/details/gztevrkjt.sHtML

[S45] C++：lambda
来源：http://3g.epnwcf.com/Article/details/guaehxdsr.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.fktsv.cn/Article/details/gnklldcbm.sHtML

[S46] C++：函数模板
来源：http://m.share.bbcook.cn/Article/details/gfwkhuyhi.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.sjlbkw.cn/Article/details/gakanbtda.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.epnwcf.com/Article/details/gzhqwpuzd.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.sjlbkw.cn/Article/details/gbvmjcnnz.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.vehdjk.com/Article/details/gjxdvdikm.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.vehdjk.com/Article/details/gghtcbewe.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.vehdjk.com/Article/details/gyfybwbxk.sHtML

[S49] C++：写文件
来源：http://www.m.share.epnwcf.com/Article/details/gwpkellju.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.tarul.cn/Article/details/gnpypdyrl.sHtML

[S50] C++：格式化数字
来源：http://3g.bbcook.cn/Article/details/ghvchrttx.sHtML


<!-- 参考信息 -->