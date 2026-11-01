代发 wailian999

[Q86] 读取 JSON 字段
来源：http://www.share.sjlbkw.cn/Article/details/ghwmrydtb.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.tarul.cn/Article/details/gmshtanfa.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.vehdjk.com/Article/details/gvmwyxfzz.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.vehdjk.com/Article/details/glkesoerr.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.tarul.cn/Article/details/gbkgejdng.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.yfazqb.com/Article/details/gvjzmvbre.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.sjlbkw.cn/Article/details/gsyrjllif.sHtML

[Q89] 判断表是否存在
来源：http://wap.fktsv.cn/Article/details/gfwtcjxdh.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.epnwcf.com/Article/details/gefqnyinr.sHtML

[Q90] 生成序号列
来源：http://www.share.tarul.cn/Article/details/gjamltoiz.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.yfazqb.com/Article/details/gvipynorc.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gwgxvsdlo.sHtML

R. Bash 专题
来源：http://wap.epnwcf.com/Article/details/gfawybzqe.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/ghnbntjso.sHtML

[R01] shebang 与严格模式
来源：http://baike.fktsv.cn/Article/details/gqskngiqi.sHtML

#!/usr/bin/env bash
来源：http://wap.fktsv.cn/Article/details/gcgzykafl.sHtML

set -euo pipefail
来源：http://3g.fktsv.cn/Article/details/gptgfncwp.sHtML

[R02] 变量赋值与使用
来源：http://read.share.sjlbkw.cn/Article/details/gyfqcbvok.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.vehdjk.com/Article/details/gmaavznfh.sHtML

[R03] 只读变量
来源：http://3g.bbcook.cn/Article/details/gbblajwgw.sHtML

readonly PI=3.14
来源：http://3g.yfazqb.com/Article/details/ghjzflqtf.sHtML

[R04] 位置参数
来源：http://mobile.bbcook.cn/Article/details/gluspxhrq.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.epnwcf.com/Article/details/gmeeljyup.sHtML

[R05] 参数默认值
来源：http://www.blog.yfazqb.com/Article/details/gshdajvpy.sHtML

name="${1:-default}"
来源：http://mobile.bbcook.cn/Article/details/ggegpzqpu.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.tarul.cn/Article/details/ggwnxcnnr.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.bbcook.cn/Article/details/grqnqikip.sHtML

[R07] if 判断文件
来源：http://baike.bbcook.cn/Article/details/gicpyztxv.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.vehdjk.com/Article/details/gcnatvxuk.sHtML

[R08] 数值比较
来源：http://read.share.epnwcf.com/Article/details/gseyhhcej.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.yfazqb.com/Article/details/gqudbnyfk.sHtML

[R09] 字符串比较
来源：http://wap.epnwcf.com/Article/details/gxyilkmbs.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.epnwcf.com/Article/details/gtbtgojne.sHtML

[R10] 正则匹配
来源：http://m.share.yfazqb.com/Article/details/grkgleudz.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.epnwcf.com/Article/details/glfoxktzt.sHtML

[R11] case 多分支
来源：http://baike.vehdjk.com/Article/details/gzjemjvwa.sHtML

case "$1" in
来源：http://mobile.fktsv.cn/Article/details/gyhlwrfah.sHtML

start) echo "启动" ;;
来源：http://www.blog.epnwcf.com/Article/details/gnjhzomdj.sHtML

stop)  echo "停止" ;;
来源：http://blog.tarul.cn/Article/details/gtpvqkaio.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.bbcook.cn/Article/details/gnnndnhdc.sHtML

esac
来源：http://www.m.share.epnwcf.com/Article/details/ghhsecbyh.sHtML

[R12] for 遍历文件
来源：http://www.blog.bbcook.cn/Article/details/gxrbbtjug.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.fktsv.cn/Article/details/gngwoqecl.sHtML

[R13] for 计数循环
来源：http://www.share.bbcook.cn/Article/details/gkyumbaig.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.epnwcf.com/Article/details/giswghzos.sHtML

[R14] C 风格 for
来源：http://m.share.epnwcf.com/Article/details/gpndnxcia.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.epnwcf.com/Article/details/gmnupxhei.sHtML

[R15] while 逐行读文件
来源：http://3g.fktsv.cn/Article/details/giikhimoq.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.bbcook.cn/Article/details/gghohgmkg.sHtML

[R16] until 等待条件
来源：http://wap.tarul.cn/Article/details/gvpqbhgru.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.tarul.cn/Article/details/gvaviqevq.sHtML

