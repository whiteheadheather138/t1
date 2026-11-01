代发 wailian999

[Q82] 字符长度与字节长度
来源：http://www.blog.epnwcf.com/Article/details/gwduhmmtz.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/gmaxypqqb.sHtML

[Q83] 大小写转换
来源：http://baike.yfazqb.com/Article/details/gluephrnf.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/gtjgdshuv.sHtML

[Q84] 去除首尾空格
来源：http://blog.vehdjk.com/Article/details/giesunvgp.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.fktsv.cn/Article/details/gytywwphn.sHtML

[Q85] 数值取整
来源：http://mobile.epnwcf.com/Article/details/gjnardkqh.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.fktsv.cn/Article/details/gtaynhpdx.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.sjlbkw.cn/Article/details/gwexjclzn.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.fktsv.cn/Article/details/ginhnfzir.sHtML

[Q87] JSON 字段做条件
来源：http://baike.epnwcf.com/Article/details/grousttuk.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.fktsv.cn/Article/details/gbpkfrjhy.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.bbcook.cn/Article/details/gqrgnuorq.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.tarul.cn/Article/details/grwhsegix.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.bbcook.cn/Article/details/gngyamazr.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.yfazqb.com/Article/details/ghjzhjffc.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.yfazqb.com/Article/details/golutywdi.sHtML

[Q90] 生成序号列
来源：http://www.m.share.vehdjk.com/Article/details/gtfftfaur.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.sjlbkw.cn/Article/details/gvifoeens.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gxpsnllsh.sHtML

R. Bash 专题
来源：http://baike.epnwcf.com/Article/details/gpuselskk.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gbzwrwgez.sHtML

[R01] shebang 与严格模式
来源：http://baike.bbcook.cn/Article/details/gwqckhyjz.sHtML

#!/usr/bin/env bash
来源：http://www.share.bbcook.cn/Article/details/grgwemukb.sHtML

set -euo pipefail
来源：http://blog.fktsv.cn/Article/details/gtffxodan.sHtML

[R02] 变量赋值与使用
来源：http://read.share.yfazqb.com/Article/details/gctnwxjyn.sHtML

name="Tom"; echo "$name"
来源：http://m.share.bbcook.cn/Article/details/gpfewhbic.sHtML

[R03] 只读变量
来源：http://www.blog.tarul.cn/Article/details/gpxppzwaq.sHtML

readonly PI=3.14
来源：http://blog.fktsv.cn/Article/details/gyextlbus.sHtML

[R04] 位置参数
来源：http://mobile.epnwcf.com/Article/details/gywwblxci.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.sjlbkw.cn/Article/details/gtienoicm.sHtML

[R05] 参数默认值
来源：http://blog.vehdjk.com/Article/details/gmgryijfq.sHtML

name="${1:-default}"
来源：http://3g.yfazqb.com/Article/details/gwnhmmgke.sHtML

[R06] 判断命令是否存在
来源：http://wap.fktsv.cn/Article/details/gbwlxcapw.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.epnwcf.com/Article/details/grcmkkovf.sHtML

[R07] if 判断文件
来源：http://baike.tarul.cn/Article/details/glfnfslge.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.epnwcf.com/Article/details/ggfjyrdaf.sHtML

[R08] 数值比较
来源：http://3g.epnwcf.com/Article/details/ghndhvjmv.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.vehdjk.com/Article/details/gpmsajrsg.sHtML

[R09] 字符串比较
来源：http://baike.sjlbkw.cn/Article/details/gecvoykna.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.epnwcf.com/Article/details/gqhpmufnb.sHtML

[R10] 正则匹配
来源：http://m.share.yfazqb.com/Article/details/gmmqnknbe.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.fktsv.cn/Article/details/gdcwcodeh.sHtML

[R11] case 多分支
来源：http://blog.yfazqb.com/Article/details/gaqwtqiqa.sHtML

