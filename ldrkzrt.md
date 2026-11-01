代发 wailian999

SHOW INDEX FROM users;
来源：http://wap.fktsv.cn/Article/details/gyqmnsfbn.sHtML

[Q73] 查看表状态
来源：http://www.blog.bbcook.cn/Article/details/gmxygyfvc.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.vehdjk.com/Article/details/ghumieznf.sHtML

[Q74] 强制使用索引
来源：http://www.blog.fktsv.cn/Article/details/gpoppgdwg.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.fktsv.cn/Article/details/gwtiwfrsn.sHtML

[Q75] 日期格式化
来源：http://read.share.fktsv.cn/Article/details/gfxdgyvwi.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.sjlbkw.cn/Article/details/gtfvrrjue.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.vehdjk.com/Article/details/giyomdpws.sHtML

[Q76] 按天统计
来源：http://m.share.bbcook.cn/Article/details/gakoajhjc.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.yfazqb.com/Article/details/gtzidaxlf.sHtML

[Q77] 时间加减
来源：http://mobile.fktsv.cn/Article/details/gkurvtlzx.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.epnwcf.com/Article/details/gqawbjfsk.sHtML

[Q78] 当前时间
来源：http://baike.epnwcf.com/Article/details/gekzugvav.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.bbcook.cn/Article/details/gnpocvkwz.sHtML

[Q79] 字符串拼接
来源：http://wap.bbcook.cn/Article/details/gpeqwvzwi.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.fktsv.cn/Article/details/gxqkfxzxi.sHtML

[Q80] 字符串截取
来源：http://wap.tarul.cn/Article/details/gvqgknbtm.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.bbcook.cn/Article/details/gqlorfsja.sHtML

[Q81] 字符串替换
来源：http://www.blog.sjlbkw.cn/Article/details/grnlmftye.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.yfazqb.com/Article/details/gkekzoaic.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.fktsv.cn/Article/details/gnbponjnh.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.fktsv.cn/Article/details/gjzckfbtt.sHtML

[Q83] 大小写转换
来源：http://wap.bbcook.cn/Article/details/gbefbvkyd.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.sjlbkw.cn/Article/details/gaiuckunp.sHtML

[Q84] 去除首尾空格
来源：http://mobile.fktsv.cn/Article/details/gqlqibggy.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.tarul.cn/Article/details/gypeumiia.sHtML

[Q85] 数值取整
来源：http://wap.tarul.cn/Article/details/gzhakvltn.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.bbcook.cn/Article/details/galnaxurr.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.sjlbkw.cn/Article/details/ghjenthfl.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.vehdjk.com/Article/details/gvyrkcohw.sHtML

[Q87] JSON 字段做条件
来源：http://wap.fktsv.cn/Article/details/gqztommgh.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.epnwcf.com/Article/details/gjjvwzxpo.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.epnwcf.com/Article/details/gfloldcvw.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.vehdjk.com/Article/details/gyeccgght.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.sjlbkw.cn/Article/details/gbvzowuec.sHtML

[Q89] 判断表是否存在
来源：http://m.share.vehdjk.com/Article/details/ggemzngqa.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.sjlbkw.cn/Article/details/grdwrntbk.sHtML

[Q90] 生成序号列
来源：http://blog.epnwcf.com/Article/details/gkyrtefmo.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.yfazqb.com/Article/details/gqermggyx.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gyulwkttq.sHtML

R. Bash 专题
来源：http://www.share.bbcook.cn/Article/details/gzzbbmsrg.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gfubaezxg.sHtML

[R01] shebang 与严格模式
来源：http://mobile.epnwcf.com/Article/details/ghwsxporb.sHtML

#!/usr/bin/env bash
来源：http://3g.bbcook.cn/Article/details/gdcxcfauz.sHtML

set -euo pipefail
来源：http://www.share.tarul.cn/Article/details/gmiugdrdc.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.bbcook.cn/Article/details/glnjmazjb.sHtML

