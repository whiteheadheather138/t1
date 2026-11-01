代发 wailian999

[Q67] 设置隔离级别
来源：http://mobile.yfazqb.com/Article/details/gqfpbudqq.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.bbcook.cn/Article/details/gmkqhtczd.sHtML

[Q68] 保存点
来源：http://wap.sjlbkw.cn/Article/details/gfevzpnhc.sHtML

SAVEPOINT sp1;
来源：http://mobile.vehdjk.com/Article/details/gqrjnoxbr.sHtML

ROLLBACK TO sp1;
来源：http://www.share.tarul.cn/Article/details/gvcsloksi.sHtML

[Q69] 查看执行计划
来源：http://m.share.bbcook.cn/Article/details/gppwgnyug.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.tarul.cn/Article/details/gawajpjza.sHtML

[Q70] 更新统计信息
来源：http://blog.tarul.cn/Article/details/gkcxhbiqk.sHtML

ANALYZE TABLE users;
来源：http://blog.yfazqb.com/Article/details/gwxuxsqon.sHtML

[Q71] 查看建表语句
来源：http://www.blog.fktsv.cn/Article/details/gxomftsom.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.tarul.cn/Article/details/gbvajrfdy.sHtML

[Q72] 查看索引
来源：http://read.share.epnwcf.com/Article/details/gsazkwtyk.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/gklispkhn.sHtML

[Q73] 查看表状态
来源：http://blog.yfazqb.com/Article/details/ggluphoit.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.vehdjk.com/Article/details/gnligneoe.sHtML

[Q74] 强制使用索引
来源：http://wap.epnwcf.com/Article/details/glhxiemev.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.fktsv.cn/Article/details/giiagqmoy.sHtML

[Q75] 日期格式化
来源：http://baike.bbcook.cn/Article/details/gxajafosq.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.sjlbkw.cn/Article/details/gedxxoyvf.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.fktsv.cn/Article/details/grvwzyohn.sHtML

[Q76] 按天统计
来源：http://read.share.fktsv.cn/Article/details/gkhimtgej.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.fktsv.cn/Article/details/gejvjjcde.sHtML

[Q77] 时间加减
来源：http://baike.tarul.cn/Article/details/ggtndlbke.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.bbcook.cn/Article/details/ggvgvwryq.sHtML

[Q78] 当前时间
来源：http://www.share.fktsv.cn/Article/details/geoemejhq.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.sjlbkw.cn/Article/details/gvjjmrftg.sHtML

[Q79] 字符串拼接
来源：http://read.share.epnwcf.com/Article/details/glzxpvmcd.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.fktsv.cn/Article/details/gyswdciql.sHtML

[Q80] 字符串截取
来源：http://m.share.yfazqb.com/Article/details/ghuaxxfgv.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.vehdjk.com/Article/details/gflygsoau.sHtML

[Q81] 字符串替换
来源：http://wap.fktsv.cn/Article/details/gtzvaydeq.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.tarul.cn/Article/details/ghfrnwnan.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.yfazqb.com/Article/details/gisjftqbb.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/gcnrexuaq.sHtML

[Q83] 大小写转换
来源：http://read.share.sjlbkw.cn/Article/details/glfxjfiot.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.yfazqb.com/Article/details/gfbcylseq.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.fktsv.cn/Article/details/gyzhryadx.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.epnwcf.com/Article/details/gdgzxnlhz.sHtML

[Q85] 数值取整
来源：http://www.blog.epnwcf.com/Article/details/ghodhkqfp.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.epnwcf.com/Article/details/gcqqpkuqn.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.fktsv.cn/Article/details/gdkkviebk.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.bbcook.cn/Article/details/gesglncfq.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.sjlbkw.cn/Article/details/gyuzsknfj.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.vehdjk.com/Article/details/gshqvhbty.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.epnwcf.com/Article/details/ggftdnnwc.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.epnwcf.com/Article/details/ggtqsttdw.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.fktsv.cn/Article/details/gtcotmhbj.sHtML

