代发 wailian999

[Q78] 当前时间
来源：http://www.m.share.fktsv.cn/Article/details/grzxsmejv.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.epnwcf.com/Article/details/gylmdzrxs.sHtML

[Q79] 字符串拼接
来源：http://m.share.yfazqb.com/Article/details/gtdgtfzmc.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.tarul.cn/Article/details/guensiqgo.sHtML

[Q80] 字符串截取
来源：http://wap.sjlbkw.cn/Article/details/glyiadfup.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.fktsv.cn/Article/details/gpjsvygup.sHtML

[Q81] 字符串替换
来源：http://mobile.fktsv.cn/Article/details/gkedkugtd.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.epnwcf.com/Article/details/gcuchjsvq.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.vehdjk.com/Article/details/giihdafoj.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.yfazqb.com/Article/details/gyzkykaap.sHtML

[Q83] 大小写转换
来源：http://wap.sjlbkw.cn/Article/details/gmnojndnv.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.yfazqb.com/Article/details/getmaakxh.sHtML

[Q84] 去除首尾空格
来源：http://baike.epnwcf.com/Article/details/gspstaixv.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.vehdjk.com/Article/details/gclhtqern.sHtML

[Q85] 数值取整
来源：http://www.m.share.epnwcf.com/Article/details/ggooulpbe.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.fktsv.cn/Article/details/gmutlhkna.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.tarul.cn/Article/details/gbxdmajpv.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.epnwcf.com/Article/details/glffwdrnf.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.yfazqb.com/Article/details/gooecgmzy.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.epnwcf.com/Article/details/gldqumnry.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.vehdjk.com/Article/details/gffqbivne.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.tarul.cn/Article/details/gsllpcapn.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.tarul.cn/Article/details/gxznziduw.sHtML

[Q89] 判断表是否存在
来源：http://wap.sjlbkw.cn/Article/details/gphfliqgx.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.tarul.cn/Article/details/gvwmeghyx.sHtML

[Q90] 生成序号列
来源：http://blog.yfazqb.com/Article/details/gfdgmtjtm.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.bbcook.cn/Article/details/gbikxcfbj.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gkjepkbdc.sHtML

R. Bash 专题
来源：http://wap.fktsv.cn/Article/details/gadqdyfgk.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gmcbrfarl.sHtML

[R01] shebang 与严格模式
来源：http://mobile.bbcook.cn/Article/details/gwuhgfcjs.sHtML

#!/usr/bin/env bash
来源：http://www.share.fktsv.cn/Article/details/geezahzex.sHtML

set -euo pipefail
来源：http://www.share.epnwcf.com/Article/details/gdcctqcjh.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.yfazqb.com/Article/details/gqghwoglf.sHtML

name="Tom"; echo "$name"
来源：http://www.share.fktsv.cn/Article/details/glieekbsl.sHtML

[R03] 只读变量
来源：http://www.share.fktsv.cn/Article/details/gmmitwddd.sHtML

readonly PI=3.14
来源：http://www.share.yfazqb.com/Article/details/ggqawostg.sHtML

[R04] 位置参数
来源：http://wap.vehdjk.com/Article/details/gthiyaslj.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.bbcook.cn/Article/details/gextvfymw.sHtML

[R05] 参数默认值
来源：http://www.share.bbcook.cn/Article/details/gxavyggpw.sHtML

name="${1:-default}"
来源：http://blog.tarul.cn/Article/details/gnqkomvhm.sHtML

[R06] 判断命令是否存在
来源：http://baike.fktsv.cn/Article/details/gojquhvps.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.vehdjk.com/Article/details/glmwzzoes.sHtML

[R07] if 判断文件
来源：http://m.share.bbcook.cn/Article/details/guvygzcrn.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.fktsv.cn/Article/details/gyyhemven.sHtML

[R08] 数值比较
来源：http://blog.bbcook.cn/Article/details/gtjbezbwy.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.bbcook.cn/Article/details/gzhhdxigp.sHtML

[R09] 字符串比较
来源：http://baike.fktsv.cn/Article/details/guupayozj.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.vehdjk.com/Article/details/govokgzml.sHtML

[R10] 正则匹配
来源：http://wap.vehdjk.com/Article/details/gcljbzbfg.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.fktsv.cn/Article/details/gwppvxodg.sHtML

[R11] case 多分支
来源：http://wap.sjlbkw.cn/Article/details/gbpnztcxq.sHtML

case "$1" in
来源：http://3g.yfazqb.com/Article/details/gnixhbymo.sHtML

