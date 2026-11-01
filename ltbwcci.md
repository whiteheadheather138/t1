代发 wailian999

[Q63] 开启事务
来源：http://read.share.yfazqb.com/Article/details/gifdtkjqe.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.sjlbkw.cn/Article/details/gcgfrftng.sHtML

[Q64] 提交事务
来源：http://m.share.fktsv.cn/Article/details/gxljxjihg.sHtML

COMMIT;
来源：http://3g.tarul.cn/Article/details/gkxasozaz.sHtML

[Q65] 回滚事务
来源：http://www.m.share.fktsv.cn/Article/details/gdwudanhe.sHtML

ROLLBACK;
来源：http://www.blog.vehdjk.com/Article/details/gcthaujlv.sHtML

[Q66] 行锁查询
来源：http://wap.epnwcf.com/Article/details/gkcqezcdg.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.yfazqb.com/Article/details/gtnczrxvi.sHtML

[Q67] 设置隔离级别
来源：http://mobile.sjlbkw.cn/Article/details/geoddrsht.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.vehdjk.com/Article/details/gfmmcoldc.sHtML

[Q68] 保存点
来源：http://www.blog.sjlbkw.cn/Article/details/getweiona.sHtML

SAVEPOINT sp1;
来源：http://mobile.tarul.cn/Article/details/gdbioyjno.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.epnwcf.com/Article/details/gkyqhumwb.sHtML

[Q69] 查看执行计划
来源：http://m.share.bbcook.cn/Article/details/gqhhesupo.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.epnwcf.com/Article/details/gsyvbosql.sHtML

[Q70] 更新统计信息
来源：http://mobile.vehdjk.com/Article/details/ggjnegrzw.sHtML

ANALYZE TABLE users;
来源：http://wap.yfazqb.com/Article/details/gahamotmk.sHtML

[Q71] 查看建表语句
来源：http://www.blog.tarul.cn/Article/details/giubhqpin.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.tarul.cn/Article/details/gaspelpxv.sHtML

[Q72] 查看索引
来源：http://read.share.bbcook.cn/Article/details/gfattrezf.sHtML

SHOW INDEX FROM users;
来源：http://mobile.epnwcf.com/Article/details/gqmozufmk.sHtML

[Q73] 查看表状态
来源：http://www.m.share.yfazqb.com/Article/details/gfqvscynb.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.sjlbkw.cn/Article/details/gdrpbqygg.sHtML

[Q74] 强制使用索引
来源：http://m.share.vehdjk.com/Article/details/gwqpvsbte.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.epnwcf.com/Article/details/gmtxuayay.sHtML

[Q75] 日期格式化
来源：http://3g.tarul.cn/Article/details/gjszqrfqt.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.fktsv.cn/Article/details/gcqkwquxk.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.sjlbkw.cn/Article/details/gwrrkquuq.sHtML

[Q76] 按天统计
来源：http://www.m.share.fktsv.cn/Article/details/gjyvpsizt.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.tarul.cn/Article/details/guzfqnbhk.sHtML

[Q77] 时间加减
来源：http://3g.fktsv.cn/Article/details/ggdufmlzw.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.epnwcf.com/Article/details/gphudjqec.sHtML

[Q78] 当前时间
来源：http://www.blog.tarul.cn/Article/details/gxsfchwgx.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.yfazqb.com/Article/details/ghtgeuojo.sHtML

[Q79] 字符串拼接
来源：http://www.blog.epnwcf.com/Article/details/ggjywmoru.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.fktsv.cn/Article/details/gaxwnhygu.sHtML

[Q80] 字符串截取
来源：http://blog.fktsv.cn/Article/details/geazwsjfb.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.epnwcf.com/Article/details/gwchxuwar.sHtML

[Q81] 字符串替换
来源：http://3g.yfazqb.com/Article/details/gjlsckujb.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.epnwcf.com/Article/details/giaballuw.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.fktsv.cn/Article/details/gsysqyfqb.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.epnwcf.com/Article/details/gdvvzxyvs.sHtML

