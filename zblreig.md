代发 wailian999

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.epnwcf.com/Article/details/gcyojeglv.sHtML

[Q75] 日期格式化
来源：http://blog.yfazqb.com/Article/details/gsemfewfb.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.tarul.cn/Article/details/gxtpdybkr.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.epnwcf.com/Article/details/ggccwmggz.sHtML

[Q76] 按天统计
来源：http://wap.sjlbkw.cn/Article/details/gagqimpot.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.sjlbkw.cn/Article/details/gwiobiino.sHtML

[Q77] 时间加减
来源：http://www.blog.tarul.cn/Article/details/gfedqcjon.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.yfazqb.com/Article/details/ghhckzthp.sHtML

[Q78] 当前时间
来源：http://www.m.share.fktsv.cn/Article/details/gwjgyxozr.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.bbcook.cn/Article/details/gguhwajdg.sHtML

[Q79] 字符串拼接
来源：http://3g.fktsv.cn/Article/details/giigswjky.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.tarul.cn/Article/details/gxrkasbpd.sHtML

[Q80] 字符串截取
来源：http://wap.tarul.cn/Article/details/gdjbatiih.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.tarul.cn/Article/details/ggmqqykrw.sHtML

[Q81] 字符串替换
来源：http://read.share.fktsv.cn/Article/details/ghtmvitih.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.vehdjk.com/Article/details/gdxbldhyd.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.fktsv.cn/Article/details/gvusavwbn.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/gmxqpdkhh.sHtML

[Q83] 大小写转换
来源：http://3g.epnwcf.com/Article/details/ghvizfron.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.epnwcf.com/Article/details/gbqceopnu.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.sjlbkw.cn/Article/details/gfzbqxlkw.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.vehdjk.com/Article/details/gjgafiwqu.sHtML

[Q85] 数值取整
来源：http://blog.epnwcf.com/Article/details/gpzlzkrku.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.sjlbkw.cn/Article/details/gvtluoikp.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.yfazqb.com/Article/details/gbkngqdbf.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.fktsv.cn/Article/details/guhbkdpgj.sHtML

[Q87] JSON 字段做条件
来源：http://blog.fktsv.cn/Article/details/gnlsovzkn.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.tarul.cn/Article/details/gyqjdnsew.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.yfazqb.com/Article/details/gbsvhxrct.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.sjlbkw.cn/Article/details/gsyqfwsjk.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.tarul.cn/Article/details/gcgrolwpg.sHtML

[Q89] 判断表是否存在
来源：http://3g.tarul.cn/Article/details/gyejezcbw.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.tarul.cn/Article/details/gtfoppwvv.sHtML

[Q90] 生成序号列
来源：http://baike.epnwcf.com/Article/details/gmahtonye.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.epnwcf.com/Article/details/gavtaepbi.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/ggfiybhon.sHtML

R. Bash 专题
来源：http://m.share.fktsv.cn/Article/details/gyotwipce.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gdegmntwd.sHtML

[R01] shebang 与严格模式
来源：http://www.share.yfazqb.com/Article/details/gxkieqypv.sHtML

#!/usr/bin/env bash
来源：http://baike.sjlbkw.cn/Article/details/gcwncnalu.sHtML

set -euo pipefail
来源：http://wap.fktsv.cn/Article/details/gupjnuxjz.sHtML

[R02] 变量赋值与使用
来源：http://mobile.bbcook.cn/Article/details/gmougsrvr.sHtML

name="Tom"; echo "$name"
来源：http://baike.bbcook.cn/Article/details/gftniggpp.sHtML

[R03] 只读变量
来源：http://www.m.share.tarul.cn/Article/details/gwiudcvpj.sHtML

readonly PI=3.14
来源：http://mobile.bbcook.cn/Article/details/glnaieeyu.sHtML

[R04] 位置参数
来源：http://mobile.yfazqb.com/Article/details/gagbgtkfb.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.tarul.cn/Article/details/gnufrjedq.sHtML