[Q89] 判断表是否存在
来源：http://www.share.fktsv.cn/Article/details/gdwcnpiix.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.yfazqb.com/Article/details/gileokmzf.sHtML

[Q90] 生成序号列
来源：http://m.share.yfazqb.com/Article/details/gzasmbwzh.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.epnwcf.com/Article/details/goyeknmzg.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gddiijurg.sHtML

R. Bash 专题
来源：http://www.share.yfazqb.com/Article/details/gvxsqnuzw.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gzpoaiorw.sHtML

[R01] shebang 与严格模式
来源：http://www.share.tarul.cn/Article/details/gllzwpxjj.sHtML

#!/usr/bin/env bash
来源：http://www.share.tarul.cn/Article/details/gfrnjrnhe.sHtML

set -euo pipefail
来源：http://mobile.epnwcf.com/Article/details/gswgcorgh.sHtML

[R02] 变量赋值与使用
来源：http://blog.sjlbkw.cn/Article/details/gtcnzfzhe.sHtML

name="Tom"; echo "$name"
来源：http://3g.tarul.cn/Article/details/gecumbyej.sHtML

[R03] 只读变量
来源：http://mobile.vehdjk.com/Article/details/gkrbpxewm.sHtML

readonly PI=3.14
来源：http://www.m.share.fktsv.cn/Article/details/gnvsfltxd.sHtML

[R04] 位置参数
来源：http://www.m.share.bbcook.cn/Article/details/gantmqhav.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.sjlbkw.cn/Article/details/gzkzvpqhs.sHtML

[R05] 参数默认值
来源：http://www.m.share.tarul.cn/Article/details/grgwatlfi.sHtML

name="${1:-default}"
来源：http://mobile.tarul.cn/Article/details/gyoxvdfpf.sHtML

[R06] 判断命令是否存在
来源：http://blog.fktsv.cn/Article/details/gbkdkpddm.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.vehdjk.com/Article/details/gnmupwabt.sHtML

[R07] if 判断文件
来源：http://blog.epnwcf.com/Article/details/ghodnsvoi.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.epnwcf.com/Article/details/gbqznqhrt.sHtML

[R08] 数值比较
来源：http://www.blog.yfazqb.com/Article/details/gfvlqbshk.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.yfazqb.com/Article/details/gnjfwbnck.sHtML

[R09] 字符串比较
来源：http://mobile.epnwcf.com/Article/details/gvjvttuob.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.fktsv.cn/Article/details/grixqzsck.sHtML

[R10] 正则匹配
来源：http://read.share.fktsv.cn/Article/details/goahjbpqx.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.vehdjk.com/Article/details/gtapkdaud.sHtML

[R11] case 多分支
来源：http://www.share.epnwcf.com/Article/details/gartyzfef.sHtML

case "$1" in
来源：http://read.share.epnwcf.com/Article/details/gdxtdcaba.sHtML

start) echo "启动" ;;
来源：http://3g.tarul.cn/Article/details/guunbuyzm.sHtML

stop)  echo "停止" ;;
来源：http://baike.vehdjk.com/Article/details/gsoadcwos.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.fktsv.cn/Article/details/gmgehxgpc.sHtML

esac
来源：http://www.share.sjlbkw.cn/Article/details/gymedeody.sHtML

[R12] for 遍历文件
来源：http://www.m.share.bbcook.cn/Article/details/gyrwiwasw.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.fktsv.cn/Article/details/gfazsurae.sHtML

[R13] for 计数循环
来源：http://baike.vehdjk.com/Article/details/geigrtkua.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.fktsv.cn/Article/details/garmrxdgx.sHtML

[R14] C 风格 for
来源：http://www.share.vehdjk.com/Article/details/giybwtouj.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.fktsv.cn/Article/details/gtixajazr.sHtML

[R15] while 逐行读文件
来源：http://baike.vehdjk.com/Article/details/gqhjlxvis.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.sjlbkw.cn/Article/details/gpyiuewes.sHtML

