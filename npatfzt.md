代发 wailian999

ROLLBACK TO sp1;
来源：http://baike.bbcook.cn/Article/details/gnrjzgqes.sHtML

[Q69] 查看执行计划
来源：http://m.share.sjlbkw.cn/Article/details/gefvkstqz.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.yfazqb.com/Article/details/gskcyejkw.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.vehdjk.com/Article/details/gtrdrjmrv.sHtML

ANALYZE TABLE users;
来源：http://baike.bbcook.cn/Article/details/gomyjjwme.sHtML

[Q71] 查看建表语句
来源：http://mobile.fktsv.cn/Article/details/gqbzxpfah.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.tarul.cn/Article/details/gxrawdefy.sHtML

[Q72] 查看索引
来源：http://baike.vehdjk.com/Article/details/gwdatthub.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.fktsv.cn/Article/details/gxcxwrpua.sHtML

[Q73] 查看表状态
来源：http://www.blog.tarul.cn/Article/details/govnfaack.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.sjlbkw.cn/Article/details/gdhtgdkdc.sHtML

[Q74] 强制使用索引
来源：http://mobile.vehdjk.com/Article/details/grrrlhbgk.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.bbcook.cn/Article/details/gpqtruyus.sHtML

[Q75] 日期格式化
来源：http://read.share.vehdjk.com/Article/details/gvloelwfz.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.fktsv.cn/Article/details/gsaektlxt.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.fktsv.cn/Article/details/gukfqirdj.sHtML

[Q76] 按天统计
来源：http://mobile.yfazqb.com/Article/details/ggtzvsove.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.fktsv.cn/Article/details/gevaiwivy.sHtML

[Q77] 时间加减
来源：http://www.blog.yfazqb.com/Article/details/gbkfaomzg.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.yfazqb.com/Article/details/gyjrdhryy.sHtML

[Q78] 当前时间
来源：http://www.share.fktsv.cn/Article/details/gsaqayigp.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.bbcook.cn/Article/details/gyvxesbwc.sHtML

[Q79] 字符串拼接
来源：http://baike.vehdjk.com/Article/details/ggeocdzih.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.fktsv.cn/Article/details/gkcjrxgwv.sHtML

[Q80] 字符串截取
来源：http://www.m.share.yfazqb.com/Article/details/ghibnpphg.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.tarul.cn/Article/details/gkhoyxvjm.sHtML

[Q81] 字符串替换
来源：http://baike.sjlbkw.cn/Article/details/gtkewchnv.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.epnwcf.com/Article/details/gbgwvpknz.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.bbcook.cn/Article/details/gjtxgyrvp.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.tarul.cn/Article/details/ggogswjwz.sHtML

[Q83] 大小写转换
来源：http://mobile.epnwcf.com/Article/details/gryienduj.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.bbcook.cn/Article/details/gyjyescxm.sHtML

[Q84] 去除首尾空格
来源：http://m.share.bbcook.cn/Article/details/gczvwyxoq.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.sjlbkw.cn/Article/details/ghhszulpo.sHtML

[Q85] 数值取整
来源：http://read.share.bbcook.cn/Article/details/gprvctakc.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.epnwcf.com/Article/details/gmjfqxeeu.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.tarul.cn/Article/details/gbuqshwgi.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.yfazqb.com/Article/details/gbfjvtgng.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.yfazqb.com/Article/details/gpabrciud.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.tarul.cn/Article/details/gkidwkucu.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.fktsv.cn/Article/details/giphepetf.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.epnwcf.com/Article/details/gnezpmqtl.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.yfazqb.com/Article/details/gvafnxvkr.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.tarul.cn/Article/details/gogdosyql.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.tarul.cn/Article/details/gvxqzyulx.sHtML

[Q90] 生成序号列
来源：http://read.share.yfazqb.com/Article/details/gusdflqml.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.sjlbkw.cn/Article/details/grenfgouy.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/galcyppfw.sHtML