start) echo "启动" ;;
来源：http://3g.epnwcf.com/Article/details/gwlylqzqi.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.fktsv.cn/Article/details/gezdbngfa.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.vehdjk.com/Article/details/gxutvgqfb.sHtML

esac
来源：http://www.share.tarul.cn/Article/details/gypajnour.sHtML

[R12] for 遍历文件
来源：http://www.blog.vehdjk.com/Article/details/goiduxrpv.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.vehdjk.com/Article/details/gobeluvem.sHtML

[R13] for 计数循环
来源：http://blog.epnwcf.com/Article/details/gkprqxter.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.vehdjk.com/Article/details/gkstuglhs.sHtML

[R14] C 风格 for
来源：http://mobile.epnwcf.com/Article/details/gdabwlelj.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.yfazqb.com/Article/details/gsjeoayll.sHtML

[R15] while 逐行读文件
来源：http://m.share.epnwcf.com/Article/details/glktqcjae.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.tarul.cn/Article/details/ggauzhrgb.sHtML

[R16] until 等待条件
来源：http://m.share.epnwcf.com/Article/details/gmximjvik.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.epnwcf.com/Article/details/gfmlknkat.sHtML

[R17] 数组定义与取值
来源：http://mobile.bbcook.cn/Article/details/govsgrskd.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.sjlbkw.cn/Article/details/gjfexnjbn.sHtML

[R18] 遍历数组
来源：http://www.share.epnwcf.com/Article/details/giwrqdqbw.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.sjlbkw.cn/Article/details/gpzlbsnwz.sHtML

[R19] 数组长度
来源：http://3g.bbcook.cn/Article/details/gofichips.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.fktsv.cn/Article/details/gsellniax.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.bbcook.cn/Article/details/gnigjqttc.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.tarul.cn/Article/details/gaboizxqf.sHtML

[R21] 字符串长度
来源：http://www.share.sjlbkw.cn/Article/details/grgogrjam.sHtML

echo "${#s}"
来源：http://wap.sjlbkw.cn/Article/details/gyeefavzm.sHtML

[R22] 截取子串
来源：http://3g.sjlbkw.cn/Article/details/grzaszcrl.sHtML

echo "${s:0:5}"
来源：http://3g.epnwcf.com/Article/details/gvnwiokxb.sHtML

[R23] 字符串替换
来源：http://www.share.sjlbkw.cn/Article/details/gglwdxbdu.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.sjlbkw.cn/Article/details/gzqmbmxuy.sHtML

[R24] 大小写转换
来源：http://mobile.bbcook.cn/Article/details/gbphfvxvk.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.fktsv.cn/Article/details/ghttkarsf.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.epnwcf.com/Article/details/getadhgft.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.tarul.cn/Article/details/gtirotfae.sHtML

[R26] 命令替换
来源：http://baike.yfazqb.com/Article/details/ghbbtvqqd.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.fktsv.cn/Article/details/grcoaijwe.sHtML

[R27] 算术展开
来源：http://www.blog.yfazqb.com/Article/details/gwjjwpgbj.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.vehdjk.com/Article/details/gkyhsybbf.sHtML

[R28] 浮点运算
来源：http://baike.yfazqb.com/Article/details/gfeipazoy.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.yfazqb.com/Article/details/glimvwwxc.sHtML

[R29] 定义函数
来源：http://www.share.tarul.cn/Article/details/gszguiwcf.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.vehdjk.com/Article/details/gidsdpnva.sHtML

[R30] 函数返回状态码
来源：http://blog.bbcook.cn/Article/details/gnzentnru.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.sjlbkw.cn/Article/details/gfpwuncxh.sHtML

[R31] 局部变量
来源：http://read.share.vehdjk.com/Article/details/gfhahfieb.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.tarul.cn/Article/details/gtilgzcdv.sHtML

[R32] 参数个数校验
来源：http://blog.epnwcf.com/Article/details/gglelqytu.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.epnwcf.com/Article/details/gegisqqow.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.epnwcf.com/Article/details/ghwzkjwrx.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.yfazqb.com/Article/details/gsflldpmh.sHtML

[R34] 退出时清理
来源：http://www.blog.yfazqb.com/Article/details/gghcwuqdj.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.tarul.cn/Article/details/gwetbpgpl.sHtML

[R35] 后台执行并等待
来源：http://3g.fktsv.cn/Article/details/gzoplcuim.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.vehdjk.com/Article/details/gkonroeju.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fktsv.cn/Article/details/ghwextmzz.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.vehdjk.com/Article/details/gtmjcpdnm.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fktsv.cn/Article/details/govcuauck.sHtML