[R17] 数组定义与取值
来源：http://3g.epnwcf.com/Article/details/gjkdwndbn.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.vehdjk.com/Article/details/gjhexfhqn.sHtML

[R18] 遍历数组
来源：http://3g.yfazqb.com/Article/details/grqporixr.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.tarul.cn/Article/details/gywtwwtlq.sHtML

[R19] 数组长度
来源：http://m.share.sjlbkw.cn/Article/details/gywwaghiv.sHtML

echo "${#arr[@]}"
来源：http://baike.yfazqb.com/Article/details/glsullfkt.sHtML

[R20] 关联数组（字典）
来源：http://mobile.sjlbkw.cn/Article/details/gazqfpflc.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.yfazqb.com/Article/details/gggbjequg.sHtML

[R21] 字符串长度
来源：http://3g.epnwcf.com/Article/details/gqwlntbpu.sHtML

echo "${#s}"
来源：http://3g.yfazqb.com/Article/details/gwvdelfoa.sHtML

[R22] 截取子串
来源：http://read.share.epnwcf.com/Article/details/gotftkhnq.sHtML

echo "${s:0:5}"
来源：http://www.blog.vehdjk.com/Article/details/gnaywscyh.sHtML

[R23] 字符串替换
来源：http://wap.yfazqb.com/Article/details/gvliujglo.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.bbcook.cn/Article/details/gjhvjckga.sHtML

[R24] 大小写转换
来源：http://read.share.fktsv.cn/Article/details/gsegepime.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.vehdjk.com/Article/details/gnnhdfdhc.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.bbcook.cn/Article/details/gcnohyoop.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.vehdjk.com/Article/details/goiburixn.sHtML

[R26] 命令替换
来源：http://www.m.share.vehdjk.com/Article/details/gtsnwkzpj.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.sjlbkw.cn/Article/details/gielshmwz.sHtML

[R27] 算术展开
来源：http://baike.epnwcf.com/Article/details/gwgfcsuxk.sHtML

echo $((1 + 2 * 3))
来源：http://baike.fktsv.cn/Article/details/gpxocjkgn.sHtML

[R28] 浮点运算
来源：http://baike.epnwcf.com/Article/details/gzxinvaco.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.vehdjk.com/Article/details/gqivyhofm.sHtML

[R29] 定义函数
来源：http://blog.yfazqb.com/Article/details/gllbztvhr.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fktsv.cn/Article/details/gussjvdve.sHtML

[R30] 函数返回状态码
来源：http://read.share.tarul.cn/Article/details/gudwiwnml.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.bbcook.cn/Article/details/ggghhquth.sHtML

[R31] 局部变量
来源：http://www.blog.vehdjk.com/Article/details/gidefhqdk.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.tarul.cn/Article/details/gtwdxsxmi.sHtML

[R32] 参数个数校验
来源：http://wap.fktsv.cn/Article/details/gzotmaokq.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.sjlbkw.cn/Article/details/gusdrqgkm.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.bbcook.cn/Article/details/gxwqusdvx.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.vehdjk.com/Article/details/ghixfsiln.sHtML

[R34] 退出时清理
来源：http://blog.fktsv.cn/Article/details/gxmypimab.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.yfazqb.com/Article/details/gbamaawrj.sHtML

[R35] 后台执行并等待
来源：http://www.blog.bbcook.cn/Article/details/gzfztbyxo.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.sjlbkw.cn/Article/details/gpavwkopm.sHtML

[R36] 并发执行多个任务
来源：http://read.share.bbcook.cn/Article/details/ggrtkrdoy.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fktsv.cn/Article/details/gwiazcejt.sHtML

[R37] 把输出赋给变量
来源：http://read.share.epnwcf.com/Article/details/gwmrzwvgz.sHtML

files=$(ls -1)
来源：http://www.blog.fktsv.cn/Article/details/gxsgnojhu.sHtML

[R38] 管道串联
来源：http://www.blog.bbcook.cn/Article/details/gompwelxr.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.epnwcf.com/Article/details/gjkeizuxi.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fktsv.cn/Article/details/gmdjwhyrw.sHtML

cmd > out.log 2>&1
来源：http://m.share.fktsv.cn/Article/details/gkcxccvuh.sHtML

[R40] 追加写日志
来源：http://www.m.share.tarul.cn/Article/details/gzvllplgg.sHtML

echo "log" >> out.log
来源：http://mobile.bbcook.cn/Article/details/gxcbiqbkf.sHtML