R. Bash 专题
来源：http://3g.fktsv.cn/Article/details/gyatcjvqw.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gflrwxehj.sHtML

[R01] shebang 与严格模式
来源：http://read.share.bbcook.cn/Article/details/gtkhvgxut.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.yfazqb.com/Article/details/ggdrhovov.sHtML

set -euo pipefail
来源：http://m.share.fktsv.cn/Article/details/gvswtoktb.sHtML

[R02] 变量赋值与使用
来源：http://www.share.epnwcf.com/Article/details/gggyurfmh.sHtML

name="Tom"; echo "$name"
来源：http://read.share.bbcook.cn/Article/details/gmxzyhqlc.sHtML

[R03] 只读变量
来源：http://m.share.yfazqb.com/Article/details/guoxpfbeu.sHtML

readonly PI=3.14
来源：http://www.blog.sjlbkw.cn/Article/details/ghnjfqwxs.sHtML

[R04] 位置参数
来源：http://m.share.vehdjk.com/Article/details/gxahvaaym.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.tarul.cn/Article/details/gnvlgzhlq.sHtML

[R05] 参数默认值
来源：http://wap.bbcook.cn/Article/details/gsodfisde.sHtML

name="${1:-default}"
来源：http://wap.bbcook.cn/Article/details/ghyiazhit.sHtML

[R06] 判断命令是否存在
来源：http://mobile.yfazqb.com/Article/details/gkdubgwuy.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.yfazqb.com/Article/details/gwsofewwf.sHtML

[R07] if 判断文件
来源：http://wap.bbcook.cn/Article/details/gkrzmoycg.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.vehdjk.com/Article/details/gmwemmzyo.sHtML

[R08] 数值比较
来源：http://read.share.yfazqb.com/Article/details/gsutdcoqh.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.vehdjk.com/Article/details/gxonafzli.sHtML

[R09] 字符串比较
来源：http://blog.yfazqb.com/Article/details/geycyyaak.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.tarul.cn/Article/details/gwkbiaved.sHtML

[R10] 正则匹配
来源：http://read.share.yfazqb.com/Article/details/grvfwizeh.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.yfazqb.com/Article/details/gyiunsaqy.sHtML

[R11] case 多分支
来源：http://www.m.share.sjlbkw.cn/Article/details/gvswkdmdy.sHtML

case "$1" in
来源：http://wap.sjlbkw.cn/Article/details/gxxpyjtkv.sHtML

start) echo "启动" ;;
来源：http://3g.vehdjk.com/Article/details/gboedgzcm.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.vehdjk.com/Article/details/getwcwoet.sHtML

*)     echo "未知命令" ;;
来源：http://baike.sjlbkw.cn/Article/details/gudxtywqa.sHtML

esac
来源：http://mobile.fktsv.cn/Article/details/gvcqcktmx.sHtML

[R12] for 遍历文件
来源：http://read.share.tarul.cn/Article/details/ghqyvemrs.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.epnwcf.com/Article/details/gzbwoimup.sHtML

[R13] for 计数循环
来源：http://read.share.epnwcf.com/Article/details/gbumvovjd.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.sjlbkw.cn/Article/details/gigowqtza.sHtML

[R14] C 风格 for
来源：http://wap.tarul.cn/Article/details/geeoplayw.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.bbcook.cn/Article/details/gbcktsyej.sHtML

[R15] while 逐行读文件
来源：http://www.share.epnwcf.com/Article/details/gvfqcjlmg.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.yfazqb.com/Article/details/gesntjvez.sHtML

[R16] until 等待条件
来源：http://wap.yfazqb.com/Article/details/gcqgcalyn.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.yfazqb.com/Article/details/gdtpapydo.sHtML

[R17] 数组定义与取值
来源：http://baike.sjlbkw.cn/Article/details/gzikrylsc.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.yfazqb.com/Article/details/givaykdns.sHtML