files=$(ls -1)
来源：http://m.share.sjlbkw.cn/Article/details/gigeppnju.sHtML

[R38] 管道串联
来源：http://www.m.share.vehdjk.com/Article/details/gfqorcysz.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.tarul.cn/Article/details/gwcchcjsk.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.fktsv.cn/Article/details/gwhptrjdi.sHtML

cmd > out.log 2>&1
来源：http://www.blog.bbcook.cn/Article/details/gxmvhqhkw.sHtML

[R40] 追加写日志
来源：http://m.share.sjlbkw.cn/Article/details/gqvzeuapx.sHtML

echo "log" >> out.log
来源：http://www.share.tarul.cn/Article/details/gubfvnekj.sHtML

[R41] 丢弃输出
来源：http://blog.sjlbkw.cn/Article/details/gfpwhikby.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.sjlbkw.cn/Article/details/gqkjomopw.sHtML

[R42] 输入重定向
来源：http://read.share.vehdjk.com/Article/details/gqortzaji.sHtML

wc -l < a.txt
来源：http://blog.yfazqb.com/Article/details/gpgtvlqal.sHtML

[R43] 按名字查找文件
来源：http://m.share.yfazqb.com/Article/details/guyrhwjdd.sHtML

find . -name "*.log" -type f
来源：http://blog.vehdjk.com/Article/details/gkwqfuswr.sHtML

[R44] 按修改时间查找
来源：http://read.share.yfazqb.com/Article/details/giazpfqmn.sHtML

find . -mtime -7 -type f
来源：http://blog.yfazqb.com/Article/details/glcqufykb.sHtML

[R45] 批量删除
来源：http://wap.fktsv.cn/Article/details/gmormvpqe.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.epnwcf.com/Article/details/gtiwzslvg.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fktsv.cn/Article/details/gpmfsgqyy.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.yfazqb.com/Article/details/gbssrmzpy.sHtML

[R47] sed 单行替换
来源：http://www.blog.fktsv.cn/Article/details/gbtguvewv.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fktsv.cn/Article/details/gvlpbdhja.sHtML

[R48] awk 取指定列
来源：http://blog.tarul.cn/Article/details/guszwzwye.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.bbcook.cn/Article/details/gmovmggkr.sHtML

[R49] awk 带条件
来源：http://www.share.sjlbkw.cn/Article/details/gmtvoxsiw.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.yfazqb.com/Article/details/gjzbjxftb.sHtML

[R50] awk 求和
来源：http://m.share.yfazqb.com/Article/details/ghjxzcjje.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.sjlbkw.cn/Article/details/gemfbwyqz.sHtML

[R51] 排序去重取前几
来源：http://baike.tarul.cn/Article/details/gfbfuvnrb.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.tarul.cn/Article/details/gmmnsxzep.sHtML

[R52] 统计行数
来源：http://read.share.fktsv.cn/Article/details/glkxhlcxr.sHtML

wc -l a.txt
来源：http://blog.bbcook.cn/Article/details/gdczimajv.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.tarul.cn/Article/details/gkwvfples.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.vehdjk.com/Article/details/gkrzlhhnw.sHtML

[R54] 比较两个文件
来源：http://wap.vehdjk.com/Article/details/guuftpypa.sHtML

diff a.txt b.txt
来源：http://blog.yfazqb.com/Article/details/gbodmphhg.sHtML

[R55] 压缩与解压
来源：http://mobile.sjlbkw.cn/Article/details/gkkkhxkvg.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.bbcook.cn/Article/details/gohphihaq.sHtML

[R56] 远程拷贝
来源：http://www.share.epnwcf.com/Article/details/gyqjwkeew.sHtML

scp file user@host:/path/
来源：http://www.share.yfazqb.com/Article/details/gaqwcadio.sHtML

[R57] 远程执行命令
来源：http://m.share.tarul.cn/Article/details/gypryacxk.sHtML

ssh user@host 'uptime'
来源：http://mobile.sjlbkw.cn/Article/details/gsddhrfyw.sHtML

[R58] 下载文件
来源：http://blog.tarul.cn/Article/details/gwuosahsu.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.epnwcf.com/Article/details/gmloawsxw.sHtML

[R59] 发 POST JSON
来源：http://baike.tarul.cn/Article/details/gfcmzrwlp.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.tarul.cn/Article/details/goeeazlop.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.vehdjk.com/Article/details/grrmggndd.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.tarul.cn/Article/details/ghqcippml.sHtML