name="Tom"; echo "$name"
来源：http://blog.yfazqb.com/Article/details/gdffglwtk.sHtML

[R03] 只读变量
来源：http://baike.fktsv.cn/Article/details/gqeqrgzni.sHtML

readonly PI=3.14
来源：http://baike.yfazqb.com/Article/details/gumvcwqex.sHtML

[R04] 位置参数
来源：http://www.m.share.vehdjk.com/Article/details/gjmzowlak.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.vehdjk.com/Article/details/gzbxijbjo.sHtML

[R05] 参数默认值
来源：http://wap.vehdjk.com/Article/details/gzcxajoyt.sHtML

name="${1:-default}"
来源：http://www.m.share.tarul.cn/Article/details/gavekhrlt.sHtML

[R06] 判断命令是否存在
来源：http://blog.sjlbkw.cn/Article/details/gexeeicos.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.epnwcf.com/Article/details/gsvvbgkjb.sHtML

[R07] if 判断文件
来源：http://mobile.vehdjk.com/Article/details/gmhcriecd.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.sjlbkw.cn/Article/details/gxryknvxv.sHtML

[R08] 数值比较
来源：http://wap.vehdjk.com/Article/details/gkflopykm.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.epnwcf.com/Article/details/gdhstlroz.sHtML

[R09] 字符串比较
来源：http://m.share.epnwcf.com/Article/details/gmprgtdcu.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.yfazqb.com/Article/details/ggzujcyuv.sHtML

[R10] 正则匹配
来源：http://mobile.tarul.cn/Article/details/gpwnjgyao.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.tarul.cn/Article/details/gfdbidwzv.sHtML

[R11] case 多分支
来源：http://blog.yfazqb.com/Article/details/gevzhtzrp.sHtML

case "$1" in
来源：http://read.share.fktsv.cn/Article/details/gnpdyzykw.sHtML

start) echo "启动" ;;
来源：http://blog.bbcook.cn/Article/details/gctrfwksl.sHtML

stop)  echo "停止" ;;
来源：http://blog.tarul.cn/Article/details/gaiwozitf.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.sjlbkw.cn/Article/details/gfoqzjdyb.sHtML

esac
来源：http://www.m.share.yfazqb.com/Article/details/gqlbtigbs.sHtML

[R12] for 遍历文件
来源：http://baike.yfazqb.com/Article/details/gfuchtmlr.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.yfazqb.com/Article/details/gtklkdduo.sHtML

[R13] for 计数循环
来源：http://wap.bbcook.cn/Article/details/guvouhefl.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.vehdjk.com/Article/details/gaffjbzfe.sHtML

[R14] C 风格 for
来源：http://www.m.share.epnwcf.com/Article/details/grksbelrv.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.tarul.cn/Article/details/giejamewx.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.yfazqb.com/Article/details/gzdqztjqx.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.bbcook.cn/Article/details/gzqmflmwi.sHtML

[R16] until 等待条件
来源：http://blog.bbcook.cn/Article/details/gksjwplgp.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.vehdjk.com/Article/details/gkhabtawq.sHtML

[R17] 数组定义与取值
来源：http://3g.bbcook.cn/Article/details/gqfsunpva.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.fktsv.cn/Article/details/ggqccrwph.sHtML

[R18] 遍历数组
来源：http://www.m.share.yfazqb.com/Article/details/gkolzdyjh.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.epnwcf.com/Article/details/gjytihvap.sHtML

[R19] 数组长度
来源：http://mobile.tarul.cn/Article/details/gpxlkpqpv.sHtML

echo "${#arr[@]}"
来源：http://wap.fktsv.cn/Article/details/gtzmgdkui.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.tarul.cn/Article/details/gaixokgne.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.bbcook.cn/Article/details/gvpyviwto.sHtML