[R18] 遍历数组
来源：http://read.share.vehdjk.com/Article/details/glincqchs.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.bbcook.cn/Article/details/gqqcjycxi.sHtML

[R19] 数组长度
来源：http://3g.sjlbkw.cn/Article/details/gmmvtfctn.sHtML

echo "${#arr[@]}"
来源：http://3g.epnwcf.com/Article/details/gdhxxzufp.sHtML

[R20] 关联数组（字典）
来源：http://baike.epnwcf.com/Article/details/grczkvchx.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.epnwcf.com/Article/details/gmvscniph.sHtML

[R21] 字符串长度
来源：http://baike.epnwcf.com/Article/details/glmfyosig.sHtML

echo "${#s}"
来源：http://m.share.fktsv.cn/Article/details/gvymnvowl.sHtML

[R22] 截取子串
来源：http://3g.sjlbkw.cn/Article/details/gqodprduj.sHtML

echo "${s:0:5}"
来源：http://3g.fktsv.cn/Article/details/geifcrpym.sHtML

[R23] 字符串替换
来源：http://wap.vehdjk.com/Article/details/gdezqxqdc.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fktsv.cn/Article/details/gcxsvlblf.sHtML

[R24] 大小写转换
来源：http://blog.tarul.cn/Article/details/gzdyxzlgv.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.epnwcf.com/Article/details/guwkdpxtt.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.epnwcf.com/Article/details/gnrnsntxf.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.vehdjk.com/Article/details/gvvlmuhep.sHtML

[R26] 命令替换
来源：http://www.share.vehdjk.com/Article/details/gqfsfsvry.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.sjlbkw.cn/Article/details/gkrjzcauk.sHtML

[R27] 算术展开
来源：http://m.share.yfazqb.com/Article/details/grzrxuswt.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.vehdjk.com/Article/details/gtgwcuiri.sHtML

[R28] 浮点运算
来源：http://mobile.vehdjk.com/Article/details/gxrjrsykp.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.tarul.cn/Article/details/gstyvhqqt.sHtML

[R29] 定义函数
来源：http://mobile.yfazqb.com/Article/details/gyuwekojg.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.vehdjk.com/Article/details/gnleidpui.sHtML

[R30] 函数返回状态码
来源：http://wap.sjlbkw.cn/Article/details/gciydtfox.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.sjlbkw.cn/Article/details/gbymjbvud.sHtML

[R31] 局部变量
来源：http://baike.yfazqb.com/Article/details/gvvxfgcqg.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.yfazqb.com/Article/details/gpwfikzyi.sHtML

[R32] 参数个数校验
来源：http://www.blog.fktsv.cn/Article/details/glttaazbi.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.epnwcf.com/Article/details/gyeudkzoj.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.tarul.cn/Article/details/gcddtlarg.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.epnwcf.com/Article/details/gvtuikczz.sHtML

[R34] 退出时清理
来源：http://m.share.fktsv.cn/Article/details/gefyxpypb.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.yfazqb.com/Article/details/gykmazpkl.sHtML

[R35] 后台执行并等待
来源：http://blog.sjlbkw.cn/Article/details/giezymcsn.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.bbcook.cn/Article/details/gesvjivme.sHtML

[R36] 并发执行多个任务
来源：http://www.share.yfazqb.com/Article/details/gewviplnc.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.vehdjk.com/Article/details/groczipqh.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.sjlbkw.cn/Article/details/gqelmcofu.sHtML

files=$(ls -1)
来源：http://m.share.fktsv.cn/Article/details/gwmukmigv.sHtML

[R38] 管道串联
来源：http://www.share.fktsv.cn/Article/details/gllcejcjs.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.yfazqb.com/Article/details/gemczvweo.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.epnwcf.com/Article/details/guvcysfbs.sHtML

cmd > out.log 2>&1
来源：http://www.blog.epnwcf.com/Article/details/gfxmhmlwy.sHtML

[R40] 追加写日志
来源：http://blog.tarul.cn/Article/details/gyrzrzsvp.sHtML