[R16] until 等待条件
来源：http://blog.fktsv.cn/Article/details/gejejdzix.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.sjlbkw.cn/Article/details/gtypswjwn.sHtML

[R17] 数组定义与取值
来源：http://3g.bbcook.cn/Article/details/gqchbhdod.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.sjlbkw.cn/Article/details/gfmhhjjbq.sHtML

[R18] 遍历数组
来源：http://mobile.bbcook.cn/Article/details/goywdhubl.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.bbcook.cn/Article/details/gcwdfldpn.sHtML

[R19] 数组长度
来源：http://blog.bbcook.cn/Article/details/gskkghgqx.sHtML

echo "${#arr[@]}"
来源：http://3g.fktsv.cn/Article/details/gfufawjkp.sHtML

[R20] 关联数组（字典）
来源：http://blog.epnwcf.com/Article/details/gitqquyse.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.bbcook.cn/Article/details/gytbgccfn.sHtML

[R21] 字符串长度
来源：http://blog.fktsv.cn/Article/details/gndksfnqi.sHtML

echo "${#s}"
来源：http://read.share.epnwcf.com/Article/details/gluqamsaw.sHtML

[R22] 截取子串
来源：http://read.share.bbcook.cn/Article/details/gmmevuudz.sHtML

echo "${s:0:5}"
来源：http://m.share.tarul.cn/Article/details/gcuuoaabq.sHtML

[R23] 字符串替换
来源：http://m.share.yfazqb.com/Article/details/glrlebktv.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.tarul.cn/Article/details/gsdmrmkup.sHtML

[R24] 大小写转换
来源：http://wap.fktsv.cn/Article/details/gbawykrel.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.sjlbkw.cn/Article/details/gfkaxcfmh.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.tarul.cn/Article/details/glrmececm.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.yfazqb.com/Article/details/gmboitzxm.sHtML

[R26] 命令替换
来源：http://mobile.tarul.cn/Article/details/gxbepkymj.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.bbcook.cn/Article/details/ghvquvnbd.sHtML

[R27] 算术展开
来源：http://3g.vehdjk.com/Article/details/gypeiwpmj.sHtML

echo $((1 + 2 * 3))
来源：http://wap.vehdjk.com/Article/details/ghdgczccy.sHtML

[R28] 浮点运算
来源：http://www.blog.fktsv.cn/Article/details/gvcxqyzmq.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.tarul.cn/Article/details/gtztkqoue.sHtML

[R29] 定义函数
来源：http://blog.vehdjk.com/Article/details/gdjfnphom.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.bbcook.cn/Article/details/gxomipjgt.sHtML

[R30] 函数返回状态码
来源：http://wap.vehdjk.com/Article/details/gvldvtgoh.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.bbcook.cn/Article/details/gdtgyrqke.sHtML

[R31] 局部变量
来源：http://read.share.vehdjk.com/Article/details/gekbgminm.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.bbcook.cn/Article/details/gpbrimeou.sHtML

[R32] 参数个数校验
来源：http://blog.epnwcf.com/Article/details/gujayncma.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.tarul.cn/Article/details/gdkariwfj.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.yfazqb.com/Article/details/ghxccjzki.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.yfazqb.com/Article/details/gggsfvwmr.sHtML

[R34] 退出时清理
来源：http://read.share.vehdjk.com/Article/details/gzqocoywv.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fktsv.cn/Article/details/gnqnnfzao.sHtML

[R35] 后台执行并等待
来源：http://blog.tarul.cn/Article/details/gpbwtfjll.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.tarul.cn/Article/details/ghbawtncx.sHtML

[R36] 并发执行多个任务
来源：http://wap.yfazqb.com/Article/details/golqysjhv.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.bbcook.cn/Article/details/ghuuepfeb.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.tarul.cn/Article/details/gxliatoux.sHtML

files=$(ls -1)
来源：http://wap.yfazqb.com/Article/details/gtugdgqor.sHtML