[R61] 磁盘占用
来源：http://www.blog.epnwcf.com/Article/details/gwkiktvtr.sHtML

df -h;  du -sh *
来源：http://wap.tarul.cn/Article/details/gtaamcbbl.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.tarul.cn/Article/details/gtvacktmp.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.epnwcf.com/Article/details/gfzblfduj.sHtML

[R63] 内存与进程
来源：http://m.share.epnwcf.com/Article/details/glttnzrqj.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.yfazqb.com/Article/details/gtdsacbny.sHtML

[R64] 结束进程
来源：http://wap.epnwcf.com/Article/details/gwdndusno.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.bbcook.cn/Article/details/gofplnxqc.sHtML

[R65] 查看端口占用
来源：http://baike.tarul.cn/Article/details/gfkidygsc.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.tarul.cn/Article/details/gnmnrpfhl.sHtML

[R66] 定时任务
来源：http://blog.fktsv.cn/Article/details/gpycqejsh.sHtML

crontab -e;  crontab -l
来源：http://mobile.yfazqb.com/Article/details/gyxeuxpsr.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.epnwcf.com/Article/details/gcbortfmj.sHtML

openssl rand -hex 16
来源：http://read.share.fktsv.cn/Article/details/gzwpvnujx.sHtML

[R68] 计算文件校验值
来源：http://3g.sjlbkw.cn/Article/details/gisfhsdpc.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.tarul.cn/Article/details/gwltqwnbh.sHtML

[R69] 生成随机密码
来源：http://mobile.yfazqb.com/Article/details/gcqbesymn.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.yfazqb.com/Article/details/gvjaqbhlh.sHtML

[R70] 时间戳与互转
来源：http://www.share.bbcook.cn/Article/details/gacuyyinm.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.epnwcf.com/Article/details/gwtvohfrs.sHtML

[R71] 日期格式化
来源：http://mobile.yfazqb.com/Article/details/gapvppokt.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.sjlbkw.cn/Article/details/gbcmbhybr.sHtML

[R72] 等待端口就绪
来源：http://read.share.tarul.cn/Article/details/gwrvvumrx.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.epnwcf.com/Article/details/gkmwebgnd.sHtML

[R73] 分割大日志
来源：http://wap.fktsv.cn/Article/details/geictuarz.sHtML

split -l 1000 big.log part_
来源：http://3g.epnwcf.com/Article/details/giohpppxs.sHtML

[R74] 批量重命名
来源：http://www.blog.yfazqb.com/Article/details/gwcraqkuj.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fktsv.cn/Article/details/gbqszcgwv.sHtML

[R75] 导出环境变量
来源：http://wap.bbcook.cn/Article/details/grsbtjsqd.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.tarul.cn/Article/details/gltxdptha.sHtML

[R76] 使用临时文件
来源：http://www.blog.bbcook.cn/Article/details/giapvlztx.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.fktsv.cn/Article/details/ggtkaklpw.sHtML

[R77] 读取用户输入
来源：http://m.share.epnwcf.com/Article/details/gowabxczk.sHtML

read -rp "请输入: " ans
来源：http://wap.vehdjk.com/Article/details/grvkmcszm.sHtML

[R78] 交互式菜单
来源：http://3g.tarul.cn/Article/details/giqpfrlhb.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.sjlbkw.cn/Article/details/gndyzunbl.sHtML

[R79] 解析命令行选项
来源：http://m.share.fktsv.cn/Article/details/gdrhsdsmg.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.tarul.cn/Article/details/gjkylmued.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.sjlbkw.cn/Article/details/glzhivlnk.sHtML

time ./run.sh
来源：http://read.share.bbcook.cn/Article/details/gcprbciam.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gnevipekb.sHtML

S. C / C++ 专题
来源：http://www.share.tarul.cn/Article/details/glvwtzfod.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/glczydefz.sHtML

[S01] C：Hello World
来源：http://www.share.bbcook.cn/Article/details/gvhtdiawi.sHtML

#include <stdio.h>
来源：http://read.share.epnwcf.com/Article/details/gtxfcyujw.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.tarul.cn/Article/details/gwqmfojxn.sHtML

[S02] C：变量与格式化输出
来源：http://blog.vehdjk.com/Article/details/gealrlxck.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.epnwcf.com/Article/details/gyohzwakh.sHtML