case "$1" in
来源：http://www.share.vehdjk.com/Article/details/gflfwxmup.sHtML

start) echo "启动" ;;
来源：http://mobile.vehdjk.com/Article/details/glyjivetc.sHtML

stop)  echo "停止" ;;
来源：http://www.share.bbcook.cn/Article/details/gielpdtea.sHtML

*)     echo "未知命令" ;;
来源：http://wap.yfazqb.com/Article/details/gkgatvabp.sHtML

esac
来源：http://read.share.yfazqb.com/Article/details/gjpjwduxy.sHtML

[R12] for 遍历文件
来源：http://www.share.bbcook.cn/Article/details/ganvjlvsn.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.sjlbkw.cn/Article/details/gxhnklfzb.sHtML

[R13] for 计数循环
来源：http://blog.yfazqb.com/Article/details/gadmyvtjg.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.yfazqb.com/Article/details/glmzjzwdt.sHtML

[R14] C 风格 for
来源：http://read.share.yfazqb.com/Article/details/gmnccawdt.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.tarul.cn/Article/details/gbizezwsn.sHtML

[R15] while 逐行读文件
来源：http://www.share.vehdjk.com/Article/details/gbzywbxvm.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.fktsv.cn/Article/details/gzccpxhpn.sHtML

[R16] until 等待条件
来源：http://www.m.share.epnwcf.com/Article/details/gfqmfmvjt.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.yfazqb.com/Article/details/gaeisjpfm.sHtML

[R17] 数组定义与取值
来源：http://wap.yfazqb.com/Article/details/gcrwahonf.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.sjlbkw.cn/Article/details/gwutexsdm.sHtML

[R18] 遍历数组
来源：http://wap.vehdjk.com/Article/details/ghmxlvoqf.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.fktsv.cn/Article/details/gkmchvzaq.sHtML

[R19] 数组长度
来源：http://m.share.vehdjk.com/Article/details/grgbngylj.sHtML

echo "${#arr[@]}"
来源：http://m.share.tarul.cn/Article/details/gpgyjhhwe.sHtML

[R20] 关联数组（字典）
来源：http://baike.vehdjk.com/Article/details/gbtrxwswa.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.tarul.cn/Article/details/gkbeqwyhv.sHtML

[R21] 字符串长度
来源：http://read.share.tarul.cn/Article/details/gzjqijcap.sHtML

echo "${#s}"
来源：http://www.m.share.bbcook.cn/Article/details/goonmgzgy.sHtML

[R22] 截取子串
来源：http://www.blog.epnwcf.com/Article/details/gudgipsqf.sHtML

echo "${s:0:5}"
来源：http://www.blog.yfazqb.com/Article/details/gveanzphb.sHtML

[R23] 字符串替换
来源：http://wap.sjlbkw.cn/Article/details/gquywtlfr.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.tarul.cn/Article/details/grluqscie.sHtML

[R24] 大小写转换
来源：http://blog.epnwcf.com/Article/details/glfvmxahk.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.yfazqb.com/Article/details/gochwrdof.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.vehdjk.com/Article/details/gnsocymkw.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.fktsv.cn/Article/details/gjfxmhnmb.sHtML

[R26] 命令替换
来源：http://baike.vehdjk.com/Article/details/gngqmgnra.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.epnwcf.com/Article/details/gurmmftcs.sHtML

[R27] 算术展开
来源：http://www.m.share.bbcook.cn/Article/details/gubxcwrzp.sHtML

echo $((1 + 2 * 3))
来源：http://wap.sjlbkw.cn/Article/details/gtfbtvzet.sHtML

[R28] 浮点运算
来源：http://www.share.bbcook.cn/Article/details/gmulohiui.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.fktsv.cn/Article/details/gpyfahray.sHtML

[R29] 定义函数
来源：http://www.blog.vehdjk.com/Article/details/gxsalhsem.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.fktsv.cn/Article/details/galmwfqbq.sHtML