echo "log" >> out.log
来源：http://m.share.vehdjk.com/Article/details/ggaxgxmnl.sHtML

[R41] 丢弃输出
来源：http://3g.tarul.cn/Article/details/gytqmvpcq.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.tarul.cn/Article/details/geelwlyrx.sHtML

[R42] 输入重定向
来源：http://wap.bbcook.cn/Article/details/guvqpkhjs.sHtML

wc -l < a.txt
来源：http://m.share.sjlbkw.cn/Article/details/gmkredozr.sHtML

[R43] 按名字查找文件
来源：http://m.share.tarul.cn/Article/details/groenijfb.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.fktsv.cn/Article/details/gnewdgpmm.sHtML

[R44] 按修改时间查找
来源：http://m.share.sjlbkw.cn/Article/details/gaayyqnxi.sHtML

find . -mtime -7 -type f
来源：http://baike.bbcook.cn/Article/details/giyimkfiq.sHtML

[R45] 批量删除
来源：http://m.share.tarul.cn/Article/details/gmvfxwlup.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.yfazqb.com/Article/details/gjfyxfinp.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.yfazqb.com/Article/details/gbixqpejk.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.tarul.cn/Article/details/gehhabcnt.sHtML

[R47] sed 单行替换
来源：http://m.share.bbcook.cn/Article/details/giaknpysu.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.yfazqb.com/Article/details/gwccuejdx.sHtML

[R48] awk 取指定列
来源：http://mobile.yfazqb.com/Article/details/gocpxnwci.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.epnwcf.com/Article/details/gswqhmxhj.sHtML

[R49] awk 带条件
来源：http://wap.vehdjk.com/Article/details/gwguaaald.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.bbcook.cn/Article/details/guhspewhk.sHtML

[R50] awk 求和
来源：http://www.blog.bbcook.cn/Article/details/goyitvmih.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fktsv.cn/Article/details/gmmohskxy.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.yfazqb.com/Article/details/gsttuchnu.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.tarul.cn/Article/details/gxyhpfkud.sHtML

[R52] 统计行数
来源：http://www.blog.fktsv.cn/Article/details/gcpddwlfy.sHtML

wc -l a.txt
来源：http://3g.tarul.cn/Article/details/grhxdqluq.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.epnwcf.com/Article/details/gsbkdxsuv.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.vehdjk.com/Article/details/ghjaxrvou.sHtML

[R54] 比较两个文件
来源：http://read.share.sjlbkw.cn/Article/details/gqvipieky.sHtML

diff a.txt b.txt
来源：http://3g.epnwcf.com/Article/details/gwugqfsmq.sHtML

[R55] 压缩与解压
来源：http://www.blog.fktsv.cn/Article/details/gwtcspjth.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.bbcook.cn/Article/details/gxkcavene.sHtML

[R56] 远程拷贝
来源：http://m.share.vehdjk.com/Article/details/gshkdideu.sHtML

scp file user@host:/path/
来源：http://baike.fktsv.cn/Article/details/gsdajjigo.sHtML

[R57] 远程执行命令
来源：http://m.share.epnwcf.com/Article/details/gpqlhxlng.sHtML

ssh user@host 'uptime'
来源：http://mobile.yfazqb.com/Article/details/gjijmfdrm.sHtML

[R58] 下载文件
来源：http://baike.vehdjk.com/Article/details/gkvgzkcmq.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.fktsv.cn/Article/details/gnbqlehyr.sHtML

[R59] 发 POST JSON
来源：http://3g.epnwcf.com/Article/details/ggotzrnzx.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.vehdjk.com/Article/details/gistkmmcv.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.sjlbkw.cn/Article/details/ghbfxygyw.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.yfazqb.com/Article/details/gmfchoqln.sHtML

[R61] 磁盘占用
来源：http://blog.vehdjk.com/Article/details/gromnjimr.sHtML