[R38] 管道串联
来源：http://www.blog.yfazqb.com/Article/details/gouunwkga.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.sjlbkw.cn/Article/details/gjwfbwvbn.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.bbcook.cn/Article/details/gnbqmsvuz.sHtML

cmd > out.log 2>&1
来源：http://read.share.yfazqb.com/Article/details/gipnksakj.sHtML

[R40] 追加写日志
来源：http://www.share.bbcook.cn/Article/details/ghcfzfyfb.sHtML

echo "log" >> out.log
来源：http://3g.bbcook.cn/Article/details/grgivzzna.sHtML

[R41] 丢弃输出
来源：http://www.share.vehdjk.com/Article/details/giulcizwr.sHtML

cmd >/dev/null 2>&1
来源：http://3g.fktsv.cn/Article/details/gtkctrafv.sHtML

[R42] 输入重定向
来源：http://baike.fktsv.cn/Article/details/gflfoqptq.sHtML

wc -l < a.txt
来源：http://3g.fktsv.cn/Article/details/gveprtbji.sHtML

[R43] 按名字查找文件
来源：http://mobile.sjlbkw.cn/Article/details/gwxatoksp.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.yfazqb.com/Article/details/gjnnsbbxs.sHtML

[R44] 按修改时间查找
来源：http://www.share.vehdjk.com/Article/details/gmddsyliq.sHtML

find . -mtime -7 -type f
来源：http://blog.fktsv.cn/Article/details/gnezjobva.sHtML

[R45] 批量删除
来源：http://www.share.yfazqb.com/Article/details/ggnwuzzmq.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.sjlbkw.cn/Article/details/guobelqsu.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.vehdjk.com/Article/details/ghoocdiqb.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.tarul.cn/Article/details/guddoxkqs.sHtML

[R47] sed 单行替换
来源：http://mobile.tarul.cn/Article/details/gggnmpyco.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.epnwcf.com/Article/details/glnikamre.sHtML

[R48] awk 取指定列
来源：http://mobile.yfazqb.com/Article/details/gkdvvqxte.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.epnwcf.com/Article/details/gztbceztv.sHtML

[R49] awk 带条件
来源：http://read.share.vehdjk.com/Article/details/gjnzhibmb.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.tarul.cn/Article/details/gnrvtlxma.sHtML

[R50] awk 求和
来源：http://wap.tarul.cn/Article/details/geqotsapr.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.epnwcf.com/Article/details/gowbfxius.sHtML

[R51] 排序去重取前几
来源：http://read.share.fktsv.cn/Article/details/gaouikgiw.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fktsv.cn/Article/details/gegicjifl.sHtML

[R52] 统计行数
来源：http://read.share.bbcook.cn/Article/details/gmazyfdwk.sHtML

wc -l a.txt
来源：http://wap.tarul.cn/Article/details/gywmjwbjs.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.sjlbkw.cn/Article/details/gdmbdaezz.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.tarul.cn/Article/details/glpdgnpsu.sHtML

[R54] 比较两个文件
来源：http://www.blog.yfazqb.com/Article/details/gmjifgccv.sHtML

diff a.txt b.txt
来源：http://wap.yfazqb.com/Article/details/ghctpegbf.sHtML

[R55] 压缩与解压
来源：http://wap.tarul.cn/Article/details/gwazyweja.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.vehdjk.com/Article/details/gmjghuoyo.sHtML

[R56] 远程拷贝
来源：http://mobile.vehdjk.com/Article/details/gdcocebfh.sHtML

scp file user@host:/path/
来源：http://read.share.yfazqb.com/Article/details/gvhjtokdz.sHtML

[R57] 远程执行命令
来源：http://m.share.bbcook.cn/Article/details/gwmjbnrwu.sHtML

ssh user@host 'uptime'
来源：http://www.share.vehdjk.com/Article/details/gcdukmwjw.sHtML

[R58] 下载文件
来源：http://www.blog.yfazqb.com/Article/details/gkbbwrknh.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.fktsv.cn/Article/details/ghfzultav.sHtML