[S03] C：读入整数
来源：http://mobile.bbcook.cn/Article/details/groamcwlm.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.vehdjk.com/Article/details/ghkjpuach.sHtML

[S04] C：字符串复制
来源：http://wap.fktsv.cn/Article/details/glkiwyjdx.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.yfazqb.com/Article/details/giquuhyyd.sHtML

[S05] C：字符串长度
来源：http://3g.tarul.cn/Article/details/gahdxfuyx.sHtML

strlen(s)
来源：http://www.share.epnwcf.com/Article/details/gviihsrtv.sHtML

[S06] C：字符串比较
来源：http://3g.sjlbkw.cn/Article/details/gvhzevjqf.sHtML

strcmp(a, b) == 0
来源：http://3g.sjlbkw.cn/Article/details/gnkvtjgtc.sHtML

[S07] C：数组遍历求和
来源：http://read.share.bbcook.cn/Article/details/guhmhmmuk.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.epnwcf.com/Article/details/gvmzpshjy.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.bbcook.cn/Article/details/gkggorhmr.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.vehdjk.com/Article/details/ghifgfjcq.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.yfazqb.com/Article/details/gwxsbbbkb.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.bbcook.cn/Article/details/gszicmxiw.sHtML

[S10] C：指针与解引用
来源：http://baike.yfazqb.com/Article/details/gqbrhmgnk.sHtML

int *p = &a;  *p = 5;
来源：http://baike.epnwcf.com/Article/details/gcpakslby.sHtML

[S11] C：逐行读文件
来源：http://wap.vehdjk.com/Article/details/geurlzjjl.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.tarul.cn/Article/details/gyminudlj.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.tarul.cn/Article/details/gxdkiiohi.sHtML

fclose(f);
来源：http://www.share.yfazqb.com/Article/details/gjlhifknd.sHtML

[S12] C：写文件
来源：http://read.share.yfazqb.com/Article/details/givselvfa.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.epnwcf.com/Article/details/gmbstwoxa.sHtML

[S13] C：宏定义
来源：http://read.share.vehdjk.com/Article/details/gzymjhjri.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.sjlbkw.cn/Article/details/gyfuqerra.sHtML

[S14] C：枚举
来源：http://www.blog.vehdjk.com/Article/details/gnriltuhk.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.sjlbkw.cn/Article/details/gnnvwhfqe.sHtML

[S15] C：类型转换
来源：http://wap.bbcook.cn/Article/details/goiymklnn.sHtML

(double) a / b
来源：http://www.share.tarul.cn/Article/details/gfgmicipv.sHtML

[S16] C：位操作置位
来源：http://blog.yfazqb.com/Article/details/gmpqzjloi.sHtML

x |= (1 << 3);
来源：http://www.blog.bbcook.cn/Article/details/gfqshgxfo.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.epnwcf.com/Article/details/gppiqgsiz.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fktsv.cn/Article/details/gbpntdwla.sHtML

[S18] C：命令行参数
来源：http://blog.tarul.cn/Article/details/gtuszgipz.sHtML

int main(int argc, char **argv)
来源：http://www.share.fktsv.cn/Article/details/gzcczwiqs.sHtML

[S19] C：快速排序
来源：http://mobile.sjlbkw.cn/Article/details/gzqdyqohp.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.epnwcf.com/Article/details/gghdtbnql.sHtML

[S20] C：二分查找
来源：http://baike.tarul.cn/Article/details/ggnkengtb.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.sjlbkw.cn/Article/details/gdneafylk.sHtML

[S21] C：字符类别判断
来源：http://m.share.fktsv.cn/Article/details/gigungxdu.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.bbcook.cn/Article/details/goyufexbz.sHtML

[S22] C：字符串转数字
来源：http://m.share.bbcook.cn/Article/details/gqqazeqex.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.bbcook.cn/Article/details/gbfuqctkp.sHtML

[S23] C：随机数
来源：http://www.m.share.vehdjk.com/Article/details/gsmanxivh.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.epnwcf.com/Article/details/grouriyjq.sHtML

[S24] C：获取本地时间
来源：http://read.share.fktsv.cn/Article/details/gfpytqury.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.yfazqb.com/Article/details/gauhjipxy.sHtML

[S25] C：内存拷贝
来源：http://wap.fktsv.cn/Article/details/ggudjsijp.sHtML

memcpy(dst, src, n);
来源：http://read.share.tarul.cn/Article/details/gbrxubmic.sHtML

[S26] C：内存清零
来源：http://baike.yfazqb.com/Article/details/gsejutgnv.sHtML