[R05] 参数默认值
来源：http://blog.sjlbkw.cn/Article/details/gbxiwxtvm.sHtML

name="${1:-default}"
来源：http://read.share.yfazqb.com/Article/details/gfdcdbdbq.sHtML

[R06] 判断命令是否存在
来源：http://blog.tarul.cn/Article/details/gqrnsjynk.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.epnwcf.com/Article/details/gsdafpezg.sHtML

[R07] if 判断文件
来源：http://mobile.vehdjk.com/Article/details/gxofbxcgp.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.bbcook.cn/Article/details/gwvxajvbq.sHtML

[R08] 数值比较
来源：http://read.share.tarul.cn/Article/details/gizcjyqhl.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fktsv.cn/Article/details/gkdpuywwl.sHtML

[R09] 字符串比较
来源：http://blog.epnwcf.com/Article/details/gyraqlkqf.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.epnwcf.com/Article/details/gypropyix.sHtML

[R10] 正则匹配
来源：http://www.blog.bbcook.cn/Article/details/gzamwfygj.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.tarul.cn/Article/details/gmhlvpmcw.sHtML

[R11] case 多分支
来源：http://www.blog.epnwcf.com/Article/details/gcyodoebf.sHtML

case "$1" in
来源：http://wap.yfazqb.com/Article/details/gxxegrzgo.sHtML

start) echo "启动" ;;
来源：http://read.share.yfazqb.com/Article/details/gbnjjzuor.sHtML

stop)  echo "停止" ;;
来源：http://baike.yfazqb.com/Article/details/gswmnslmt.sHtML

*)     echo "未知命令" ;;
来源：http://wap.fktsv.cn/Article/details/gobidqhsh.sHtML

esac
来源：http://3g.epnwcf.com/Article/details/gnzblsdnl.sHtML

[R12] for 遍历文件
来源：http://www.share.fktsv.cn/Article/details/gvylarswd.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.fktsv.cn/Article/details/gmznpfung.sHtML

[R13] for 计数循环
来源：http://baike.fktsv.cn/Article/details/giyttdeyz.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.vehdjk.com/Article/details/gdmgdplwo.sHtML

[R14] C 风格 for
来源：http://m.share.tarul.cn/Article/details/gzrgjiacg.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.tarul.cn/Article/details/gptacvjca.sHtML

[R15] while 逐行读文件
来源：http://3g.yfazqb.com/Article/details/grooxvnes.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.epnwcf.com/Article/details/gnnxgcuhp.sHtML

[R16] until 等待条件
来源：http://read.share.vehdjk.com/Article/details/ghgwbeysm.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.bbcook.cn/Article/details/gwmuddvyu.sHtML

[R17] 数组定义与取值
来源：http://mobile.bbcook.cn/Article/details/getdneksz.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.epnwcf.com/Article/details/gduxzvxjn.sHtML

[R18] 遍历数组
来源：http://baike.tarul.cn/Article/details/gkeesywsi.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.sjlbkw.cn/Article/details/gykbidrze.sHtML

[R19] 数组长度
来源：http://www.share.yfazqb.com/Article/details/ghbwuownj.sHtML

echo "${#arr[@]}"
来源：http://baike.fktsv.cn/Article/details/gipqnwflo.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.tarul.cn/Article/details/gzrscxpqk.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.tarul.cn/Article/details/gwrdybopr.sHtML

[R21] 字符串长度
来源：http://blog.epnwcf.com/Article/details/grhkzmoyd.sHtML

echo "${#s}"
来源：http://www.share.fktsv.cn/Article/details/gfcovmgaf.sHtML

[R22] 截取子串
来源：http://baike.fktsv.cn/Article/details/gnckfhrfj.sHtML

echo "${s:0:5}"
来源：http://www.blog.tarul.cn/Article/details/gzwddquan.sHtML

[R23] 字符串替换
来源：http://m.share.bbcook.cn/Article/details/gfwobwywx.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.vehdjk.com/Article/details/gjkbdriqm.sHtML