[R59] 发 POST JSON
来源：http://m.share.epnwcf.com/Article/details/gafzxfewd.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.bbcook.cn/Article/details/gbbkdsytw.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.tarul.cn/Article/details/gosuhvayi.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.sjlbkw.cn/Article/details/gitdudxuf.sHtML

[R61] 磁盘占用
来源：http://www.share.epnwcf.com/Article/details/gkccbyihl.sHtML

df -h;  du -sh *
来源：http://www.blog.bbcook.cn/Article/details/grmxqfcsr.sHtML

[R62] 找最占空间的文件
来源：http://wap.sjlbkw.cn/Article/details/grdmskvru.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.sjlbkw.cn/Article/details/getljjsgf.sHtML

[R63] 内存与进程
来源：http://www.share.fktsv.cn/Article/details/gnxxqmwfs.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.vehdjk.com/Article/details/gbuddkgpj.sHtML

[R64] 结束进程
来源：http://wap.vehdjk.com/Article/details/gonusklji.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.epnwcf.com/Article/details/gsgdhjtwn.sHtML

[R65] 查看端口占用
来源：http://3g.bbcook.cn/Article/details/ggdckoiqn.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.epnwcf.com/Article/details/gvfrfslpt.sHtML

[R66] 定时任务
来源：http://read.share.sjlbkw.cn/Article/details/gglzxxqee.sHtML

crontab -e;  crontab -l
来源：http://mobile.sjlbkw.cn/Article/details/gudwygmuo.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.bbcook.cn/Article/details/goxhyjqpr.sHtML

openssl rand -hex 16
来源：http://baike.epnwcf.com/Article/details/glblzszrp.sHtML

[R68] 计算文件校验值
来源：http://wap.sjlbkw.cn/Article/details/gfhpkbgak.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.vehdjk.com/Article/details/gbpcswoff.sHtML

[R69] 生成随机密码
来源：http://blog.bbcook.cn/Article/details/grhjbggwp.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.epnwcf.com/Article/details/ghimhkknc.sHtML

[R70] 时间戳与互转
来源：http://blog.epnwcf.com/Article/details/ggwxrmgky.sHtML

date +%s;  date -d @1700000000
来源：http://wap.yfazqb.com/Article/details/gksmbqubn.sHtML

[R71] 日期格式化
来源：http://m.share.sjlbkw.cn/Article/details/gnjhelhgb.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.epnwcf.com/Article/details/gysxdwkmx.sHtML

[R72] 等待端口就绪
来源：http://m.share.yfazqb.com/Article/details/gphvtzpbq.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fktsv.cn/Article/details/gvnwgicdj.sHtML

[R73] 分割大日志
来源：http://www.share.yfazqb.com/Article/details/gugwtiacg.sHtML

split -l 1000 big.log part_
来源：http://m.share.yfazqb.com/Article/details/gmkhflacw.sHtML

[R74] 批量重命名
来源：http://blog.vehdjk.com/Article/details/gtshevftb.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.tarul.cn/Article/details/gmpgnixmc.sHtML

[R75] 导出环境变量
来源：http://www.m.share.fktsv.cn/Article/details/ggnnnjoae.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.bbcook.cn/Article/details/gdezrwjui.sHtML

[R76] 使用临时文件
来源：http://wap.sjlbkw.cn/Article/details/ghoihfxcy.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.vehdjk.com/Article/details/gfjuohtdo.sHtML

[R77] 读取用户输入
来源：http://baike.tarul.cn/Article/details/gthikexbg.sHtML

read -rp "请输入: " ans
来源：http://baike.epnwcf.com/Article/details/gxtirznxq.sHtML

[R78] 交互式菜单
来源：http://wap.epnwcf.com/Article/details/gjqrvshii.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.epnwcf.com/Article/details/gbovbbske.sHtML