df -h;  du -sh *
来源：http://baike.bbcook.cn/Article/details/gjsdextgk.sHtML

[R62] 找最占空间的文件
来源：http://m.share.bbcook.cn/Article/details/gcmdtkykq.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.tarul.cn/Article/details/gneyjjezx.sHtML

[R63] 内存与进程
来源：http://read.share.bbcook.cn/Article/details/gyvxrxbjl.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.epnwcf.com/Article/details/gwgyfbaeh.sHtML

[R64] 结束进程
来源：http://mobile.fktsv.cn/Article/details/gmnqaqvpa.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.sjlbkw.cn/Article/details/gwucfjnwn.sHtML

[R65] 查看端口占用
来源：http://baike.bbcook.cn/Article/details/gezmptnyl.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.yfazqb.com/Article/details/gdphfikaw.sHtML

[R66] 定时任务
来源：http://mobile.epnwcf.com/Article/details/gcnkchdjs.sHtML

crontab -e;  crontab -l
来源：http://m.share.epnwcf.com/Article/details/gzmkswmdy.sHtML

[R67] 生成随机十六进制串
来源：http://wap.bbcook.cn/Article/details/gywsaxnrm.sHtML

openssl rand -hex 16
来源：http://blog.yfazqb.com/Article/details/gtlblchox.sHtML

[R68] 计算文件校验值
来源：http://m.share.yfazqb.com/Article/details/gidzprjqn.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fktsv.cn/Article/details/gdhwzglbp.sHtML

[R69] 生成随机密码
来源：http://wap.fktsv.cn/Article/details/gdvqjdkxy.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.epnwcf.com/Article/details/ghulklblp.sHtML

[R70] 时间戳与互转
来源：http://www.blog.sjlbkw.cn/Article/details/gjouxpraq.sHtML

date +%s;  date -d @1700000000
来源：http://3g.yfazqb.com/Article/details/gwxxxzsqu.sHtML

[R71] 日期格式化
来源：http://mobile.bbcook.cn/Article/details/gamrmtidp.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.epnwcf.com/Article/details/gmvipsofa.sHtML

[R72] 等待端口就绪
来源：http://3g.tarul.cn/Article/details/gmcjeyxni.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.tarul.cn/Article/details/gfjchrukb.sHtML

[R73] 分割大日志
来源：http://mobile.fktsv.cn/Article/details/gvuydnlvn.sHtML

split -l 1000 big.log part_
来源：http://wap.sjlbkw.cn/Article/details/gzwbrsuyz.sHtML

[R74] 批量重命名
来源：http://3g.bbcook.cn/Article/details/gxmzvxjlj.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.bbcook.cn/Article/details/ghwooiljp.sHtML

[R75] 导出环境变量
来源：http://read.share.yfazqb.com/Article/details/gtkrwvcys.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.vehdjk.com/Article/details/gvfzoyfpk.sHtML

[R76] 使用临时文件
来源：http://wap.fktsv.cn/Article/details/gobtbeave.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.vehdjk.com/Article/details/gqkeiualg.sHtML

[R77] 读取用户输入
来源：http://www.blog.epnwcf.com/Article/details/gnaoazggo.sHtML

read -rp "请输入: " ans
来源：http://mobile.yfazqb.com/Article/details/gpncbhuhy.sHtML

[R78] 交互式菜单
来源：http://www.share.vehdjk.com/Article/details/gjmbcxykr.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.bbcook.cn/Article/details/ghvmuqvwv.sHtML

[R79] 解析命令行选项
来源：http://baike.sjlbkw.cn/Article/details/gcdibziep.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.vehdjk.com/Article/details/gqsqaisla.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.yfazqb.com/Article/details/gdrxmvvqp.sHtML

time ./run.sh
来源：http://mobile.bbcook.cn/Article/details/gitmegphz.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/ghcahsmjt.sHtML

S. C / C++ 专题
来源：http://baike.fktsv.cn/Article/details/gdgbwswdf.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gzrmbtqwt.sHtML