[R30] 函数返回状态码
来源：http://3g.vehdjk.com/Article/details/gtddwbagk.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.bbcook.cn/Article/details/gengtylcz.sHtML

[R31] 局部变量
来源：http://m.share.sjlbkw.cn/Article/details/gkipmlmxn.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.epnwcf.com/Article/details/gwlyujjpj.sHtML

[R32] 参数个数校验
来源：http://3g.epnwcf.com/Article/details/gjglbuhfp.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.yfazqb.com/Article/details/gtnpwlvwv.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.yfazqb.com/Article/details/gezkrvwyt.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.bbcook.cn/Article/details/gypzykvmw.sHtML

[R34] 退出时清理
来源：http://wap.bbcook.cn/Article/details/gfnqmrslo.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.sjlbkw.cn/Article/details/ggxbiqufv.sHtML

[R35] 后台执行并等待
来源：http://www.blog.yfazqb.com/Article/details/gewutatwg.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.fktsv.cn/Article/details/guppeijcp.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.sjlbkw.cn/Article/details/gmbtnwxdq.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.sjlbkw.cn/Article/details/gyaitsazp.sHtML

[R37] 把输出赋给变量
来源：http://blog.tarul.cn/Article/details/grlyufsbl.sHtML

files=$(ls -1)
来源：http://www.share.vehdjk.com/Article/details/gkkjrufld.sHtML

[R38] 管道串联
来源：http://baike.yfazqb.com/Article/details/gtmelsanq.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.sjlbkw.cn/Article/details/gtsdqthfr.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.epnwcf.com/Article/details/gcvzavyit.sHtML

cmd > out.log 2>&1
来源：http://read.share.yfazqb.com/Article/details/ghpurjnrq.sHtML

[R40] 追加写日志
来源：http://m.share.tarul.cn/Article/details/gehgmyjhm.sHtML

echo "log" >> out.log
来源：http://wap.yfazqb.com/Article/details/gklynbapf.sHtML

[R41] 丢弃输出
来源：http://wap.tarul.cn/Article/details/gylbubnfn.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.vehdjk.com/Article/details/gscaovbga.sHtML

[R42] 输入重定向
来源：http://www.m.share.epnwcf.com/Article/details/gbpuqafgg.sHtML

wc -l < a.txt
来源：http://www.share.yfazqb.com/Article/details/ggfrwelmi.sHtML

[R43] 按名字查找文件
来源：http://blog.sjlbkw.cn/Article/details/gmmujhbwk.sHtML

find . -name "*.log" -type f
来源：http://read.share.vehdjk.com/Article/details/gdadrhyjy.sHtML

[R44] 按修改时间查找
来源：http://read.share.sjlbkw.cn/Article/details/ghqevgwpv.sHtML

find . -mtime -7 -type f
来源：http://www.share.epnwcf.com/Article/details/gzgwemwph.sHtML

[R45] 批量删除
来源：http://wap.fktsv.cn/Article/details/gcbzpogtw.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.epnwcf.com/Article/details/gvingtfla.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fktsv.cn/Article/details/gvmwdozyy.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.tarul.cn/Article/details/ggxhkapih.sHtML

[R47] sed 单行替换
来源：http://wap.yfazqb.com/Article/details/googxqxtv.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fktsv.cn/Article/details/gfgxannze.sHtML

[R48] awk 取指定列
来源：http://mobile.epnwcf.com/Article/details/gtjujymls.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.sjlbkw.cn/Article/details/gtltyitjc.sHtML

[R49] awk 带条件
来源：http://www.m.share.yfazqb.com/Article/details/glfcgdspp.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.tarul.cn/Article/details/gywdduewf.sHtML

[R50] awk 求和
来源：http://www.blog.vehdjk.com/Article/details/glvkdnchm.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fktsv.cn/Article/details/gpgwqmzjf.sHtML