[R24] 大小写转换
来源：http://www.blog.sjlbkw.cn/Article/details/gszcmhrea.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.bbcook.cn/Article/details/gisvuqiof.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fktsv.cn/Article/details/ggcgcpxba.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.fktsv.cn/Article/details/glskfkrpz.sHtML

[R26] 命令替换
来源：http://m.share.bbcook.cn/Article/details/gomhvjmuu.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.vehdjk.com/Article/details/gclrwubyu.sHtML

[R27] 算术展开
来源：http://mobile.vehdjk.com/Article/details/ghbdsbrgt.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.vehdjk.com/Article/details/gmxxgdczl.sHtML

[R28] 浮点运算
来源：http://wap.tarul.cn/Article/details/gdcnnzztc.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fktsv.cn/Article/details/gxyhzvvwi.sHtML

[R29] 定义函数
来源：http://blog.yfazqb.com/Article/details/gtispycdy.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.tarul.cn/Article/details/gtxovgvvb.sHtML

[R30] 函数返回状态码
来源：http://wap.tarul.cn/Article/details/gmqmkwlro.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.yfazqb.com/Article/details/gcylazmum.sHtML

[R31] 局部变量
来源：http://mobile.tarul.cn/Article/details/gwcehejbh.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.bbcook.cn/Article/details/ghfkqhkbf.sHtML

[R32] 参数个数校验
来源：http://www.blog.sjlbkw.cn/Article/details/gexfmtcul.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.yfazqb.com/Article/details/gfqarbaoh.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.epnwcf.com/Article/details/gsexwuooi.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.epnwcf.com/Article/details/gysgdcmtx.sHtML

[R34] 退出时清理
来源：http://m.share.epnwcf.com/Article/details/gpxvmjole.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.fktsv.cn/Article/details/glkxtwmfg.sHtML

[R35] 后台执行并等待
来源：http://mobile.fktsv.cn/Article/details/gclubehvs.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.sjlbkw.cn/Article/details/gphgazimt.sHtML

[R36] 并发执行多个任务
来源：http://m.share.sjlbkw.cn/Article/details/glauxatik.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.bbcook.cn/Article/details/grwuyzrha.sHtML

[R37] 把输出赋给变量
来源：http://baike.tarul.cn/Article/details/gjjgcfslj.sHtML

files=$(ls -1)
来源：http://read.share.vehdjk.com/Article/details/gfcydtmbm.sHtML

[R38] 管道串联
来源：http://www.blog.sjlbkw.cn/Article/details/gdpyizbyf.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.yfazqb.com/Article/details/glqxsjwyb.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.vehdjk.com/Article/details/gnbuhuhcy.sHtML

cmd > out.log 2>&1
来源：http://read.share.fktsv.cn/Article/details/gismzktrh.sHtML

[R40] 追加写日志
来源：http://wap.epnwcf.com/Article/details/gaemruyrx.sHtML

echo "log" >> out.log
来源：http://blog.tarul.cn/Article/details/gdxpbxlvg.sHtML

[R41] 丢弃输出
来源：http://blog.yfazqb.com/Article/details/gmrtzawnb.sHtML

cmd >/dev/null 2>&1
来源：http://3g.tarul.cn/Article/details/gedzarnpt.sHtML

[R42] 输入重定向
来源：http://www.m.share.yfazqb.com/Article/details/gutcmkdyy.sHtML

wc -l < a.txt
来源：http://3g.tarul.cn/Article/details/gpkzmuhvn.sHtML

[R43] 按名字查找文件
来源：http://www.share.bbcook.cn/Article/details/gymxstkwp.sHtML

find . -name "*.log" -type f
来源：http://www.share.fktsv.cn/Article/details/giurbjqzt.sHtML

[R44] 按修改时间查找
来源：http://www.share.epnwcf.com/Article/details/gzavcdumb.sHtML