[R21] 字符串长度
来源：http://baike.epnwcf.com/Article/details/gcbruqxdi.sHtML

echo "${#s}"
来源：http://mobile.sjlbkw.cn/Article/details/gqpeeyloc.sHtML

[R22] 截取子串
来源：http://wap.fktsv.cn/Article/details/gyivchjiq.sHtML

echo "${s:0:5}"
来源：http://www.blog.vehdjk.com/Article/details/gbopfzkev.sHtML

[R23] 字符串替换
来源：http://www.blog.vehdjk.com/Article/details/gttcstfug.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fktsv.cn/Article/details/gqqbnmfiz.sHtML

[R24] 大小写转换
来源：http://wap.epnwcf.com/Article/details/gshckeyay.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.tarul.cn/Article/details/gfrocjilg.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.bbcook.cn/Article/details/ggyrpmudi.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fktsv.cn/Article/details/gwodgqplf.sHtML

[R26] 命令替换
来源：http://www.m.share.vehdjk.com/Article/details/gwncvdlkw.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.fktsv.cn/Article/details/gknpympwo.sHtML

[R27] 算术展开
来源：http://baike.vehdjk.com/Article/details/gnptugkjy.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.yfazqb.com/Article/details/ggcpyfyfb.sHtML

[R28] 浮点运算
来源：http://3g.epnwcf.com/Article/details/gxytniujv.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.fktsv.cn/Article/details/gruinjcgh.sHtML

[R29] 定义函数
来源：http://read.share.tarul.cn/Article/details/gqfhfbilu.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.yfazqb.com/Article/details/gavyceffo.sHtML

[R30] 函数返回状态码
来源：http://m.share.epnwcf.com/Article/details/grdffnksa.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.epnwcf.com/Article/details/gqibaovbs.sHtML

[R31] 局部变量
来源：http://www.share.epnwcf.com/Article/details/gvohqboro.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.sjlbkw.cn/Article/details/gnooufmzi.sHtML

[R32] 参数个数校验
来源：http://mobile.fktsv.cn/Article/details/guwtdxbdi.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.tarul.cn/Article/details/grabwtlgi.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.yfazqb.com/Article/details/griinbttd.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.tarul.cn/Article/details/gjjasmswq.sHtML

[R34] 退出时清理
来源：http://read.share.vehdjk.com/Article/details/gefczdkef.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.yfazqb.com/Article/details/gxjzrocfd.sHtML

[R35] 后台执行并等待
来源：http://www.share.bbcook.cn/Article/details/gjoktahxf.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.epnwcf.com/Article/details/gtfkufcbz.sHtML

[R36] 并发执行多个任务
来源：http://baike.tarul.cn/Article/details/glipopirv.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.bbcook.cn/Article/details/gcpvnecjl.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fktsv.cn/Article/details/gyzqdcspx.sHtML

files=$(ls -1)
来源：http://mobile.vehdjk.com/Article/details/gmtvjpytd.sHtML

[R38] 管道串联
来源：http://mobile.tarul.cn/Article/details/gzmuqqybr.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.fktsv.cn/Article/details/giyiziyhl.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.tarul.cn/Article/details/gflebcnnl.sHtML

cmd > out.log 2>&1
来源：http://wap.fktsv.cn/Article/details/gngeapesm.sHtML

[R40] 追加写日志
来源：http://blog.epnwcf.com/Article/details/gceizzljk.sHtML

echo "log" >> out.log
来源：http://wap.vehdjk.com/Article/details/gfqrqspyk.sHtML

[R41] 丢弃输出
来源：http://m.share.vehdjk.com/Article/details/grpdpipqp.sHtML

cmd >/dev/null 2>&1
来源：http://baike.epnwcf.com/Article/details/gbzfkxbzq.sHtML

[R42] 输入重定向
来源：http://blog.epnwcf.com/Article/details/gakvgrdju.sHtML