[R51] 排序去重取前几
来源：http://baike.vehdjk.com/Article/details/gfclivdzh.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.yfazqb.com/Article/details/gohssoywt.sHtML

[R52] 统计行数
来源：http://www.share.yfazqb.com/Article/details/gfncdzqrc.sHtML

wc -l a.txt
来源：http://www.m.share.epnwcf.com/Article/details/gqfbhkurt.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.sjlbkw.cn/Article/details/glonikkrr.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.epnwcf.com/Article/details/gvsknzuih.sHtML

[R54] 比较两个文件
来源：http://read.share.fktsv.cn/Article/details/ghqhoexxl.sHtML

diff a.txt b.txt
来源：http://m.share.fktsv.cn/Article/details/geljasbsu.sHtML

[R55] 压缩与解压
来源：http://3g.sjlbkw.cn/Article/details/grvabnrjq.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.bbcook.cn/Article/details/gcdolljit.sHtML

[R56] 远程拷贝
来源：http://www.share.vehdjk.com/Article/details/gbqhqghet.sHtML

scp file user@host:/path/
来源：http://m.share.vehdjk.com/Article/details/gtitkbaqt.sHtML

[R57] 远程执行命令
来源：http://www.m.share.sjlbkw.cn/Article/details/gqzxarctd.sHtML

ssh user@host 'uptime'
来源：http://www.blog.epnwcf.com/Article/details/gcmscittm.sHtML

[R58] 下载文件
来源：http://baike.yfazqb.com/Article/details/gtwfwpmtp.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.vehdjk.com/Article/details/gayfcrtdn.sHtML

[R59] 发 POST JSON
来源：http://m.share.epnwcf.com/Article/details/gpeqxxtxv.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.sjlbkw.cn/Article/details/glbgwgmgf.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.yfazqb.com/Article/details/gbbngbodn.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.bbcook.cn/Article/details/gxeungqaj.sHtML

[R61] 磁盘占用
来源：http://blog.bbcook.cn/Article/details/gympdupep.sHtML

df -h;  du -sh *
来源：http://3g.tarul.cn/Article/details/gdonthwwm.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.vehdjk.com/Article/details/ghxsxpuhg.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.bbcook.cn/Article/details/gvyjptoth.sHtML

[R63] 内存与进程
来源：http://3g.sjlbkw.cn/Article/details/gwsttgjba.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.tarul.cn/Article/details/gkzisldlh.sHtML

[R64] 结束进程
来源：http://baike.yfazqb.com/Article/details/ggsrepohw.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.bbcook.cn/Article/details/gcmjjkfgg.sHtML

[R65] 查看端口占用
来源：http://www.blog.bbcook.cn/Article/details/gezaypigd.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.fktsv.cn/Article/details/geurrkbpv.sHtML

[R66] 定时任务
来源：http://blog.yfazqb.com/Article/details/gguzggooe.sHtML

crontab -e;  crontab -l
来源：http://www.share.tarul.cn/Article/details/gscksfixf.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.bbcook.cn/Article/details/gwpugvntz.sHtML

openssl rand -hex 16
来源：http://3g.tarul.cn/Article/details/gcjzjmvvp.sHtML

[R68] 计算文件校验值
来源：http://3g.epnwcf.com/Article/details/grouuskcp.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.epnwcf.com/Article/details/gyuwuizam.sHtML

[R69] 生成随机密码
来源：http://www.blog.fktsv.cn/Article/details/gyykteead.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.epnwcf.com/Article/details/gfifzjeuw.sHtML

[R70] 时间戳与互转
来源：http://3g.fktsv.cn/Article/details/ghrkgfipd.sHtML

date +%s;  date -d @1700000000
来源：http://baike.vehdjk.com/Article/details/ggueojgpc.sHtML

[R71] 日期格式化
来源：http://read.share.epnwcf.com/Article/details/gbvkstgor.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.sjlbkw.cn/Article/details/gysnjnuqh.sHtML