[R79] 解析命令行选项
来源：http://www.share.bbcook.cn/Article/details/gmgsniitx.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.yfazqb.com/Article/details/guqmdwsdk.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.tarul.cn/Article/details/gpdlriijo.sHtML

time ./run.sh
来源：http://blog.tarul.cn/Article/details/ghmlcccyh.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gxssfdnjy.sHtML

S. C / C++ 专题
来源：http://www.share.fktsv.cn/Article/details/gaoakwjpj.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gtowwgjne.sHtML

[S01] C：Hello World
来源：http://baike.bbcook.cn/Article/details/gzinveeye.sHtML

#include <stdio.h>
来源：http://3g.fktsv.cn/Article/details/ggvuuqhiq.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fktsv.cn/Article/details/gwfhfauwc.sHtML

[S02] C：变量与格式化输出
来源：http://3g.yfazqb.com/Article/details/ggkscniqp.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fktsv.cn/Article/details/gqcoiieay.sHtML

[S03] C：读入整数
来源：http://read.share.sjlbkw.cn/Article/details/gtghbtfak.sHtML

int x; scanf("%d", &x);
来源：http://www.share.yfazqb.com/Article/details/glswifmdh.sHtML

[S04] C：字符串复制
来源：http://read.share.vehdjk.com/Article/details/grswrvjwm.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.sjlbkw.cn/Article/details/gkbavksrq.sHtML

[S05] C：字符串长度
来源：http://www.share.vehdjk.com/Article/details/gvbxeszga.sHtML

strlen(s)
来源：http://blog.sjlbkw.cn/Article/details/golscenaq.sHtML

[S06] C：字符串比较
来源：http://mobile.fktsv.cn/Article/details/gvlcmrecv.sHtML

strcmp(a, b) == 0
来源：http://www.blog.yfazqb.com/Article/details/gcetxyjqq.sHtML

[S07] C：数组遍历求和
来源：http://3g.sjlbkw.cn/Article/details/giwjyibbv.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fktsv.cn/Article/details/gincqrgbj.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.vehdjk.com/Article/details/gelcgtuws.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.tarul.cn/Article/details/gaoizesld.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fktsv.cn/Article/details/gctbnyato.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.vehdjk.com/Article/details/gdiizpkph.sHtML

[S10] C：指针与解引用
来源：http://baike.yfazqb.com/Article/details/ghnwflaua.sHtML

int *p = &a;  *p = 5;
来源：http://baike.sjlbkw.cn/Article/details/gkecfajrm.sHtML

[S11] C：逐行读文件
来源：http://baike.tarul.cn/Article/details/gzpavnunb.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.tarul.cn/Article/details/guivnfmiw.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.vehdjk.com/Article/details/gsadxdgvf.sHtML

fclose(f);
来源：http://www.m.share.yfazqb.com/Article/details/gjxjrezcf.sHtML

[S12] C：写文件
来源：http://3g.vehdjk.com/Article/details/gwuppcfks.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.vehdjk.com/Article/details/gathmscba.sHtML

[S13] C：宏定义
来源：http://3g.tarul.cn/Article/details/guyajiucr.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.epnwcf.com/Article/details/gotxebwro.sHtML

[S14] C：枚举
来源：http://blog.bbcook.cn/Article/details/gtuusozti.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.sjlbkw.cn/Article/details/gllvakqdw.sHtML

[S15] C：类型转换
来源：http://baike.yfazqb.com/Article/details/gvrucczfv.sHtML

(double) a / b
来源：http://m.share.bbcook.cn/Article/details/graizzouw.sHtML

[S16] C：位操作置位
来源：http://mobile.bbcook.cn/Article/details/gmdpbmmmx.sHtML

x |= (1 << 3);
来源：http://www.blog.tarul.cn/Article/details/gfuyqtfse.sHtML

[S17] C：安全拼接字符串
来源：http://baike.bbcook.cn/Article/details/gbqnyekix.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.yfazqb.com/Article/details/gxpwrkysy.sHtML