find . -mtime -7 -type f
来源：http://mobile.fktsv.cn/Article/details/gwshoukiy.sHtML

[R45] 批量删除
来源：http://3g.tarul.cn/Article/details/gwbjdqjcs.sHtML

find . -name "*.tmp" -delete
来源：http://3g.vehdjk.com/Article/details/ggryiupkq.sHtML

[R46] 递归替换文件内容
来源：http://3g.yfazqb.com/Article/details/gslnvabzk.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.tarul.cn/Article/details/gpefcuymh.sHtML

[R47] sed 单行替换
来源：http://3g.fktsv.cn/Article/details/gwnbrmxnd.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.bbcook.cn/Article/details/gaeliecsv.sHtML

[R48] awk 取指定列
来源：http://wap.epnwcf.com/Article/details/gksonvoen.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.yfazqb.com/Article/details/gjftdwihb.sHtML

[R49] awk 带条件
来源：http://blog.bbcook.cn/Article/details/gojdqryzq.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.bbcook.cn/Article/details/gydzqytwm.sHtML

[R50] awk 求和
来源：http://mobile.epnwcf.com/Article/details/gzpinzdai.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.sjlbkw.cn/Article/details/gqowrbwuc.sHtML

[R51] 排序去重取前几
来源：http://m.share.yfazqb.com/Article/details/gvnjkyopz.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.vehdjk.com/Article/details/gtoqihvyj.sHtML

[R52] 统计行数
来源：http://www.share.bbcook.cn/Article/details/gaggggojp.sHtML

wc -l a.txt
来源：http://blog.epnwcf.com/Article/details/gxlrekinj.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.tarul.cn/Article/details/ghrskfcne.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.tarul.cn/Article/details/gmnjomqqg.sHtML

[R54] 比较两个文件
来源：http://www.share.bbcook.cn/Article/details/gggxieogz.sHtML

diff a.txt b.txt
来源：http://read.share.sjlbkw.cn/Article/details/gmrkiuepr.sHtML

[R55] 压缩与解压
来源：http://wap.fktsv.cn/Article/details/gizwlcmba.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.sjlbkw.cn/Article/details/grjqogwxx.sHtML

[R56] 远程拷贝
来源：http://www.share.fktsv.cn/Article/details/glcygilgn.sHtML

scp file user@host:/path/
来源：http://www.blog.fktsv.cn/Article/details/giwargnem.sHtML

[R57] 远程执行命令
来源：http://baike.bbcook.cn/Article/details/gdvrpughy.sHtML

ssh user@host 'uptime'
来源：http://3g.tarul.cn/Article/details/gyxqwbeqq.sHtML

[R58] 下载文件
来源：http://m.share.epnwcf.com/Article/details/gwsbzgafa.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.epnwcf.com/Article/details/grxlmvnxf.sHtML

[R59] 发 POST JSON
来源：http://mobile.yfazqb.com/Article/details/gaqvvguzx.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fktsv.cn/Article/details/govhzqtpb.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.vehdjk.com/Article/details/gsgdexwwr.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.vehdjk.com/Article/details/ggbdflgbg.sHtML

[R61] 磁盘占用
来源：http://www.m.share.bbcook.cn/Article/details/gxorutnqd.sHtML

df -h;  du -sh *
来源：http://www.m.share.fktsv.cn/Article/details/gsdfrrhjt.sHtML

[R62] 找最占空间的文件
来源：http://m.share.tarul.cn/Article/details/gwowsxbdr.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.bbcook.cn/Article/details/gryersewg.sHtML

[R63] 内存与进程
来源：http://www.m.share.epnwcf.com/Article/details/glqshefmi.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.vehdjk.com/Article/details/gbdhrkdmg.sHtML

[R64] 结束进程
来源：http://www.blog.bbcook.cn/Article/details/gwdmlwcrs.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.epnwcf.com/Article/details/gjstmader.sHtML

[R65] 查看端口占用
来源：http://m.share.vehdjk.com/Article/details/gxthgveba.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.epnwcf.com/Article/details/gwfndgcmx.sHtML