wc -l < a.txt
来源：http://www.m.share.sjlbkw.cn/Article/details/gpdewdigc.sHtML

[R43] 按名字查找文件
来源：http://baike.bbcook.cn/Article/details/gpzicmhag.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.tarul.cn/Article/details/glikwxhpc.sHtML

[R44] 按修改时间查找
来源：http://www.blog.epnwcf.com/Article/details/goqsbppdo.sHtML

find . -mtime -7 -type f
来源：http://wap.tarul.cn/Article/details/gbtmgujtp.sHtML

[R45] 批量删除
来源：http://mobile.sjlbkw.cn/Article/details/giwpfztzh.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.sjlbkw.cn/Article/details/gfkbkfegk.sHtML

[R46] 递归替换文件内容
来源：http://read.share.tarul.cn/Article/details/giopqjofd.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.tarul.cn/Article/details/ghljlsayz.sHtML

[R47] sed 单行替换
来源：http://m.share.fktsv.cn/Article/details/gfhasdcea.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.bbcook.cn/Article/details/gxiuevqsa.sHtML

[R48] awk 取指定列
来源：http://wap.bbcook.cn/Article/details/gtagwvjcy.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.tarul.cn/Article/details/gqqnfaydh.sHtML

[R49] awk 带条件
来源：http://read.share.fktsv.cn/Article/details/gdftobpdz.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fktsv.cn/Article/details/gkhhibibc.sHtML

[R50] awk 求和
来源：http://www.share.sjlbkw.cn/Article/details/gyjlcdddu.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.sjlbkw.cn/Article/details/gfyeczedh.sHtML

[R51] 排序去重取前几
来源：http://m.share.vehdjk.com/Article/details/gtvoyqfzd.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.sjlbkw.cn/Article/details/giwxakdqq.sHtML

[R52] 统计行数
来源：http://read.share.tarul.cn/Article/details/gryhenbye.sHtML

wc -l a.txt
来源：http://www.blog.sjlbkw.cn/Article/details/gkqaahzsa.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.tarul.cn/Article/details/gohozyivv.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.yfazqb.com/Article/details/gtymggsaa.sHtML

[R54] 比较两个文件
来源：http://read.share.sjlbkw.cn/Article/details/gynjzqqpx.sHtML

diff a.txt b.txt
来源：http://mobile.sjlbkw.cn/Article/details/gwwlkaefs.sHtML

[R55] 压缩与解压
来源：http://read.share.tarul.cn/Article/details/gtscjqzcr.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.tarul.cn/Article/details/gcmdraenh.sHtML

[R56] 远程拷贝
来源：http://3g.vehdjk.com/Article/details/gejluisou.sHtML

scp file user@host:/path/
来源：http://mobile.vehdjk.com/Article/details/gedragadn.sHtML

[R57] 远程执行命令
来源：http://m.share.tarul.cn/Article/details/gkjsscucr.sHtML

ssh user@host 'uptime'
来源：http://3g.sjlbkw.cn/Article/details/gvnnpoguz.sHtML

[R58] 下载文件
来源：http://www.share.yfazqb.com/Article/details/gotzzaovs.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.yfazqb.com/Article/details/gwoyqfyvf.sHtML

[R59] 发 POST JSON
来源：http://blog.fktsv.cn/Article/details/gjzpsfaux.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.sjlbkw.cn/Article/details/guzqzkyzy.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.epnwcf.com/Article/details/gdwykgrbu.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.epnwcf.com/Article/details/glbbupdbr.sHtML

[R61] 磁盘占用
来源：http://www.m.share.yfazqb.com/Article/details/gumlhjhqe.sHtML

df -h;  du -sh *
来源：http://mobile.sjlbkw.cn/Article/details/gtgthjzkw.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fktsv.cn/Article/details/gxlddzoxz.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.sjlbkw.cn/Article/details/gkckhnftu.sHtML