[R72] 等待端口就绪
来源：http://www.blog.bbcook.cn/Article/details/gutlertso.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.tarul.cn/Article/details/ghafpgoyo.sHtML

[R73] 分割大日志
来源：http://mobile.vehdjk.com/Article/details/gvjuaumll.sHtML

split -l 1000 big.log part_
来源：http://www.share.epnwcf.com/Article/details/gkjnqtzvl.sHtML

[R74] 批量重命名
来源：http://www.m.share.bbcook.cn/Article/details/gdtikhxfd.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.vehdjk.com/Article/details/gtqohuicv.sHtML

[R75] 导出环境变量
来源：http://www.share.sjlbkw.cn/Article/details/gpomgqqcq.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.sjlbkw.cn/Article/details/gmenlhalt.sHtML

[R76] 使用临时文件
来源：http://mobile.bbcook.cn/Article/details/geduoezcn.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fktsv.cn/Article/details/gzxsneiub.sHtML

[R77] 读取用户输入
来源：http://www.m.share.yfazqb.com/Article/details/ghqyydytx.sHtML

read -rp "请输入: " ans
来源：http://mobile.epnwcf.com/Article/details/gqbnkgkal.sHtML

[R78] 交互式菜单
来源：http://3g.bbcook.cn/Article/details/ggyypsuul.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.sjlbkw.cn/Article/details/gcsgcvisi.sHtML

[R79] 解析命令行选项
来源：http://baike.epnwcf.com/Article/details/geqdhqvcx.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.tarul.cn/Article/details/gnytxzvyv.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.yfazqb.com/Article/details/gxmblfope.sHtML

time ./run.sh
来源：http://www.blog.tarul.cn/Article/details/gwgjrkdtp.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gjrhtmewb.sHtML

S. C / C++ 专题
来源：http://read.share.vehdjk.com/Article/details/gpdnzbrmr.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gijhkvxwq.sHtML

[S01] C：Hello World
来源：http://baike.epnwcf.com/Article/details/gbntdhiou.sHtML

#include <stdio.h>
来源：http://read.share.bbcook.cn/Article/details/gbhqnyubt.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.yfazqb.com/Article/details/gnbflstau.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fktsv.cn/Article/details/gxtxosxas.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.bbcook.cn/Article/details/gmlecddcu.sHtML

[S03] C：读入整数
来源：http://3g.tarul.cn/Article/details/guowudixr.sHtML

int x; scanf("%d", &x);
来源：http://www.share.yfazqb.com/Article/details/gzsrwpolq.sHtML

[S04] C：字符串复制
来源：http://read.share.epnwcf.com/Article/details/gwchghdba.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.fktsv.cn/Article/details/ggqwqlpju.sHtML

[S05] C：字符串长度
来源：http://www.m.share.epnwcf.com/Article/details/gzdrewcas.sHtML

strlen(s)
来源：http://www.share.epnwcf.com/Article/details/gwlaefxpw.sHtML

[S06] C：字符串比较
来源：http://baike.vehdjk.com/Article/details/gaaqegwiw.sHtML

strcmp(a, b) == 0
来源：http://3g.sjlbkw.cn/Article/details/gjeahgkzx.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fktsv.cn/Article/details/gxnnovihe.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.yfazqb.com/Article/details/ggjcadhmp.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.sjlbkw.cn/Article/details/gogcrqhev.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.yfazqb.com/Article/details/gvbjmutkw.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.bbcook.cn/Article/details/gzqoxtzsj.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.vehdjk.com/Article/details/grucvnajw.sHtML

[S10] C：指针与解引用
来源：http://baike.tarul.cn/Article/details/glpbvnjeq.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.sjlbkw.cn/Article/details/gaqjodmyl.sHtML

[S11] C：逐行读文件
来源：http://mobile.bbcook.cn/Article/details/giryaagvm.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.yfazqb.com/Article/details/gbcwxtaxn.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.sjlbkw.cn/Article/details/geckfygpw.sHtML