[R66] 定时任务
来源：http://read.share.bbcook.cn/Article/details/gbtiffqit.sHtML

crontab -e;  crontab -l
来源：http://www.share.yfazqb.com/Article/details/gsmsyinwq.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fktsv.cn/Article/details/geijizsez.sHtML

openssl rand -hex 16
来源：http://mobile.epnwcf.com/Article/details/gkhgurlrl.sHtML

[R68] 计算文件校验值
来源：http://mobile.tarul.cn/Article/details/geguappwm.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.tarul.cn/Article/details/ggclipdij.sHtML

[R69] 生成随机密码
来源：http://wap.epnwcf.com/Article/details/gnogzbkdi.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.fktsv.cn/Article/details/gdlwjkgie.sHtML

[R70] 时间戳与互转
来源：http://wap.yfazqb.com/Article/details/gulrpekyg.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.bbcook.cn/Article/details/gasfdxiix.sHtML

[R71] 日期格式化
来源：http://mobile.tarul.cn/Article/details/grwszmeyr.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.sjlbkw.cn/Article/details/gympoaxnf.sHtML

[R72] 等待端口就绪
来源：http://wap.tarul.cn/Article/details/grwljpqck.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.sjlbkw.cn/Article/details/glbsdvgyz.sHtML

[R73] 分割大日志
来源：http://mobile.bbcook.cn/Article/details/gcdbgbqxp.sHtML

split -l 1000 big.log part_
来源：http://wap.vehdjk.com/Article/details/gwtykjvsk.sHtML

[R74] 批量重命名
来源：http://mobile.yfazqb.com/Article/details/gphidokvy.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.epnwcf.com/Article/details/gcwgvohzy.sHtML

[R75] 导出环境变量
来源：http://read.share.epnwcf.com/Article/details/gxkbofphu.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.sjlbkw.cn/Article/details/gwzesbzft.sHtML

[R76] 使用临时文件
来源：http://3g.epnwcf.com/Article/details/gkdogrgxi.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.tarul.cn/Article/details/guqufyejj.sHtML

[R77] 读取用户输入
来源：http://www.blog.fktsv.cn/Article/details/gkqlxnprb.sHtML

read -rp "请输入: " ans
来源：http://blog.yfazqb.com/Article/details/gopltywlw.sHtML

[R78] 交互式菜单
来源：http://www.blog.bbcook.cn/Article/details/guujzohqi.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fktsv.cn/Article/details/gdzwsmkdi.sHtML

[R79] 解析命令行选项
来源：http://mobile.bbcook.cn/Article/details/gvkrjvjbs.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fktsv.cn/Article/details/gsdqqluaz.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.sjlbkw.cn/Article/details/glkrqwayx.sHtML

time ./run.sh
来源：http://m.share.sjlbkw.cn/Article/details/gqxqdqjkj.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gagyoweis.sHtML

S. C / C++ 专题
来源：http://wap.epnwcf.com/Article/details/grxpfqyyq.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gsmzyhjgw.sHtML

[S01] C：Hello World
来源：http://www.blog.vehdjk.com/Article/details/gfjejzkjx.sHtML

#include <stdio.h>
来源：http://www.m.share.tarul.cn/Article/details/ghboapiff.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.bbcook.cn/Article/details/grwcscfyg.sHtML

[S02] C：变量与格式化输出
来源：http://3g.vehdjk.com/Article/details/gvymytrie.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.vehdjk.com/Article/details/gcgzddpvk.sHtML

[S03] C：读入整数
来源：http://baike.vehdjk.com/Article/details/gowzqywil.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.vehdjk.com/Article/details/glrbzzrap.sHtML

[S04] C：字符串复制
来源：http://m.share.vehdjk.com/Article/details/gnlskgmkv.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.epnwcf.com/Article/details/gtqxeaxzn.sHtML

[S05] C：字符串长度
来源：http://m.share.fktsv.cn/Article/details/gulvopaqs.sHtML