[Q83] 大小写转换
来源：http://wap.vehdjk.com/Article/details/gcxlsxoyh.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.bbcook.cn/Article/details/gfphijich.sHtML

[Q84] 去除首尾空格
来源：http://wap.fktsv.cn/Article/details/gmhzkaxot.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.epnwcf.com/Article/details/getdiejxv.sHtML

[Q85] 数值取整
来源：http://www.share.sjlbkw.cn/Article/details/glloieruk.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.bbcook.cn/Article/details/gcxicovok.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.bbcook.cn/Article/details/ghibitzsc.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.vehdjk.com/Article/details/gimtrnkmp.sHtML

[Q87] JSON 字段做条件
来源：http://blog.fktsv.cn/Article/details/gsiusfmdw.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.epnwcf.com/Article/details/gthjhflqj.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.fktsv.cn/Article/details/groexcimk.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.fktsv.cn/Article/details/gqsmnblrz.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.bbcook.cn/Article/details/gqmuylzgt.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.sjlbkw.cn/Article/details/gtaqlcfhb.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.tarul.cn/Article/details/gethcvhtz.sHtML

[Q90] 生成序号列
来源：http://www.blog.tarul.cn/Article/details/gphshftas.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.vehdjk.com/Article/details/gvawozpbt.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gcakcpuko.sHtML

R. Bash 专题
来源：http://read.share.bbcook.cn/Article/details/gaadtrdvn.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gkvzrgnoo.sHtML

[R01] shebang 与严格模式
来源：http://baike.tarul.cn/Article/details/goxhnvexq.sHtML

#!/usr/bin/env bash
来源：http://read.share.sjlbkw.cn/Article/details/gspiddiae.sHtML

set -euo pipefail
来源：http://mobile.tarul.cn/Article/details/gpuzoqnqz.sHtML

[R02] 变量赋值与使用
来源：http://3g.tarul.cn/Article/details/gfgmljxtd.sHtML

name="Tom"; echo "$name"
来源：http://read.share.vehdjk.com/Article/details/gdnupiyuv.sHtML

[R03] 只读变量
来源：http://www.m.share.vehdjk.com/Article/details/gjvpxksnk.sHtML

readonly PI=3.14
来源：http://mobile.yfazqb.com/Article/details/gdheyrgej.sHtML

[R04] 位置参数
来源：http://m.share.vehdjk.com/Article/details/gvjtgxzzv.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.sjlbkw.cn/Article/details/gxqbgcxbq.sHtML

[R05] 参数默认值
来源：http://read.share.fktsv.cn/Article/details/gaqqlofah.sHtML

name="${1:-default}"
来源：http://www.blog.tarul.cn/Article/details/gqgmhguyt.sHtML

[R06] 判断命令是否存在
来源：http://www.share.bbcook.cn/Article/details/ghxulkyzh.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.sjlbkw.cn/Article/details/glfkpllne.sHtML

[R07] if 判断文件
来源：http://m.share.epnwcf.com/Article/details/gdpuebxna.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.bbcook.cn/Article/details/glvygziac.sHtML

[R08] 数值比较
来源：http://wap.tarul.cn/Article/details/gthdrjijr.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.epnwcf.com/Article/details/gqyjljyau.sHtML

[R09] 字符串比较
来源：http://www.m.share.sjlbkw.cn/Article/details/gcxzldtxj.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.epnwcf.com/Article/details/gxvemoulm.sHtML

[R10] 正则匹配
来源：http://blog.yfazqb.com/Article/details/gkqvxgkgv.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.fktsv.cn/Article/details/gmxkrjcop.sHtML

[R11] case 多分支
来源：http://read.share.sjlbkw.cn/Article/details/ghmwpdwnw.sHtML

case "$1" in
来源：http://m.share.sjlbkw.cn/Article/details/grunjmiyp.sHtML

start) echo "启动" ;;
来源：http://www.blog.tarul.cn/Article/details/gwwljypek.sHtML