[S18] C：命令行参数
来源：http://wap.tarul.cn/Article/details/gvxkopxta.sHtML

int main(int argc, char **argv)
来源：http://3g.epnwcf.com/Article/details/guucotwlq.sHtML

[S19] C：快速排序
来源：http://blog.fktsv.cn/Article/details/guvydjoot.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fktsv.cn/Article/details/gubqqgnmt.sHtML

[S20] C：二分查找
来源：http://mobile.epnwcf.com/Article/details/gebwrurol.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.tarul.cn/Article/details/gheievlkk.sHtML

[S21] C：字符类别判断
来源：http://wap.sjlbkw.cn/Article/details/gtrpupzvw.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.sjlbkw.cn/Article/details/gvvpmnmeb.sHtML

[S22] C：字符串转数字
来源：http://read.share.bbcook.cn/Article/details/gsqfxoldf.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.vehdjk.com/Article/details/gmqpebgeh.sHtML

[S23] C：随机数
来源：http://www.share.sjlbkw.cn/Article/details/gmjekrpxt.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.epnwcf.com/Article/details/gmficbcrg.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.tarul.cn/Article/details/gtzyyjeda.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.bbcook.cn/Article/details/gqnmwmdls.sHtML

[S25] C：内存拷贝
来源：http://3g.vehdjk.com/Article/details/gjgzceptt.sHtML

memcpy(dst, src, n);
来源：http://read.share.epnwcf.com/Article/details/gzrvfivpf.sHtML

[S26] C：内存清零
来源：http://www.share.epnwcf.com/Article/details/gfanvpyzo.sHtML

memset(a, 0, sizeof a);
来源：http://wap.bbcook.cn/Article/details/gdarhonru.sHtML

[S27] C：定义常量
来源：http://www.share.bbcook.cn/Article/details/gwcsizawk.sHtML

const double PI = 3.14159;
来源：http://m.share.epnwcf.com/Article/details/gpsgiaqye.sHtML

[S28] C：静态变量
来源：http://mobile.epnwcf.com/Article/details/gyigdvhfd.sHtML

static int counter = 0;
来源：http://www.blog.bbcook.cn/Article/details/gbilxnszz.sHtML

[S29] C：变参函数
来源：http://mobile.fktsv.cn/Article/details/gwawmeeml.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.epnwcf.com/Article/details/gkbjysneu.sHtML

[S30] C：头文件保护
来源：http://www.blog.yfazqb.com/Article/details/gjwadthey.sHtML

#ifndef X_H
来源：http://m.share.vehdjk.com/Article/details/gltpdmfyq.sHtML

#define X_H
来源：http://www.share.fktsv.cn/Article/details/gljoqbxah.sHtML

#endif
来源：http://blog.sjlbkw.cn/Article/details/gwwzxripk.sHtML

[S31] C++：Hello World
来源：http://blog.fktsv.cn/Article/details/gkmaboojl.sHtML

#include <iostream>
来源：http://blog.vehdjk.com/Article/details/giljnwbwq.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.yfazqb.com/Article/details/gxbhrovzi.sHtML

[S32] C++：字符串
来源：http://www.m.share.tarul.cn/Article/details/grdpqvxhl.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.vehdjk.com/Article/details/gyrnhszly.sHtML

[S33] C++：vector 增删
来源：http://3g.fktsv.cn/Article/details/gsiuuqruc.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.fktsv.cn/Article/details/ggjgqfgsl.sHtML

[S34] C++：遍历 vector
来源：http://3g.vehdjk.com/Article/details/gcwndtzwi.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fktsv.cn/Article/details/ghbnmvjto.sHtML

[S35] C++：map
来源：http://www.blog.sjlbkw.cn/Article/details/gmhcvvcsf.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.vehdjk.com/Article/details/gwsilllsk.sHtML

[S36] C++：unordered_map
来源：http://blog.tarul.cn/Article/details/gxmpbxayq.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.bbcook.cn/Article/details/geggbfola.sHtML


<!-- 参考信息 -->