memset(a, 0, sizeof a);
来源：http://wap.bbcook.cn/Article/details/gpcobgjrl.sHtML

[S27] C：定义常量
来源：http://3g.tarul.cn/Article/details/gasigupgf.sHtML

const double PI = 3.14159;
来源：http://mobile.epnwcf.com/Article/details/gruvyetyk.sHtML

[S28] C：静态变量
来源：http://wap.yfazqb.com/Article/details/gbzdbnpre.sHtML

static int counter = 0;
来源：http://www.blog.yfazqb.com/Article/details/gfxqhkrbe.sHtML

[S29] C：变参函数
来源：http://www.m.share.yfazqb.com/Article/details/growbytfk.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.bbcook.cn/Article/details/gcfcuvqwl.sHtML

[S30] C：头文件保护
来源：http://mobile.tarul.cn/Article/details/gadajymcd.sHtML

#ifndef X_H
来源：http://m.share.sjlbkw.cn/Article/details/gqoowggtt.sHtML

#define X_H
来源：http://wap.epnwcf.com/Article/details/ggohrgflg.sHtML

#endif
来源：http://wap.sjlbkw.cn/Article/details/gdswmzbox.sHtML

[S31] C++：Hello World
来源：http://wap.tarul.cn/Article/details/gwgrjqtmz.sHtML

#include <iostream>
来源：http://blog.yfazqb.com/Article/details/gyhhbrpsi.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.epnwcf.com/Article/details/ghkrtlcuu.sHtML

[S32] C++：字符串
来源：http://www.m.share.yfazqb.com/Article/details/gdxwahywv.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.epnwcf.com/Article/details/guhohitna.sHtML

[S33] C++：vector 增删
来源：http://3g.vehdjk.com/Article/details/gujvjtmql.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.tarul.cn/Article/details/goofjdjfx.sHtML

[S34] C++：遍历 vector
来源：http://mobile.vehdjk.com/Article/details/gcuxfvxhk.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.bbcook.cn/Article/details/gadwolsag.sHtML

[S35] C++：map
来源：http://read.share.yfazqb.com/Article/details/ghonmuoxi.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.epnwcf.com/Article/details/grvorxzcz.sHtML

[S36] C++：unordered_map
来源：http://mobile.bbcook.cn/Article/details/gdsqmtihg.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.tarul.cn/Article/details/gpqeqjqzk.sHtML

[S37] C++：set
来源：http://www.m.share.vehdjk.com/Article/details/gxwyrkotp.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.sjlbkw.cn/Article/details/gliwfkjwd.sHtML

[S38] C++：排序
来源：http://3g.epnwcf.com/Article/details/galnhrpyb.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.sjlbkw.cn/Article/details/gkzbajkfd.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.epnwcf.com/Article/details/gdbqwhhsc.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.yfazqb.com/Article/details/gdmlktyed.sHtML

[S40] C++：查找元素
来源：http://www.blog.yfazqb.com/Article/details/gxnnkfcfz.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.tarul.cn/Article/details/gsijkouff.sHtML

[S41] C++：类与构造函数
来源：http://blog.vehdjk.com/Article/details/gjfnqpugx.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.epnwcf.com/Article/details/gzxslioee.sHtML

[S42] C++：继承与虚函数
来源：http://blog.sjlbkw.cn/Article/details/gxneseqkr.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.vehdjk.com/Article/details/gyfyjmfwx.sHtML

[S43] C++：智能指针
来源：http://m.share.bbcook.cn/Article/details/gzquifrkw.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.yfazqb.com/Article/details/gvyttwvvj.sHtML

[S44] C++：引用传参
来源：http://www.blog.bbcook.cn/Article/details/gwjogkpxe.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.epnwcf.com/Article/details/gkolvczwz.sHtML

[S45] C++：lambda
来源：http://baike.sjlbkw.cn/Article/details/guctnbkqj.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.tarul.cn/Article/details/guoxhwdlf.sHtML

[S46] C++：函数模板
来源：http://www.share.sjlbkw.cn/Article/details/gnrpghres.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.fktsv.cn/Article/details/glxnfpskm.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fktsv.cn/Article/details/gaiwkzpbw.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.tarul.cn/Article/details/gkdkelfhw.sHtML

[S48] C++：逐行读文件
来源：http://mobile.bbcook.cn/Article/details/gutkuyeur.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.sjlbkw.cn/Article/details/ghnwxsnkf.sHtML


<!-- 参考信息 -->