stop)  echo "停止" ;;
来源：http://mobile.fktsv.cn/Article/details/gqrebqsrd.sHtML

*)     echo "未知命令" ;;
来源：http://3g.sjlbkw.cn/Article/details/gnwthpcoq.sHtML

esac
来源：http://www.m.share.sjlbkw.cn/Article/details/gufbmtiio.sHtML

[R12] for 遍历文件
来源：http://3g.fktsv.cn/Article/details/gxcgcdjtl.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.epnwcf.com/Article/details/grtzoxmhj.sHtML

[R13] for 计数循环
来源：http://mobile.vehdjk.com/Article/details/grzzighks.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.fktsv.cn/Article/details/gasgfazyb.sHtML

[R14] C 风格 for
来源：http://www.m.share.sjlbkw.cn/Article/details/gzqrhlvcw.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.bbcook.cn/Article/details/gqrsjsmtz.sHtML

[R15] while 逐行读文件
来源：http://www.blog.yfazqb.com/Article/details/gfsdqknbk.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.bbcook.cn/Article/details/gfvzzbmht.sHtML

[R16] until 等待条件
来源：http://m.share.yfazqb.com/Article/details/gfcgwrfoc.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.sjlbkw.cn/Article/details/gtmlvovlk.sHtML

[R17] 数组定义与取值
来源：http://blog.sjlbkw.cn/Article/details/gtrpnstzh.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.sjlbkw.cn/Article/details/gonwpzifj.sHtML

[R18] 遍历数组
来源：http://www.share.fktsv.cn/Article/details/gaecubpnt.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.vehdjk.com/Article/details/gshuysjgm.sHtML

[R19] 数组长度
来源：http://read.share.tarul.cn/Article/details/giqmsqpun.sHtML

echo "${#arr[@]}"
来源：http://www.blog.sjlbkw.cn/Article/details/gtrylbcba.sHtML

[R20] 关联数组（字典）
来源：http://wap.sjlbkw.cn/Article/details/gvkecbtxp.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.vehdjk.com/Article/details/gjxhltkld.sHtML

[R21] 字符串长度
来源：http://wap.fktsv.cn/Article/details/gepcciwzg.sHtML

echo "${#s}"
来源：http://www.blog.sjlbkw.cn/Article/details/giqvlgxhg.sHtML

[R22] 截取子串
来源：http://www.blog.epnwcf.com/Article/details/gybryiiii.sHtML

echo "${s:0:5}"
来源：http://www.m.share.bbcook.cn/Article/details/grikbmhej.sHtML

[R23] 字符串替换
来源：http://baike.vehdjk.com/Article/details/gtpjnvqhc.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.bbcook.cn/Article/details/gauwiymqj.sHtML

[R24] 大小写转换
来源：http://read.share.sjlbkw.cn/Article/details/gfzazwley.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.yfazqb.com/Article/details/gdcjzverk.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.yfazqb.com/Article/details/gbwpufgki.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.vehdjk.com/Article/details/gpjdtfews.sHtML

[R26] 命令替换
来源：http://wap.epnwcf.com/Article/details/gtlycfjub.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.bbcook.cn/Article/details/gfrxiivjm.sHtML

[R27] 算术展开
来源：http://baike.vehdjk.com/Article/details/geifceukt.sHtML

echo $((1 + 2 * 3))
来源：http://3g.epnwcf.com/Article/details/gsozeigtc.sHtML

[R28] 浮点运算
来源：http://www.share.bbcook.cn/Article/details/ggzkounrw.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.epnwcf.com/Article/details/gzziqnkut.sHtML

[R29] 定义函数
来源：http://www.blog.sjlbkw.cn/Article/details/gzyqbkcfk.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.tarul.cn/Article/details/gbgsagccu.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.yfazqb.com/Article/details/gkxglkvba.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.tarul.cn/Article/details/ghuoqhyzn.sHtML

[R31] 局部变量
来源：http://wap.epnwcf.com/Article/details/gsgdjxexa.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.fktsv.cn/Article/details/ggqxtyqvr.sHtML