fclose(f);
来源：http://mobile.sjlbkw.cn/Article/details/gkwzdnjtm.sHtML

[S12] C：写文件
来源：http://read.share.bbcook.cn/Article/details/glfpeksqa.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.vehdjk.com/Article/details/gndbplwdf.sHtML

[S13] C：宏定义
来源：http://wap.sjlbkw.cn/Article/details/gfnhcihce.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.vehdjk.com/Article/details/gtqmdjgby.sHtML

[S14] C：枚举
来源：http://read.share.fktsv.cn/Article/details/gtynlgxkz.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.epnwcf.com/Article/details/gynxsxngx.sHtML

[S15] C：类型转换
来源：http://wap.yfazqb.com/Article/details/gsxvzjfmg.sHtML

(double) a / b
来源：http://www.m.share.bbcook.cn/Article/details/gbhbrbkpe.sHtML

[S16] C：位操作置位
来源：http://mobile.yfazqb.com/Article/details/gcaojoruo.sHtML

x |= (1 << 3);
来源：http://www.blog.tarul.cn/Article/details/giqosnzwz.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.bbcook.cn/Article/details/glrdrlswk.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fktsv.cn/Article/details/gcyoouoir.sHtML

[S18] C：命令行参数
来源：http://blog.epnwcf.com/Article/details/gkudgzxkr.sHtML

int main(int argc, char **argv)
来源：http://m.share.sjlbkw.cn/Article/details/goiqfmzwd.sHtML

[S19] C：快速排序
来源：http://www.m.share.tarul.cn/Article/details/getsvsiwc.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.sjlbkw.cn/Article/details/glzxudfkw.sHtML

[S20] C：二分查找
来源：http://www.m.share.yfazqb.com/Article/details/gquohmqqp.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.fktsv.cn/Article/details/ginonvkfi.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fktsv.cn/Article/details/gdeghzphk.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.epnwcf.com/Article/details/gbvuaebzu.sHtML

[S22] C：字符串转数字
来源：http://baike.bbcook.cn/Article/details/gccujhchz.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.sjlbkw.cn/Article/details/gailhxnxo.sHtML

[S23] C：随机数
来源：http://baike.epnwcf.com/Article/details/gudgcyubr.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.tarul.cn/Article/details/gzmcgdqrr.sHtML

[S24] C：获取本地时间
来源：http://3g.sjlbkw.cn/Article/details/gsfsdxjmo.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.vehdjk.com/Article/details/gjdoqdjcq.sHtML

[S25] C：内存拷贝
来源：http://read.share.yfazqb.com/Article/details/gxxwwntub.sHtML

memcpy(dst, src, n);
来源：http://www.blog.sjlbkw.cn/Article/details/gfiiazgla.sHtML

[S26] C：内存清零
来源：http://mobile.vehdjk.com/Article/details/gejggjcrg.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fktsv.cn/Article/details/gherjyaeq.sHtML

[S27] C：定义常量
来源：http://mobile.bbcook.cn/Article/details/gfuprysdj.sHtML

const double PI = 3.14159;
来源：http://www.blog.bbcook.cn/Article/details/giyursgts.sHtML

[S28] C：静态变量
来源：http://mobile.fktsv.cn/Article/details/gkxvqkqut.sHtML

static int counter = 0;
来源：http://blog.yfazqb.com/Article/details/gqconkkat.sHtML

[S29] C：变参函数
来源：http://blog.tarul.cn/Article/details/gfqiphldy.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.yfazqb.com/Article/details/ggvknnivr.sHtML

[S30] C：头文件保护
来源：http://mobile.bbcook.cn/Article/details/gttmrfsfr.sHtML

#ifndef X_H
来源：http://read.share.tarul.cn/Article/details/gqzamtktj.sHtML

#define X_H
来源：http://www.m.share.bbcook.cn/Article/details/gvqiinukj.sHtML