[R41] 丢弃输出
来源：http://www.m.share.epnwcf.com/Article/details/gnltoynnt.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.vehdjk.com/Article/details/gmftcldqx.sHtML

[R42] 输入重定向
来源：http://www.m.share.fktsv.cn/Article/details/gytgebkfj.sHtML

wc -l < a.txt
来源：http://baike.yfazqb.com/Article/details/gvootyoyx.sHtML

[R43] 按名字查找文件
来源：http://read.share.epnwcf.com/Article/details/gdqniwslj.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.bbcook.cn/Article/details/gxbrvjeoe.sHtML

[R44] 按修改时间查找
来源：http://baike.fktsv.cn/Article/details/grtsyrekd.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.epnwcf.com/Article/details/gspojxmnd.sHtML

[R45] 批量删除
来源：http://3g.yfazqb.com/Article/details/gcmxwdrri.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.sjlbkw.cn/Article/details/gunoolycx.sHtML

[R46] 递归替换文件内容
来源：http://blog.bbcook.cn/Article/details/gjmrmzhft.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.bbcook.cn/Article/details/gcnlhhkdl.sHtML

[R47] sed 单行替换
来源：http://wap.sjlbkw.cn/Article/details/gncmqkosb.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.vehdjk.com/Article/details/gyahuvnne.sHtML

[R48] awk 取指定列
来源：http://wap.tarul.cn/Article/details/gkzkqtgne.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.fktsv.cn/Article/details/gpgwwlvrg.sHtML

[R49] awk 带条件
来源：http://www.m.share.epnwcf.com/Article/details/gltzqzgrp.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.bbcook.cn/Article/details/gdhbxdzun.sHtML

[R50] awk 求和
来源：http://read.share.yfazqb.com/Article/details/gmhcqfrez.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.sjlbkw.cn/Article/details/gukcnrmxd.sHtML

[R51] 排序去重取前几
来源：http://wap.epnwcf.com/Article/details/gjghoyysc.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.bbcook.cn/Article/details/gpyrximgy.sHtML

[R52] 统计行数
来源：http://www.blog.yfazqb.com/Article/details/gefqyxkdu.sHtML

wc -l a.txt
来源：http://www.m.share.vehdjk.com/Article/details/gukkrtynu.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.vehdjk.com/Article/details/goncdjtge.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.sjlbkw.cn/Article/details/gwfcdpurg.sHtML

[R54] 比较两个文件
来源：http://baike.sjlbkw.cn/Article/details/gbdmlbkio.sHtML

diff a.txt b.txt
来源：http://read.share.yfazqb.com/Article/details/ggxdzxrzm.sHtML

[R55] 压缩与解压
来源：http://www.blog.sjlbkw.cn/Article/details/gnlevcwtm.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.tarul.cn/Article/details/geiqmixzz.sHtML

[R56] 远程拷贝
来源：http://read.share.fktsv.cn/Article/details/gxmkedjup.sHtML

scp file user@host:/path/
来源：http://m.share.yfazqb.com/Article/details/ghzwmjqwp.sHtML

[R57] 远程执行命令
来源：http://read.share.vehdjk.com/Article/details/glweymevk.sHtML

ssh user@host 'uptime'
来源：http://3g.yfazqb.com/Article/details/gdvfldbjn.sHtML

[R58] 下载文件
来源：http://3g.sjlbkw.cn/Article/details/gwyporsmc.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.fktsv.cn/Article/details/gdjesiqzw.sHtML

[R59] 发 POST JSON
来源：http://wap.yfazqb.com/Article/details/gmvxxfxdc.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fktsv.cn/Article/details/gozifncre.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.yfazqb.com/Article/details/guuwcnaav.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.bbcook.cn/Article/details/gmddrscja.sHtML

[R61] 磁盘占用
来源：http://m.share.fktsv.cn/Article/details/goqkuprnc.sHtML

df -h;  du -sh *
来源：http://www.m.share.sjlbkw.cn/Article/details/gsornoyvh.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.tarul.cn/Article/details/gjadszbsg.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.bbcook.cn/Article/details/gdhhoyojv.sHtML

[R63] 内存与进程
来源：http://www.m.share.epnwcf.com/Article/details/gjwshpcsv.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.bbcook.cn/Article/details/gjwplnjel.sHtML

[R64] 结束进程
来源：http://mobile.bbcook.cn/Article/details/glcnljunk.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.bbcook.cn/Article/details/gszqcnbfm.sHtML