[R32] 参数个数校验
来源：http://www.m.share.bbcook.cn/Article/details/gfmnginjy.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.bbcook.cn/Article/details/gvlylckgm.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.tarul.cn/Article/details/gesjsbfbi.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.tarul.cn/Article/details/garaukcbd.sHtML

[R34] 退出时清理
来源：http://mobile.tarul.cn/Article/details/guigmxvzb.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.bbcook.cn/Article/details/gwznfevoq.sHtML

[R35] 后台执行并等待
来源：http://mobile.sjlbkw.cn/Article/details/gvalfjsmc.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fktsv.cn/Article/details/gahotwrlf.sHtML

[R36] 并发执行多个任务
来源：http://m.share.fktsv.cn/Article/details/gbdpvkcxa.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.bbcook.cn/Article/details/gaiywwvtc.sHtML

[R37] 把输出赋给变量
来源：http://3g.tarul.cn/Article/details/gubybthax.sHtML

files=$(ls -1)
来源：http://baike.yfazqb.com/Article/details/gdjmhscea.sHtML

[R38] 管道串联
来源：http://baike.epnwcf.com/Article/details/gpmcypcjs.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.epnwcf.com/Article/details/gtmefynlj.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.sjlbkw.cn/Article/details/gxhjnfcme.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.vehdjk.com/Article/details/gbpqfwjuy.sHtML

[R40] 追加写日志
来源：http://www.share.tarul.cn/Article/details/gscevuaws.sHtML

echo "log" >> out.log
来源：http://3g.yfazqb.com/Article/details/gwqclfaxp.sHtML

[R41] 丢弃输出
来源：http://baike.epnwcf.com/Article/details/gpjcceibz.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.epnwcf.com/Article/details/glzwzcocq.sHtML

[R42] 输入重定向
来源：http://www.m.share.fktsv.cn/Article/details/gvghbfhyk.sHtML

wc -l < a.txt
来源：http://m.share.fktsv.cn/Article/details/gihnlvxbf.sHtML

[R43] 按名字查找文件
来源：http://3g.sjlbkw.cn/Article/details/gynezqfst.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.yfazqb.com/Article/details/gznerfnyg.sHtML

[R44] 按修改时间查找
来源：http://blog.fktsv.cn/Article/details/gifmfzoim.sHtML

find . -mtime -7 -type f
来源：http://blog.bbcook.cn/Article/details/gavdiaoxp.sHtML

[R45] 批量删除
来源：http://blog.tarul.cn/Article/details/goywzlmhl.sHtML

find . -name "*.tmp" -delete
来源：http://blog.yfazqb.com/Article/details/gjzzofrkl.sHtML

[R46] 递归替换文件内容
来源：http://www.share.sjlbkw.cn/Article/details/ggyedgmko.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.tarul.cn/Article/details/gxzoykrkw.sHtML

[R47] sed 单行替换
来源：http://mobile.sjlbkw.cn/Article/details/gmpdxusfp.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.yfazqb.com/Article/details/gomhmodcu.sHtML

[R48] awk 取指定列
来源：http://wap.vehdjk.com/Article/details/ghhbbvzcw.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.bbcook.cn/Article/details/gattawlxm.sHtML

[R49] awk 带条件
来源：http://m.share.epnwcf.com/Article/details/gfzkjrgdr.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.epnwcf.com/Article/details/gxprcmjbm.sHtML

[R50] awk 求和
来源：http://read.share.sjlbkw.cn/Article/details/gnrjgqpmo.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.tarul.cn/Article/details/gejpsobde.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.epnwcf.com/Article/details/gefcxkste.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.vehdjk.com/Article/details/gqihsxkqw.sHtML

[R52] 统计行数
来源：http://m.share.yfazqb.com/Article/details/gvjxvzvgx.sHtML

wc -l a.txt
来源：http://blog.fktsv.cn/Article/details/gdszudows.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.sjlbkw.cn/Article/details/gjlaunyol.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.tarul.cn/Article/details/gbjuypbbg.sHtML