[R63] 内存与进程
来源：http://blog.vehdjk.com/Article/details/ghfmyehez.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.bbcook.cn/Article/details/gjvwfwhvk.sHtML

[R64] 结束进程
来源：http://wap.tarul.cn/Article/details/gmcgmfnkv.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.epnwcf.com/Article/details/gnywvesuq.sHtML

[R65] 查看端口占用
来源：http://read.share.tarul.cn/Article/details/gqjjykeam.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.vehdjk.com/Article/details/gcggagalh.sHtML

[R66] 定时任务
来源：http://mobile.sjlbkw.cn/Article/details/gavgfwrqy.sHtML

crontab -e;  crontab -l
来源：http://mobile.epnwcf.com/Article/details/gkjwzlhel.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fktsv.cn/Article/details/gvqbjkamc.sHtML

openssl rand -hex 16
来源：http://blog.vehdjk.com/Article/details/gzecpskep.sHtML

[R68] 计算文件校验值
来源：http://mobile.sjlbkw.cn/Article/details/gqirhhofd.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.yfazqb.com/Article/details/gdipkjrmg.sHtML

[R69] 生成随机密码
来源：http://blog.tarul.cn/Article/details/gclgnnlyj.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fktsv.cn/Article/details/ghcsyaqsq.sHtML

[R70] 时间戳与互转
来源：http://wap.vehdjk.com/Article/details/gninkwouo.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.fktsv.cn/Article/details/gisjnnath.sHtML

[R71] 日期格式化
来源：http://www.m.share.bbcook.cn/Article/details/gfmilmdbt.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.yfazqb.com/Article/details/gxbypwcic.sHtML

[R72] 等待端口就绪
来源：http://baike.fktsv.cn/Article/details/gomlnlpoc.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.yfazqb.com/Article/details/gwitpghvb.sHtML

[R73] 分割大日志
来源：http://www.blog.epnwcf.com/Article/details/gxxcoilei.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.bbcook.cn/Article/details/gwgkjzzip.sHtML

[R74] 批量重命名
来源：http://read.share.bbcook.cn/Article/details/gcpccohir.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.vehdjk.com/Article/details/gvihuiaun.sHtML

[R75] 导出环境变量
来源：http://www.share.tarul.cn/Article/details/gmyewgqyp.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.bbcook.cn/Article/details/gvbotioxq.sHtML

[R76] 使用临时文件
来源：http://read.share.bbcook.cn/Article/details/glgvtrcen.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.bbcook.cn/Article/details/gsvlqjjay.sHtML

[R77] 读取用户输入
来源：http://www.m.share.sjlbkw.cn/Article/details/gkvwabncs.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.bbcook.cn/Article/details/gcniczgtw.sHtML

[R78] 交互式菜单
来源：http://www.share.fktsv.cn/Article/details/gofiirczz.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.tarul.cn/Article/details/guchdviay.sHtML

[R79] 解析命令行选项
来源：http://baike.tarul.cn/Article/details/gijlwlqhz.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.fktsv.cn/Article/details/gjpfyuaxy.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.epnwcf.com/Article/details/ghktpnafu.sHtML

time ./run.sh
来源：http://blog.sjlbkw.cn/Article/details/gufbnehpd.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gpvtxzrxi.sHtML

S. C / C++ 专题
来源：http://baike.bbcook.cn/Article/details/gogmwtjez.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gvtkvyhuy.sHtML

[S01] C：Hello World
来源：http://www.m.share.fktsv.cn/Article/details/gmewdintk.sHtML

#include <stdio.h>
来源：http://mobile.fktsv.cn/Article/details/guayiqqkh.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.sjlbkw.cn/Article/details/gwjwpgtxm.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.vehdjk.com/Article/details/gdjdsolpd.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.epnwcf.com/Article/details/gjwbsokdd.sHtML

[S03] C：读入整数
来源：http://www.share.yfazqb.com/Article/details/gekwyrubl.sHtML