[S01] C：Hello World
来源：http://mobile.bbcook.cn/Article/details/gcotsyixf.sHtML

#include <stdio.h>
来源：http://wap.epnwcf.com/Article/details/gjsxlqqec.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.sjlbkw.cn/Article/details/gkufxnstf.sHtML

[S02] C：变量与格式化输出
来源：http://baike.sjlbkw.cn/Article/details/gjtryfipf.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fktsv.cn/Article/details/gpercyvls.sHtML

[S03] C：读入整数
来源：http://baike.tarul.cn/Article/details/gjwrlmvtb.sHtML

int x; scanf("%d", &x);
来源：http://mobile.fktsv.cn/Article/details/gxkfyzqad.sHtML

[S04] C：字符串复制
来源：http://read.share.yfazqb.com/Article/details/gfluplqld.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.fktsv.cn/Article/details/gschxaffm.sHtML

[S05] C：字符串长度
来源：http://www.m.share.tarul.cn/Article/details/gwsaxhqzx.sHtML

strlen(s)
来源：http://mobile.bbcook.cn/Article/details/gjhjbnblf.sHtML

[S06] C：字符串比较
来源：http://www.blog.yfazqb.com/Article/details/gemtvladv.sHtML

strcmp(a, b) == 0
来源：http://wap.sjlbkw.cn/Article/details/gbmiafdzi.sHtML

[S07] C：数组遍历求和
来源：http://baike.sjlbkw.cn/Article/details/gydopulyc.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.bbcook.cn/Article/details/gtoutdnki.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.bbcook.cn/Article/details/gpvcdenxg.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.bbcook.cn/Article/details/gshssrzhj.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.bbcook.cn/Article/details/gdmjywmdm.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.yfazqb.com/Article/details/gqacddqpk.sHtML

[S10] C：指针与解引用
来源：http://wap.epnwcf.com/Article/details/gdenhlmnq.sHtML

int *p = &a;  *p = 5;
来源：http://blog.vehdjk.com/Article/details/gbabbzikn.sHtML

[S11] C：逐行读文件
来源：http://3g.bbcook.cn/Article/details/goxsiuuzt.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.sjlbkw.cn/Article/details/grpdyqutk.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.vehdjk.com/Article/details/grdzyotyp.sHtML

fclose(f);
来源：http://baike.bbcook.cn/Article/details/gswxvepju.sHtML

[S12] C：写文件
来源：http://www.blog.sjlbkw.cn/Article/details/gkkkzligs.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.vehdjk.com/Article/details/ghflxrgrw.sHtML

[S13] C：宏定义
来源：http://read.share.sjlbkw.cn/Article/details/gvgocmvik.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.yfazqb.com/Article/details/ghgxgvgbw.sHtML

[S14] C：枚举
来源：http://3g.sjlbkw.cn/Article/details/gjzyjhjwp.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.epnwcf.com/Article/details/gvqbhiusi.sHtML

[S15] C：类型转换
来源：http://www.m.share.vehdjk.com/Article/details/gwsgouucz.sHtML

(double) a / b
来源：http://mobile.epnwcf.com/Article/details/gycmxzqth.sHtML

[S16] C：位操作置位
来源：http://wap.yfazqb.com/Article/details/gwhtjiniq.sHtML

x |= (1 << 3);
来源：http://blog.sjlbkw.cn/Article/details/grbkicgfm.sHtML

[S17] C：安全拼接字符串
来源：http://wap.sjlbkw.cn/Article/details/gczbhznqa.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.epnwcf.com/Article/details/gtsxhdrfq.sHtML

[S18] C：命令行参数
来源：http://read.share.yfazqb.com/Article/details/gqqhvmyla.sHtML

int main(int argc, char **argv)
来源：http://www.share.sjlbkw.cn/Article/details/grgwhhplf.sHtML