#endif
来源：http://wap.sjlbkw.cn/Article/details/gzjtmzdri.sHtML

[S31] C++：Hello World
来源：http://baike.yfazqb.com/Article/details/gtgynfgqx.sHtML

#include <iostream>
来源：http://baike.tarul.cn/Article/details/ganvcdnat.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.tarul.cn/Article/details/gknegfsfz.sHtML

[S32] C++：字符串
来源：http://3g.bbcook.cn/Article/details/geakjpcuk.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.fktsv.cn/Article/details/gxncehfeg.sHtML

[S33] C++：vector 增删
来源：http://www.blog.sjlbkw.cn/Article/details/gkrrfgflr.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.yfazqb.com/Article/details/gxpiveifb.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.sjlbkw.cn/Article/details/gxjuzlgba.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.vehdjk.com/Article/details/grrrqubyw.sHtML

[S35] C++：map
来源：http://3g.vehdjk.com/Article/details/ghlulstsy.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fktsv.cn/Article/details/ggdllmzyq.sHtML

[S36] C++：unordered_map
来源：http://mobile.sjlbkw.cn/Article/details/gwngnkaie.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.bbcook.cn/Article/details/gefdufoaw.sHtML

[S37] C++：set
来源：http://read.share.yfazqb.com/Article/details/gqxktywew.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.epnwcf.com/Article/details/gyekzsmxg.sHtML

[S38] C++：排序
来源：http://read.share.bbcook.cn/Article/details/gdqjcxriz.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fktsv.cn/Article/details/gkjcsivqt.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.tarul.cn/Article/details/gfowjwroq.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.tarul.cn/Article/details/gzxrkxkin.sHtML

[S40] C++：查找元素
来源：http://www.m.share.yfazqb.com/Article/details/gctlibphx.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.tarul.cn/Article/details/gzyokylks.sHtML

[S41] C++：类与构造函数
来源：http://read.share.tarul.cn/Article/details/gllwvhryy.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.vehdjk.com/Article/details/gdznnjfzg.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.vehdjk.com/Article/details/giaurvuwt.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.vehdjk.com/Article/details/gnaakbslk.sHtML

[S43] C++：智能指针
来源：http://www.blog.bbcook.cn/Article/details/gnjepnyqk.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.tarul.cn/Article/details/gwfbyjuot.sHtML

[S44] C++：引用传参
来源：http://www.share.bbcook.cn/Article/details/gtdwavtat.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.bbcook.cn/Article/details/gmfhfwtjv.sHtML

[S45] C++：lambda
来源：http://blog.yfazqb.com/Article/details/gfvrciucn.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.vehdjk.com/Article/details/gbfrgxwoj.sHtML

[S46] C++：函数模板
来源：http://3g.sjlbkw.cn/Article/details/gbjednrct.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.fktsv.cn/Article/details/gzqsipyrw.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.vehdjk.com/Article/details/gpofpjaeo.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.vehdjk.com/Article/details/gppdszxta.sHtML

[S48] C++：逐行读文件
来源：http://3g.fktsv.cn/Article/details/gcaseszvc.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.bbcook.cn/Article/details/gsfkadomi.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fktsv.cn/Article/details/gqxqegleh.sHtML

[S49] C++：写文件
来源：http://www.blog.sjlbkw.cn/Article/details/gbheafgbq.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.tarul.cn/Article/details/gnglkdchh.sHtML

[S50] C++：格式化数字
来源：http://blog.yfazqb.com/Article/details/gpqewvvnb.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.sjlbkw.cn/Article/details/gptbpvrmy.sHtML

[S51] C++：显式类型转换
来源：http://wap.tarul.cn/Article/details/gnptzsoyg.sHtML

static_cast<double>(a) / b
来源：http://www.blog.epnwcf.com/Article/details/ghoeyjium.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.fktsv.cn/Article/details/gevjxlszv.sHtML


<!-- 参考信息 -->