[R54] 比较两个文件
来源：http://read.share.yfazqb.com/Article/details/gbpbsjdrb.sHtML

diff a.txt b.txt
来源：http://www.blog.tarul.cn/Article/details/gqpiubztq.sHtML

[R55] 压缩与解压
来源：http://www.m.share.tarul.cn/Article/details/gxkcedkpp.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fktsv.cn/Article/details/guqfubvnw.sHtML

[R56] 远程拷贝
来源：http://baike.yfazqb.com/Article/details/grttyfeos.sHtML

scp file user@host:/path/
来源：http://m.share.yfazqb.com/Article/details/ggfeskdbb.sHtML

[R57] 远程执行命令
来源：http://blog.bbcook.cn/Article/details/gqavrvter.sHtML

ssh user@host 'uptime'
来源：http://mobile.vehdjk.com/Article/details/gzwhewowu.sHtML

[R58] 下载文件
来源：http://blog.yfazqb.com/Article/details/gvrygwejo.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.epnwcf.com/Article/details/grcuakdfs.sHtML

[R59] 发 POST JSON
来源：http://blog.sjlbkw.cn/Article/details/gccqrgxes.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.vehdjk.com/Article/details/gjtddppau.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fktsv.cn/Article/details/gcjxcpetd.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.yfazqb.com/Article/details/gqqqgtkod.sHtML

[R61] 磁盘占用
来源：http://m.share.tarul.cn/Article/details/gomuupaby.sHtML

df -h;  du -sh *
来源：http://blog.sjlbkw.cn/Article/details/gnmqddzfg.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.tarul.cn/Article/details/gwotddnln.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.vehdjk.com/Article/details/gplmfraqp.sHtML

[R63] 内存与进程
来源：http://baike.epnwcf.com/Article/details/gneqhfamr.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.fktsv.cn/Article/details/guqcgkbon.sHtML

[R64] 结束进程
来源：http://www.blog.bbcook.cn/Article/details/gttqmafgp.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.yfazqb.com/Article/details/gnkcceueq.sHtML

[R65] 查看端口占用
来源：http://baike.fktsv.cn/Article/details/gsferzryf.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.fktsv.cn/Article/details/gxqjiiqsm.sHtML

[R66] 定时任务
来源：http://read.share.yfazqb.com/Article/details/gpmoyisvg.sHtML

crontab -e;  crontab -l
来源：http://read.share.vehdjk.com/Article/details/gkqqqznqm.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.vehdjk.com/Article/details/grispzwzz.sHtML

openssl rand -hex 16
来源：http://m.share.yfazqb.com/Article/details/gtneaqsjn.sHtML

[R68] 计算文件校验值
来源：http://www.blog.epnwcf.com/Article/details/gjbknqxfe.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.vehdjk.com/Article/details/gsjodaqmx.sHtML

[R69] 生成随机密码
来源：http://read.share.bbcook.cn/Article/details/ghlkbkqqx.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.fktsv.cn/Article/details/gcuslxgzl.sHtML

[R70] 时间戳与互转
来源：http://read.share.vehdjk.com/Article/details/gklngbezd.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.bbcook.cn/Article/details/gvvziivxt.sHtML

[R71] 日期格式化
来源：http://read.share.fktsv.cn/Article/details/glwmhuciv.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fktsv.cn/Article/details/gytvsepac.sHtML

[R72] 等待端口就绪
来源：http://www.blog.yfazqb.com/Article/details/gvpbxepfp.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.epnwcf.com/Article/details/gdmomyjau.sHtML

[R73] 分割大日志
来源：http://blog.fktsv.cn/Article/details/ghczxofvz.sHtML

split -l 1000 big.log part_
来源：http://wap.tarul.cn/Article/details/gqlccvfsw.sHtML

[R74] 批量重命名
来源：http://m.share.epnwcf.com/Article/details/gpgqawzrv.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.tarul.cn/Article/details/gqrhwuiaw.sHtML