[S19] C：快速排序
来源：http://mobile.epnwcf.com/Article/details/gzotlyijh.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fktsv.cn/Article/details/gfxplqcce.sHtML

[S20] C：二分查找
来源：http://3g.sjlbkw.cn/Article/details/gtpghyscu.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.yfazqb.com/Article/details/gtpcsijlw.sHtML

[S21] C：字符类别判断
来源：http://www.blog.bbcook.cn/Article/details/gydlbhnaw.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.tarul.cn/Article/details/gsydgouih.sHtML

[S22] C：字符串转数字
来源：http://blog.sjlbkw.cn/Article/details/gegnnqcot.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.epnwcf.com/Article/details/gjuewyswn.sHtML

[S23] C：随机数
来源：http://read.share.sjlbkw.cn/Article/details/gdaqvjcxz.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.fktsv.cn/Article/details/gscwnrbdo.sHtML

[S24] C：获取本地时间
来源：http://www.blog.sjlbkw.cn/Article/details/ggpnozkqk.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fktsv.cn/Article/details/gvybwhqsg.sHtML

[S25] C：内存拷贝
来源：http://www.blog.sjlbkw.cn/Article/details/gpjwcatpy.sHtML

memcpy(dst, src, n);
来源：http://blog.tarul.cn/Article/details/gobjkycgf.sHtML

[S26] C：内存清零
来源：http://3g.sjlbkw.cn/Article/details/gtkwzdiwf.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.tarul.cn/Article/details/ggyyuorcl.sHtML

[S27] C：定义常量
来源：http://blog.sjlbkw.cn/Article/details/guyjdcpoa.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fktsv.cn/Article/details/gurdfplpe.sHtML

[S28] C：静态变量
来源：http://read.share.epnwcf.com/Article/details/glfklldfk.sHtML

static int counter = 0;
来源：http://www.m.share.bbcook.cn/Article/details/gspqnihut.sHtML

[S29] C：变参函数
来源：http://www.blog.tarul.cn/Article/details/gtehkhxdg.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.sjlbkw.cn/Article/details/gighjcptp.sHtML

[S30] C：头文件保护
来源：http://wap.tarul.cn/Article/details/gswoebtmw.sHtML

#ifndef X_H
来源：http://www.share.vehdjk.com/Article/details/ggwyvlqhc.sHtML

#define X_H
来源：http://mobile.vehdjk.com/Article/details/gdibpupwi.sHtML

#endif
来源：http://read.share.vehdjk.com/Article/details/gusmlvyxg.sHtML

[S31] C++：Hello World
来源：http://3g.tarul.cn/Article/details/gwgejfoct.sHtML

#include <iostream>
来源：http://wap.vehdjk.com/Article/details/gktkfwkdl.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.sjlbkw.cn/Article/details/gusbfkkbg.sHtML

[S32] C++：字符串
来源：http://www.m.share.sjlbkw.cn/Article/details/gelldwiye.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.epnwcf.com/Article/details/gwrresziq.sHtML

[S33] C++：vector 增删
来源：http://mobile.fktsv.cn/Article/details/ggndgamrf.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fktsv.cn/Article/details/grbrclvhb.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fktsv.cn/Article/details/gncolndct.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.sjlbkw.cn/Article/details/gsdawczgj.sHtML

[S35] C++：map
来源：http://mobile.sjlbkw.cn/Article/details/gmflbghmu.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.yfazqb.com/Article/details/glakjbdqb.sHtML

[S36] C++：unordered_map
来源：http://baike.fktsv.cn/Article/details/gxduyiciy.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.yfazqb.com/Article/details/ghopohtol.sHtML

[S37] C++：set
来源：http://m.share.sjlbkw.cn/Article/details/gtpamgnwt.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.epnwcf.com/Article/details/gkkpurzer.sHtML

[S38] C++：排序
来源：http://wap.fktsv.cn/Article/details/guqdmayvm.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.tarul.cn/Article/details/gumzjivwi.sHtML


<!-- 参考信息 -->