strlen(s)
来源：http://read.share.sjlbkw.cn/Article/details/ggubmqtia.sHtML

[S06] C：字符串比较
来源：http://baike.vehdjk.com/Article/details/gumsnoaef.sHtML

strcmp(a, b) == 0
来源：http://baike.fktsv.cn/Article/details/gtzfbkvpk.sHtML

[S07] C：数组遍历求和
来源：http://www.share.sjlbkw.cn/Article/details/gwbvsogea.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.tarul.cn/Article/details/gohuiazud.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.tarul.cn/Article/details/gfxezujdc.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.fktsv.cn/Article/details/gukdrsitb.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.vehdjk.com/Article/details/gskooybzd.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.epnwcf.com/Article/details/gqkqsbviq.sHtML

[S10] C：指针与解引用
来源：http://3g.yfazqb.com/Article/details/guvghvafl.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.yfazqb.com/Article/details/gleukajgq.sHtML

[S11] C：逐行读文件
来源：http://wap.fktsv.cn/Article/details/gixgpexdk.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.yfazqb.com/Article/details/guaxeohxf.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.tarul.cn/Article/details/ghyzwksbv.sHtML

fclose(f);
来源：http://m.share.epnwcf.com/Article/details/gzohyoxog.sHtML

[S12] C：写文件
来源：http://www.blog.bbcook.cn/Article/details/gvxfjpcbn.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.sjlbkw.cn/Article/details/gyxrhcedm.sHtML

[S13] C：宏定义
来源：http://www.m.share.bbcook.cn/Article/details/gyklwfdyr.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fktsv.cn/Article/details/gfmdhzkpc.sHtML

[S14] C：枚举
来源：http://m.share.tarul.cn/Article/details/gcuzcejmo.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.bbcook.cn/Article/details/gvjgcpmdh.sHtML

[S15] C：类型转换
来源：http://m.share.bbcook.cn/Article/details/gxgqlhyfl.sHtML

(double) a / b
来源：http://mobile.sjlbkw.cn/Article/details/gzjtpaxqp.sHtML

[S16] C：位操作置位
来源：http://m.share.tarul.cn/Article/details/gezmqtlyx.sHtML

x |= (1 << 3);
来源：http://www.share.fktsv.cn/Article/details/gmrrlmagw.sHtML

[S17] C：安全拼接字符串
来源：http://baike.fktsv.cn/Article/details/grasmynwp.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.vehdjk.com/Article/details/gccicdpbm.sHtML

[S18] C：命令行参数
来源：http://read.share.tarul.cn/Article/details/ggmrkqssz.sHtML

int main(int argc, char **argv)
来源：http://wap.bbcook.cn/Article/details/ghtwbxjbd.sHtML

[S19] C：快速排序
来源：http://3g.sjlbkw.cn/Article/details/gyevhoorb.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.vehdjk.com/Article/details/gzibiinam.sHtML

[S20] C：二分查找
来源：http://read.share.bbcook.cn/Article/details/gyalhbtwm.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.tarul.cn/Article/details/gwrlbmyzm.sHtML

[S21] C：字符类别判断
来源：http://mobile.fktsv.cn/Article/details/gaxvbycgl.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.sjlbkw.cn/Article/details/gjuhxjdqe.sHtML

[S22] C：字符串转数字
来源：http://blog.sjlbkw.cn/Article/details/gqmpgytua.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.yfazqb.com/Article/details/gveauyrqu.sHtML

[S23] C：随机数
来源：http://www.share.tarul.cn/Article/details/gimuyqlia.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.vehdjk.com/Article/details/gssgzfvju.sHtML

[S24] C：获取本地时间
来源：http://wap.vehdjk.com/Article/details/gjlhrhpdl.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.tarul.cn/Article/details/glwioxugm.sHtML

[S25] C：内存拷贝
来源：http://mobile.tarul.cn/Article/details/gxaqvdtxp.sHtML