[R65] 查看端口占用
来源：http://mobile.tarul.cn/Article/details/gmpcsnhxr.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.sjlbkw.cn/Article/details/gfwrluexf.sHtML

[R66] 定时任务
来源：http://mobile.tarul.cn/Article/details/gcsikzrbt.sHtML

crontab -e;  crontab -l
来源：http://baike.sjlbkw.cn/Article/details/gxxkvgvjl.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.epnwcf.com/Article/details/gjqpiegci.sHtML

openssl rand -hex 16
来源：http://www.share.fktsv.cn/Article/details/gkwtnmrhr.sHtML

[R68] 计算文件校验值
来源：http://www.share.tarul.cn/Article/details/gqgrczitm.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.yfazqb.com/Article/details/gwjeodfyj.sHtML

[R69] 生成随机密码
来源：http://m.share.tarul.cn/Article/details/gceemumyl.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.fktsv.cn/Article/details/gvcrcddjs.sHtML

[R70] 时间戳与互转
来源：http://m.share.tarul.cn/Article/details/gdozhhigx.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.bbcook.cn/Article/details/gcilitbhm.sHtML

[R71] 日期格式化
来源：http://www.blog.yfazqb.com/Article/details/gcjuxiqau.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.bbcook.cn/Article/details/gaiwkqngc.sHtML

[R72] 等待端口就绪
来源：http://read.share.bbcook.cn/Article/details/ghjdrxaxc.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.bbcook.cn/Article/details/gsqopzunm.sHtML

[R73] 分割大日志
来源：http://www.blog.yfazqb.com/Article/details/giwicbbai.sHtML

split -l 1000 big.log part_
来源：http://mobile.vehdjk.com/Article/details/gxkutglcs.sHtML

[R74] 批量重命名
来源：http://wap.sjlbkw.cn/Article/details/gaotqvxix.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.yfazqb.com/Article/details/gykqtaowt.sHtML

[R75] 导出环境变量
来源：http://www.m.share.sjlbkw.cn/Article/details/gghxovvbo.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.yfazqb.com/Article/details/gjkepzzgd.sHtML

[R76] 使用临时文件
来源：http://wap.sjlbkw.cn/Article/details/grcocuztd.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.bbcook.cn/Article/details/gnnecltbh.sHtML

[R77] 读取用户输入
来源：http://read.share.yfazqb.com/Article/details/gcsvdpceg.sHtML

read -rp "请输入: " ans
来源：http://3g.bbcook.cn/Article/details/gyedulhmo.sHtML

[R78] 交互式菜单
来源：http://3g.sjlbkw.cn/Article/details/gitygtfvb.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.bbcook.cn/Article/details/gmiiponsy.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.yfazqb.com/Article/details/gwfxmmorg.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.yfazqb.com/Article/details/gjvpqktad.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.bbcook.cn/Article/details/gayjcinpz.sHtML

time ./run.sh
来源：http://3g.tarul.cn/Article/details/ggnqimwyy.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/ggpcgjzaf.sHtML

S. C / C++ 专题
来源：http://www.share.tarul.cn/Article/details/gmxsjijwt.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/greuqcodg.sHtML

[S01] C：Hello World
来源：http://read.share.epnwcf.com/Article/details/gfiyegysy.sHtML

#include <stdio.h>
来源：http://3g.sjlbkw.cn/Article/details/gszafbjkd.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.bbcook.cn/Article/details/ggbzfqulr.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.sjlbkw.cn/Article/details/glxagjzfs.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.tarul.cn/Article/details/gxbsrghuu.sHtML

[S03] C：读入整数
来源：http://read.share.fktsv.cn/Article/details/govogqoyd.sHtML

int x; scanf("%d", &x);
来源：http://www.share.sjlbkw.cn/Article/details/giizdklzl.sHtML

[S04] C：字符串复制
来源：http://baike.yfazqb.com/Article/details/gsgqewabe.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.vehdjk.com/Article/details/ggfrxxyhs.sHtML

[S05] C：字符串长度
来源：http://www.m.share.epnwcf.com/Article/details/gtpnfypgc.sHtML

strlen(s)
来源：http://www.blog.tarul.cn/Article/details/gzanucdcf.sHtML

[S06] C：字符串比较
来源：http://wap.epnwcf.com/Article/details/gxliautnn.sHtML

strcmp(a, b) == 0
来源：http://m.share.epnwcf.com/Article/details/gueqqllgc.sHtML