[R75] 导出环境变量
来源：http://www.share.fktsv.cn/Article/details/giypmdfmd.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.sjlbkw.cn/Article/details/gheuowoxv.sHtML

[R76] 使用临时文件
来源：http://blog.sjlbkw.cn/Article/details/gggysspmw.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fktsv.cn/Article/details/gdzdlgobl.sHtML

[R77] 读取用户输入
来源：http://www.blog.epnwcf.com/Article/details/gzhtklvpa.sHtML

read -rp "请输入: " ans
来源：http://3g.fktsv.cn/Article/details/gxxvbkkhz.sHtML

[R78] 交互式菜单
来源：http://m.share.fktsv.cn/Article/details/gycxctmcu.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.bbcook.cn/Article/details/gpbvkggca.sHtML

[R79] 解析命令行选项
来源：http://3g.yfazqb.com/Article/details/gjsmnrfuz.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.yfazqb.com/Article/details/gjmwcypsh.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.sjlbkw.cn/Article/details/ggvcyktgq.sHtML

time ./run.sh
来源：http://3g.sjlbkw.cn/Article/details/goyueolkp.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gxyizcxqh.sHtML

S. C / C++ 专题
来源：http://wap.vehdjk.com/Article/details/gqelqtydz.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/glinixssl.sHtML

[S01] C：Hello World
来源：http://www.blog.vehdjk.com/Article/details/gvvoformk.sHtML

#include <stdio.h>
来源：http://blog.vehdjk.com/Article/details/gkbzijkdh.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.yfazqb.com/Article/details/gxsigcuqa.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fktsv.cn/Article/details/gxeqmkmnw.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.epnwcf.com/Article/details/gidumbdsb.sHtML

[S03] C：读入整数
来源：http://3g.epnwcf.com/Article/details/ghhkocbmy.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.epnwcf.com/Article/details/gtdzniula.sHtML

[S04] C：字符串复制
来源：http://m.share.vehdjk.com/Article/details/gfnzjnaqb.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.epnwcf.com/Article/details/grgncnqes.sHtML

[S05] C：字符串长度
来源：http://3g.sjlbkw.cn/Article/details/geqrmabih.sHtML

strlen(s)
来源：http://www.m.share.bbcook.cn/Article/details/gfubkkdtv.sHtML

[S06] C：字符串比较
来源：http://blog.tarul.cn/Article/details/glfjgwmbx.sHtML

strcmp(a, b) == 0
来源：http://m.share.sjlbkw.cn/Article/details/gpbpsjojk.sHtML

[S07] C：数组遍历求和
来源：http://m.share.yfazqb.com/Article/details/gordoteaj.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.sjlbkw.cn/Article/details/gtddfaptj.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.yfazqb.com/Article/details/gwxvpgxcm.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fktsv.cn/Article/details/gvpnpswhn.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.tarul.cn/Article/details/giinhpqtr.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.tarul.cn/Article/details/gclbdawrt.sHtML

[S10] C：指针与解引用
来源：http://blog.fktsv.cn/Article/details/gqkwfpwgw.sHtML

int *p = &a;  *p = 5;
来源：http://wap.sjlbkw.cn/Article/details/gsfxftmkv.sHtML

[S11] C：逐行读文件
来源：http://blog.epnwcf.com/Article/details/geeltxrzd.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.vehdjk.com/Article/details/gudkniutc.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.bbcook.cn/Article/details/girgvoool.sHtML

fclose(f);
来源：http://3g.bbcook.cn/Article/details/gjvlrgpor.sHtML

[S12] C：写文件
来源：http://www.m.share.fktsv.cn/Article/details/glrjsfnro.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.tarul.cn/Article/details/grippuekv.sHtML

[S13] C：宏定义
来源：http://www.share.sjlbkw.cn/Article/details/grfevrfld.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.bbcook.cn/Article/details/gtjbevwft.sHtML