memcpy(dst, src, n);
来源：http://wap.bbcook.cn/Article/details/gfftymbui.sHtML

[S26] C：内存清零
来源：http://wap.sjlbkw.cn/Article/details/ghsiexngs.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.tarul.cn/Article/details/gzdijyjlr.sHtML

[S27] C：定义常量
来源：http://wap.epnwcf.com/Article/details/grdrkqoud.sHtML

const double PI = 3.14159;
来源：http://mobile.tarul.cn/Article/details/giksyzbxp.sHtML

[S28] C：静态变量
来源：http://blog.epnwcf.com/Article/details/gsegkihho.sHtML

static int counter = 0;
来源：http://wap.tarul.cn/Article/details/ggslsuqef.sHtML

[S29] C：变参函数
来源：http://wap.epnwcf.com/Article/details/gbnhdfazm.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.bbcook.cn/Article/details/gatynuxon.sHtML

[S30] C：头文件保护
来源：http://www.blog.yfazqb.com/Article/details/gtxhdenau.sHtML

#ifndef X_H
来源：http://read.share.epnwcf.com/Article/details/ggladyazf.sHtML

#define X_H
来源：http://baike.bbcook.cn/Article/details/gypxvekyo.sHtML

#endif
来源：http://wap.yfazqb.com/Article/details/gmtkijtdo.sHtML

[S31] C++：Hello World
来源：http://www.blog.epnwcf.com/Article/details/ghoqxaidk.sHtML

#include <iostream>
来源：http://mobile.fktsv.cn/Article/details/gjoqxxwln.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.tarul.cn/Article/details/gimnqqywq.sHtML

[S32] C++：字符串
来源：http://baike.yfazqb.com/Article/details/gebchrqsl.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.epnwcf.com/Article/details/giouhjtze.sHtML

[S33] C++：vector 增删
来源：http://baike.fktsv.cn/Article/details/govdrhwgd.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.sjlbkw.cn/Article/details/gcjgakszz.sHtML

[S34] C++：遍历 vector
来源：http://read.share.sjlbkw.cn/Article/details/gkajflfqt.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.bbcook.cn/Article/details/gereulsbb.sHtML

[S35] C++：map
来源：http://www.m.share.yfazqb.com/Article/details/gnfuriaop.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.vehdjk.com/Article/details/gpunojnkj.sHtML

[S36] C++：unordered_map
来源：http://3g.bbcook.cn/Article/details/goiguxpbj.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.bbcook.cn/Article/details/gjknesqke.sHtML

[S37] C++：set
来源：http://baike.bbcook.cn/Article/details/gzwjfedwo.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.sjlbkw.cn/Article/details/gpropysgg.sHtML

[S38] C++：排序
来源：http://wap.sjlbkw.cn/Article/details/goasuccdd.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fktsv.cn/Article/details/gjfewkhpa.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.yfazqb.com/Article/details/guldwqneq.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.tarul.cn/Article/details/gtklqffio.sHtML

[S40] C++：查找元素
来源：http://baike.tarul.cn/Article/details/gpohanapn.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.vehdjk.com/Article/details/gnpuxafbg.sHtML

[S41] C++：类与构造函数
来源：http://read.share.bbcook.cn/Article/details/gztdvgtvw.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.vehdjk.com/Article/details/gfvrywryq.sHtML

[S42] C++：继承与虚函数
来源：http://blog.sjlbkw.cn/Article/details/ghcfcsgfv.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.bbcook.cn/Article/details/gdoywdabx.sHtML

[S43] C++：智能指针
来源：http://read.share.fktsv.cn/Article/details/gdqsjdobd.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.vehdjk.com/Article/details/gizvgfbzs.sHtML

[S44] C++：引用传参
来源：http://www.m.share.epnwcf.com/Article/details/gcztkqssi.sHtML

void inc(int &x) { ++x; }
来源：http://3g.bbcook.cn/Article/details/gpqyfbcuc.sHtML


<!-- 参考信息 -->