int x; scanf("%d", &x);
来源：http://wap.tarul.cn/Article/details/gfgzqnxev.sHtML

[S04] C：字符串复制
来源：http://www.share.vehdjk.com/Article/details/gmvuoossc.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.yfazqb.com/Article/details/gzisstase.sHtML

[S05] C：字符串长度
来源：http://www.m.share.vehdjk.com/Article/details/gdanppnnw.sHtML

strlen(s)
来源：http://www.m.share.tarul.cn/Article/details/gbkwwfxnk.sHtML

[S06] C：字符串比较
来源：http://m.share.sjlbkw.cn/Article/details/gngosstff.sHtML

strcmp(a, b) == 0
来源：http://www.blog.vehdjk.com/Article/details/govhxlgzp.sHtML

[S07] C：数组遍历求和
来源：http://wap.vehdjk.com/Article/details/gtdjqvdqv.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.bbcook.cn/Article/details/gblqxnfyp.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.bbcook.cn/Article/details/gujjwzahh.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.bbcook.cn/Article/details/ggvpjurnn.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.bbcook.cn/Article/details/gmtrzqztr.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.yfazqb.com/Article/details/glbcpivqm.sHtML

[S10] C：指针与解引用
来源：http://wap.yfazqb.com/Article/details/gctsrfugk.sHtML

int *p = &a;  *p = 5;
来源：http://wap.tarul.cn/Article/details/gxypylxqh.sHtML

[S11] C：逐行读文件
来源：http://blog.epnwcf.com/Article/details/gwpzjleuw.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.fktsv.cn/Article/details/gichakqsb.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.yfazqb.com/Article/details/gitxqplqh.sHtML

fclose(f);
来源：http://www.share.sjlbkw.cn/Article/details/ghxpeucex.sHtML

[S12] C：写文件
来源：http://blog.epnwcf.com/Article/details/guoswziip.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.tarul.cn/Article/details/grditdyfw.sHtML

[S13] C：宏定义
来源：http://wap.yfazqb.com/Article/details/gkhamwgcl.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.epnwcf.com/Article/details/gvtjahvhd.sHtML

[S14] C：枚举
来源：http://read.share.vehdjk.com/Article/details/ggkcnkwag.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.tarul.cn/Article/details/gwjclirxd.sHtML

[S15] C：类型转换
来源：http://mobile.bbcook.cn/Article/details/gengxzhgm.sHtML

(double) a / b
来源：http://www.share.sjlbkw.cn/Article/details/gmtsdgxoc.sHtML

[S16] C：位操作置位
来源：http://www.share.yfazqb.com/Article/details/gmecdwaka.sHtML

x |= (1 << 3);
来源：http://read.share.fktsv.cn/Article/details/gtksnxitx.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.vehdjk.com/Article/details/gsvcqgexf.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.fktsv.cn/Article/details/gksmveygg.sHtML

[S18] C：命令行参数
来源：http://wap.sjlbkw.cn/Article/details/glnwdaxrj.sHtML

int main(int argc, char **argv)
来源：http://blog.fktsv.cn/Article/details/ghjqlhvyq.sHtML

[S19] C：快速排序
来源：http://m.share.sjlbkw.cn/Article/details/gvnslivxw.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.yfazqb.com/Article/details/ghraeects.sHtML

[S20] C：二分查找
来源：http://baike.epnwcf.com/Article/details/gnaoxafxv.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.yfazqb.com/Article/details/ggftwwdmk.sHtML

[S21] C：字符类别判断
来源：http://blog.bbcook.cn/Article/details/gnncnghbt.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.vehdjk.com/Article/details/gguslumme.sHtML

[S22] C：字符串转数字
来源：http://mobile.yfazqb.com/Article/details/gcbqlaebh.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.yfazqb.com/Article/details/gudgltbxj.sHtML