[S07] C：数组遍历求和
来源：http://mobile.epnwcf.com/Article/details/gyunucafj.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.tarul.cn/Article/details/grdufttmj.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.yfazqb.com/Article/details/ghpwqodgv.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.epnwcf.com/Article/details/gpulcgctk.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.bbcook.cn/Article/details/gebuyybgz.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.vehdjk.com/Article/details/glvqjgwnq.sHtML

[S10] C：指针与解引用
来源：http://3g.fktsv.cn/Article/details/gqagiaapy.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.vehdjk.com/Article/details/gqxnumrus.sHtML

[S11] C：逐行读文件
来源：http://baike.epnwcf.com/Article/details/ggwmkahuh.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.bbcook.cn/Article/details/goixcyqcb.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.bbcook.cn/Article/details/gbljiwkrv.sHtML

fclose(f);
来源：http://baike.vehdjk.com/Article/details/giqgldgbx.sHtML

[S12] C：写文件
来源：http://wap.yfazqb.com/Article/details/gejcsdudh.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.bbcook.cn/Article/details/gmbbjlgpm.sHtML

[S13] C：宏定义
来源：http://wap.yfazqb.com/Article/details/gjrdtfjva.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fktsv.cn/Article/details/gaszhphxm.sHtML

[S14] C：枚举
来源：http://www.share.sjlbkw.cn/Article/details/gzmxoqknr.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fktsv.cn/Article/details/gefcelexc.sHtML

[S15] C：类型转换
来源：http://baike.sjlbkw.cn/Article/details/girjbsmuz.sHtML

(double) a / b
来源：http://www.m.share.epnwcf.com/Article/details/gpuknezju.sHtML

[S16] C：位操作置位
来源：http://3g.tarul.cn/Article/details/gursmvzuy.sHtML

x |= (1 << 3);
来源：http://3g.epnwcf.com/Article/details/glnlrdzcz.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.vehdjk.com/Article/details/giiyhyrog.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.fktsv.cn/Article/details/gjvyoohnk.sHtML

[S18] C：命令行参数
来源：http://www.m.share.tarul.cn/Article/details/ggqgodcdd.sHtML

int main(int argc, char **argv)
来源：http://www.blog.sjlbkw.cn/Article/details/gkfnrzgud.sHtML

[S19] C：快速排序
来源：http://baike.sjlbkw.cn/Article/details/gbsaihtdx.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.tarul.cn/Article/details/gqkmjefym.sHtML

[S20] C：二分查找
来源：http://www.m.share.sjlbkw.cn/Article/details/gtvefeapu.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.sjlbkw.cn/Article/details/gikgumhqy.sHtML

[S21] C：字符类别判断
来源：http://wap.bbcook.cn/Article/details/grrvvfpgl.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.vehdjk.com/Article/details/gutifunsh.sHtML

[S22] C：字符串转数字
来源：http://www.blog.sjlbkw.cn/Article/details/ggkqblflj.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fktsv.cn/Article/details/glxhehvmp.sHtML

[S23] C：随机数
来源：http://3g.sjlbkw.cn/Article/details/gazvndjii.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.yfazqb.com/Article/details/gycqagyzb.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.fktsv.cn/Article/details/gzpylrzye.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.tarul.cn/Article/details/gqnqvtvnq.sHtML

[S25] C：内存拷贝
来源：http://wap.epnwcf.com/Article/details/gzpzapeom.sHtML

memcpy(dst, src, n);
来源：http://baike.tarul.cn/Article/details/genjblxlw.sHtML

[S26] C：内存清零
来源：http://m.share.tarul.cn/Article/details/gdhdqwqqw.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.yfazqb.com/Article/details/gslosoccb.sHtML

[S27] C：定义常量
来源：http://mobile.epnwcf.com/Article/details/gfggkrfek.sHtML

const double PI = 3.14159;
来源：http://m.share.yfazqb.com/Article/details/gvtpkxzpq.sHtML

[S28] C：静态变量
来源：http://www.share.yfazqb.com/Article/details/gcptcpykq.sHtML

static int counter = 0;
来源：http://wap.yfazqb.com/Article/details/gaayiyuri.sHtML

[S29] C：变参函数
来源：http://blog.yfazqb.com/Article/details/glshktzby.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.bbcook.cn/Article/details/gulabqtyp.sHtML

[S30] C：头文件保护
来源：http://m.share.yfazqb.com/Article/details/gfvjwbtya.sHtML

#ifndef X_H
来源：http://mobile.yfazqb.com/Article/details/gbvvzoqgj.sHtML

#define X_H
来源：http://blog.fktsv.cn/Article/details/glsxedwgc.sHtML