[S14] C：枚举
来源：http://www.blog.sjlbkw.cn/Article/details/gqnmsdegr.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.sjlbkw.cn/Article/details/gbnnngmcu.sHtML

[S15] C：类型转换
来源：http://www.m.share.fktsv.cn/Article/details/gcvlfrwyq.sHtML

(double) a / b
来源：http://www.m.share.bbcook.cn/Article/details/gtnzkuspe.sHtML

[S16] C：位操作置位
来源：http://m.share.tarul.cn/Article/details/gsmluhdlv.sHtML

x |= (1 << 3);
来源：http://blog.bbcook.cn/Article/details/gepsaotfk.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.vehdjk.com/Article/details/gigknpscl.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.fktsv.cn/Article/details/gmxvjsjth.sHtML

[S18] C：命令行参数
来源：http://m.share.vehdjk.com/Article/details/gtkedicln.sHtML

int main(int argc, char **argv)
来源：http://mobile.vehdjk.com/Article/details/gwpikhzno.sHtML

[S19] C：快速排序
来源：http://www.share.epnwcf.com/Article/details/gdgwovhxy.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.bbcook.cn/Article/details/glgcrmjxz.sHtML

[S20] C：二分查找
来源：http://www.blog.epnwcf.com/Article/details/ghhekvdxy.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.vehdjk.com/Article/details/gjgnyunuk.sHtML

[S21] C：字符类别判断
来源：http://www.share.tarul.cn/Article/details/ghldgggix.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.sjlbkw.cn/Article/details/gnzzftgck.sHtML

[S22] C：字符串转数字
来源：http://blog.yfazqb.com/Article/details/gxhczakmy.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.vehdjk.com/Article/details/gkemyjmow.sHtML

[S23] C：随机数
来源：http://mobile.tarul.cn/Article/details/gmlwnyrqe.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.yfazqb.com/Article/details/gnmqkkyyh.sHtML

[S24] C：获取本地时间
来源：http://m.share.vehdjk.com/Article/details/gbvivgwib.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fktsv.cn/Article/details/gpnfpnquw.sHtML

[S25] C：内存拷贝
来源：http://wap.tarul.cn/Article/details/ghxnsfygr.sHtML

memcpy(dst, src, n);
来源：http://3g.bbcook.cn/Article/details/grjtuivlq.sHtML

[S26] C：内存清零
来源：http://3g.yfazqb.com/Article/details/gnqqsdjvm.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.sjlbkw.cn/Article/details/gllfpbyjc.sHtML

[S27] C：定义常量
来源：http://www.m.share.sjlbkw.cn/Article/details/gjjcrbgev.sHtML

const double PI = 3.14159;
来源：http://read.share.fktsv.cn/Article/details/guhxjxiqr.sHtML

[S28] C：静态变量
来源：http://blog.yfazqb.com/Article/details/gicvmcwnv.sHtML

static int counter = 0;
来源：http://www.blog.bbcook.cn/Article/details/gulamryce.sHtML

[S29] C：变参函数
来源：http://m.share.yfazqb.com/Article/details/gmvktrtos.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.tarul.cn/Article/details/gibvibsnf.sHtML

[S30] C：头文件保护
来源：http://read.share.tarul.cn/Article/details/grvacbitt.sHtML

#ifndef X_H
来源：http://read.share.yfazqb.com/Article/details/gbamfvtmv.sHtML

#define X_H
来源：http://www.share.tarul.cn/Article/details/gvnpbxhdv.sHtML

#endif
来源：http://www.share.tarul.cn/Article/details/gtrrdrojg.sHtML

[S31] C++：Hello World
来源：http://www.blog.tarul.cn/Article/details/gehsmzmcd.sHtML

#include <iostream>
来源：http://m.share.epnwcf.com/Article/details/gigwqlpnl.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.vehdjk.com/Article/details/gnjadytel.sHtML

[S32] C++：字符串
来源：http://3g.yfazqb.com/Article/details/giwotmspy.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.vehdjk.com/Article/details/gdnxxxvqq.sHtML


<!-- 参考信息 -->