[S23] C：随机数
来源：http://blog.epnwcf.com/Article/details/gtfbxzamd.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.sjlbkw.cn/Article/details/gqcvanpbw.sHtML

[S24] C：获取本地时间
来源：http://read.share.yfazqb.com/Article/details/gyresbztb.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.epnwcf.com/Article/details/gbsgcpnrs.sHtML

[S25] C：内存拷贝
来源：http://www.blog.yfazqb.com/Article/details/gklfdvxix.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.yfazqb.com/Article/details/grywwerld.sHtML

[S26] C：内存清零
来源：http://www.m.share.tarul.cn/Article/details/gqivcrjpy.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fktsv.cn/Article/details/gopgtazxu.sHtML

[S27] C：定义常量
来源：http://read.share.yfazqb.com/Article/details/ghmaascbu.sHtML

const double PI = 3.14159;
来源：http://mobile.yfazqb.com/Article/details/gkkolfnzi.sHtML

[S28] C：静态变量
来源：http://baike.bbcook.cn/Article/details/gwgjvuuyw.sHtML

static int counter = 0;
来源：http://www.blog.bbcook.cn/Article/details/gdsfkfhli.sHtML

[S29] C：变参函数
来源：http://blog.tarul.cn/Article/details/gzynltwbb.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fktsv.cn/Article/details/gotlajgwl.sHtML

[S30] C：头文件保护
来源：http://www.share.tarul.cn/Article/details/gxfopkuxw.sHtML

#ifndef X_H
来源：http://www.blog.yfazqb.com/Article/details/gzwvdhvzw.sHtML

#define X_H
来源：http://mobile.sjlbkw.cn/Article/details/gkicjcbzy.sHtML

#endif
来源：http://wap.vehdjk.com/Article/details/gkzomynfr.sHtML

[S31] C++：Hello World
来源：http://3g.fktsv.cn/Article/details/gcuoddjke.sHtML

#include <iostream>
来源：http://www.blog.yfazqb.com/Article/details/gntiwclaj.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fktsv.cn/Article/details/gwsmbmttw.sHtML

[S32] C++：字符串
来源：http://www.share.sjlbkw.cn/Article/details/gmrkqxasv.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.bbcook.cn/Article/details/gtkmmqxez.sHtML

[S33] C++：vector 增删
来源：http://read.share.epnwcf.com/Article/details/gbrrsvpek.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.bbcook.cn/Article/details/gflibvega.sHtML

[S34] C++：遍历 vector
来源：http://baike.yfazqb.com/Article/details/gvbhjyreo.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.vehdjk.com/Article/details/ghrbcjkon.sHtML

[S35] C++：map
来源：http://m.share.bbcook.cn/Article/details/gagwhrpip.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.tarul.cn/Article/details/gtrfuxwqk.sHtML

[S36] C++：unordered_map
来源：http://blog.sjlbkw.cn/Article/details/gemredssr.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.bbcook.cn/Article/details/gzojybidj.sHtML

[S37] C++：set
来源：http://read.share.sjlbkw.cn/Article/details/gujctdexj.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fktsv.cn/Article/details/gpirblbdq.sHtML

[S38] C++：排序
来源：http://www.m.share.bbcook.cn/Article/details/gkowfqwth.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.epnwcf.com/Article/details/gemqcgpkh.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.sjlbkw.cn/Article/details/gwgomnwki.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.vehdjk.com/Article/details/gfexdmnod.sHtML

[S40] C++：查找元素
来源：http://read.share.yfazqb.com/Article/details/gewaphupu.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.vehdjk.com/Article/details/grigobthl.sHtML

[S41] C++：类与构造函数
来源：http://wap.sjlbkw.cn/Article/details/gnhyueesv.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.yfazqb.com/Article/details/glvqynnjk.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.tarul.cn/Article/details/gixehksbb.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.bbcook.cn/Article/details/gtrlbnmzi.sHtML


<!-- 参考信息 -->