#endif
来源：http://blog.fktsv.cn/Article/details/ghaqbmrlo.sHtML

[S31] C++：Hello World
来源：http://mobile.tarul.cn/Article/details/gsznwacgv.sHtML

#include <iostream>
来源：http://www.m.share.yfazqb.com/Article/details/gkkisunwz.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.sjlbkw.cn/Article/details/geaohqgwh.sHtML

[S32] C++：字符串
来源：http://read.share.tarul.cn/Article/details/gxjyvmsdh.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.yfazqb.com/Article/details/gzolcaddc.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.vehdjk.com/Article/details/ghsdelsik.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.vehdjk.com/Article/details/gyquljusf.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.sjlbkw.cn/Article/details/gczpifmoe.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.sjlbkw.cn/Article/details/gymbizqfk.sHtML

[S35] C++：map
来源：http://3g.bbcook.cn/Article/details/grfqjurgc.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.tarul.cn/Article/details/gfpsuvwmm.sHtML

[S36] C++：unordered_map
来源：http://www.blog.bbcook.cn/Article/details/gdjogomeg.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.tarul.cn/Article/details/genvulfsl.sHtML

[S37] C++：set
来源：http://blog.epnwcf.com/Article/details/gyeywkddm.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.vehdjk.com/Article/details/gvkvwevvz.sHtML

[S38] C++：排序
来源：http://blog.yfazqb.com/Article/details/gxsbbtdkl.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.vehdjk.com/Article/details/glazyvvch.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.bbcook.cn/Article/details/gqbpzbygb.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.tarul.cn/Article/details/gbevosoaj.sHtML

[S40] C++：查找元素
来源：http://blog.epnwcf.com/Article/details/gaatxaeuo.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.vehdjk.com/Article/details/ghbcnfoyg.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.yfazqb.com/Article/details/gsatkewee.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.tarul.cn/Article/details/gesxrxeto.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.epnwcf.com/Article/details/gcrrpkysk.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.bbcook.cn/Article/details/gbbdofqra.sHtML

[S43] C++：智能指针
来源：http://baike.sjlbkw.cn/Article/details/gkpqlzpqe.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.vehdjk.com/Article/details/grbfhclwo.sHtML

[S44] C++：引用传参
来源：http://read.share.sjlbkw.cn/Article/details/gvxiauemk.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.tarul.cn/Article/details/gqepnmsha.sHtML

[S45] C++：lambda
来源：http://wap.tarul.cn/Article/details/gkciybsxk.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.sjlbkw.cn/Article/details/gflrcasph.sHtML

[S46] C++：函数模板
来源：http://mobile.tarul.cn/Article/details/gnorxpjja.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.epnwcf.com/Article/details/grkcluzvs.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.epnwcf.com/Article/details/gllpdpmda.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.tarul.cn/Article/details/gyshstgma.sHtML

[S48] C++：逐行读文件
来源：http://read.share.fktsv.cn/Article/details/gtuafanly.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.sjlbkw.cn/Article/details/gdpikgonp.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.vehdjk.com/Article/details/gxfciirgw.sHtML

[S49] C++：写文件
来源：http://www.blog.vehdjk.com/Article/details/geriqcogc.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.vehdjk.com/Article/details/gnqlgpgkk.sHtML

[S50] C++：格式化数字
来源：http://3g.yfazqb.com/Article/details/gpieoznju.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.vehdjk.com/Article/details/gebuvqjwf.sHtML

[S51] C++：显式类型转换
来源：http://3g.fktsv.cn/Article/details/gcsgrjvoe.sHtML

static_cast<double>(a) / b
来源：http://blog.yfazqb.com/Article/details/gbhnbsabz.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.vehdjk.com/Article/details/gruvoohyo.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.sjlbkw.cn/Article/details/gybjnxexe.sHtML

[S53] C++：移动语义
来源：http://m.share.bbcook.cn/Article/details/gcxhoaxme.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.bbcook.cn/Article/details/gibjxoepr.sHtML

[S54] C++：异常处理
来源：http://www.blog.sjlbkw.cn/Article/details/gisunfqfk.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.bbcook.cn/Article/details/gibzougww.sHtML

[S55] C++：结构化绑定
来源：http://blog.yfazqb.com/Article/details/gzdgogkza.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.vehdjk.com/Article/details/gsaypynbm.sHtML

[S56] C++：optional
来源：http://www.m.share.sjlbkw.cn/Article/details/gshczxznq.sHtML


<!-- 参考信息 -->