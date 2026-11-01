代发 wailian999

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.vehdjk.com/Article/details/gfcfvqhrh.sHtML

[Q54] 清空表
来源：http://wap.epnwcf.com/Article/details/gdaosborf.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.tarul.cn/Article/details/ghdrvorob.sHtML

[Q55] 排名（并列占位）
来源：http://wap.epnwcf.com/Article/details/gcxdxduqb.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.epnwcf.com/Article/details/gbrsnudby.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.tarul.cn/Article/details/glyzekpdl.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.tarul.cn/Article/details/gkpeylhqi.sHtML

[Q57] 行号
来源：http://m.share.epnwcf.com/Article/details/gfxyxggte.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.fktsv.cn/Article/details/gststflzj.sHtML

[Q58] 累计求和
来源：http://read.share.yfazqb.com/Article/details/gdyzqiwmg.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.fktsv.cn/Article/details/gmpzfapeb.sHtML

[Q59] 分组内累计
来源：http://m.share.sjlbkw.cn/Article/details/gaxwtflws.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.fktsv.cn/Article/details/gmtwxntau.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.bbcook.cn/Article/details/gtllgnzrj.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.fktsv.cn/Article/details/gqtdnqtnb.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.bbcook.cn/Article/details/gsstpokfh.sHtML

[Q61] 移动平均
来源：http://3g.tarul.cn/Article/details/gcjxgkfjz.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.sjlbkw.cn/Article/details/gvrgtltmi.sHtML

[Q62] 分组占比
来源：http://mobile.vehdjk.com/Article/details/ghvcbayuy.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.tarul.cn/Article/details/gxcqbulgv.sHtML

[Q63] 开启事务
来源：http://blog.tarul.cn/Article/details/gigbkwpai.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.vehdjk.com/Article/details/gomknzsga.sHtML

[Q64] 提交事务
来源：http://www.share.tarul.cn/Article/details/gteoyoiwf.sHtML

COMMIT;
来源：http://mobile.tarul.cn/Article/details/gbvxgapla.sHtML

[Q65] 回滚事务
来源：http://baike.epnwcf.com/Article/details/gnuogjhja.sHtML

ROLLBACK;
来源：http://blog.sjlbkw.cn/Article/details/gyqxzpqou.sHtML

[Q66] 行锁查询
来源：http://www.share.vehdjk.com/Article/details/giisbefru.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.bbcook.cn/Article/details/gnexrggyx.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.vehdjk.com/Article/details/gdzlddqdb.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.sjlbkw.cn/Article/details/gmqgnomtu.sHtML

[Q68] 保存点
来源：http://www.share.tarul.cn/Article/details/ggriixjqc.sHtML

SAVEPOINT sp1;
来源：http://blog.bbcook.cn/Article/details/galftgrmz.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.vehdjk.com/Article/details/gtcxyqgmv.sHtML

[Q69] 查看执行计划
来源：http://read.share.epnwcf.com/Article/details/gkadebmgk.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.vehdjk.com/Article/details/gizdkflog.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.bbcook.cn/Article/details/gbnreoflf.sHtML

ANALYZE TABLE users;
来源：http://wap.epnwcf.com/Article/details/gdmsjfgmf.sHtML

[Q71] 查看建表语句
来源：http://mobile.fktsv.cn/Article/details/gcfsmobja.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.epnwcf.com/Article/details/gwxikzwqz.sHtML

[Q72] 查看索引
来源：http://3g.sjlbkw.cn/Article/details/gxwelptdw.sHtML

SHOW INDEX FROM users;
来源：http://baike.bbcook.cn/Article/details/gozsslotr.sHtML

[Q73] 查看表状态
来源：http://wap.yfazqb.com/Article/details/gjlffsjjp.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.bbcook.cn/Article/details/gaqkdmyvu.sHtML

[Q74] 强制使用索引
来源：http://3g.tarul.cn/Article/details/gndcwfhip.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.bbcook.cn/Article/details/gcmnhdzjg.sHtML

[Q75] 日期格式化
来源：http://wap.yfazqb.com/Article/details/gkmhkomlk.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.vehdjk.com/Article/details/giojbjpai.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.bbcook.cn/Article/details/gpaiycqxw.sHtML

[Q76] 按天统计
来源：http://blog.fktsv.cn/Article/details/gccfvudmk.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.fktsv.cn/Article/details/gvpgtsqbo.sHtML

[Q77] 时间加减
来源：http://read.share.sjlbkw.cn/Article/details/gqqzzekre.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.yfazqb.com/Article/details/gqinprvsx.sHtML

[Q78] 当前时间
来源：http://www.share.tarul.cn/Article/details/ghgjtwlww.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.yfazqb.com/Article/details/gczbeocfq.sHtML

[Q79] 字符串拼接
来源：http://baike.sjlbkw.cn/Article/details/glhxrzewj.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.bbcook.cn/Article/details/gzrxzswum.sHtML

[Q80] 字符串截取
来源：http://wap.yfazqb.com/Article/details/grxzcsygo.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.tarul.cn/Article/details/gsjjhdecb.sHtML

[Q81] 字符串替换
来源：http://blog.vehdjk.com/Article/details/gfscqmnog.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.tarul.cn/Article/details/ggrkqodaz.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.yfazqb.com/Article/details/gwdlapvvo.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.yfazqb.com/Article/details/godvmlvdv.sHtML

[Q83] 大小写转换
来源：http://baike.yfazqb.com/Article/details/gcoxfmcmd.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.bbcook.cn/Article/details/grvqeckao.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.epnwcf.com/Article/details/gmwrxpqpu.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.epnwcf.com/Article/details/gsmgkfmuz.sHtML

[Q85] 数值取整
来源：http://wap.vehdjk.com/Article/details/gpykawjao.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.vehdjk.com/Article/details/gwuqchwtz.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.sjlbkw.cn/Article/details/getvszgvg.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.epnwcf.com/Article/details/grfxupsvp.sHtML

[Q87] JSON 字段做条件
来源：http://baike.vehdjk.com/Article/details/gpmyyxvci.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.bbcook.cn/Article/details/gvcrjjkrd.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.epnwcf.com/Article/details/gvexzmtus.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.fktsv.cn/Article/details/gzhjvnwvr.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.epnwcf.com/Article/details/gfmstaull.sHtML

[Q89] 判断表是否存在
来源：http://3g.epnwcf.com/Article/details/gmgkpxswm.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.vehdjk.com/Article/details/gksqmzsta.sHtML

[Q90] 生成序号列
来源：http://read.share.tarul.cn/Article/details/gyndwnacf.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.sjlbkw.cn/Article/details/grswbvjbl.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gbqoqpafz.sHtML

R. Bash 专题
来源：http://3g.yfazqb.com/Article/details/gfnasaici.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gfxffcpof.sHtML

[R01] shebang 与严格模式
来源：http://m.share.yfazqb.com/Article/details/gtnqktyog.sHtML

#!/usr/bin/env bash
来源：http://www.share.tarul.cn/Article/details/gjxzkrsmx.sHtML

set -euo pipefail
来源：http://www.m.share.sjlbkw.cn/Article/details/gvvvbgssv.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.bbcook.cn/Article/details/gmhjstqxy.sHtML

name="Tom"; echo "$name"
来源：http://www.share.bbcook.cn/Article/details/garsqkjoq.sHtML

[R03] 只读变量
来源：http://mobile.yfazqb.com/Article/details/gonckspcd.sHtML

readonly PI=3.14
来源：http://baike.yfazqb.com/Article/details/gxewarfpg.sHtML

[R04] 位置参数
来源：http://3g.sjlbkw.cn/Article/details/ghzixxlgc.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.fktsv.cn/Article/details/gpairzawq.sHtML

[R05] 参数默认值
来源：http://read.share.tarul.cn/Article/details/gliniayet.sHtML

name="${1:-default}"
来源：http://www.m.share.sjlbkw.cn/Article/details/giqtvcrim.sHtML

[R06] 判断命令是否存在
来源：http://blog.bbcook.cn/Article/details/gwtwbmdqp.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.sjlbkw.cn/Article/details/gfonyyzwz.sHtML

[R07] if 判断文件
来源：http://www.blog.epnwcf.com/Article/details/gwkeocyeq.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.vehdjk.com/Article/details/gpdncbrdv.sHtML

[R08] 数值比较
来源：http://mobile.yfazqb.com/Article/details/gvswsttdd.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.bbcook.cn/Article/details/gzefkgsra.sHtML

[R09] 字符串比较
来源：http://m.share.tarul.cn/Article/details/gmcjlciej.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.tarul.cn/Article/details/ghvtrbpgt.sHtML

[R10] 正则匹配
来源：http://baike.bbcook.cn/Article/details/gfbzofpwj.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.fktsv.cn/Article/details/gmmenwanl.sHtML

[R11] case 多分支
来源：http://www.m.share.fktsv.cn/Article/details/gidebdvwd.sHtML

case "$1" in
来源：http://mobile.sjlbkw.cn/Article/details/gwufekdqf.sHtML

start) echo "启动" ;;
来源：http://read.share.sjlbkw.cn/Article/details/gwldifbqn.sHtML

stop)  echo "停止" ;;
来源：http://www.share.sjlbkw.cn/Article/details/gaeqxkokz.sHtML

*)     echo "未知命令" ;;
来源：http://3g.bbcook.cn/Article/details/ghyzxpxcb.sHtML

esac
来源：http://wap.yfazqb.com/Article/details/gxbwdqkmg.sHtML

[R12] for 遍历文件
来源：http://baike.epnwcf.com/Article/details/grtrtfubd.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.vehdjk.com/Article/details/gbyhkktlw.sHtML

[R13] for 计数循环
来源：http://baike.sjlbkw.cn/Article/details/ghmbxtpxd.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.bbcook.cn/Article/details/gbvqzuequ.sHtML

[R14] C 风格 for
来源：http://www.share.fktsv.cn/Article/details/gopyjagyo.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.bbcook.cn/Article/details/gausfujvd.sHtML

[R15] while 逐行读文件
来源：http://www.share.fktsv.cn/Article/details/gaeoonvvh.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.bbcook.cn/Article/details/gjnymtziq.sHtML

[R16] until 等待条件
来源：http://blog.sjlbkw.cn/Article/details/gabdqaftw.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.vehdjk.com/Article/details/gdzkvkepw.sHtML

[R17] 数组定义与取值
来源：http://mobile.tarul.cn/Article/details/gmkjzupjl.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.yfazqb.com/Article/details/gquyljnbx.sHtML

[R18] 遍历数组
来源：http://m.share.fktsv.cn/Article/details/gejtsyohv.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.sjlbkw.cn/Article/details/gyzhbspzo.sHtML

[R19] 数组长度
来源：http://read.share.epnwcf.com/Article/details/grwgepzpl.sHtML

echo "${#arr[@]}"
来源：http://www.share.yfazqb.com/Article/details/gbatnzbtb.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.vehdjk.com/Article/details/gadlkxjqf.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.sjlbkw.cn/Article/details/gquxxhykh.sHtML

[R21] 字符串长度
来源：http://m.share.fktsv.cn/Article/details/gwkaxhzeh.sHtML

echo "${#s}"
来源：http://www.share.vehdjk.com/Article/details/guviqymsy.sHtML

[R22] 截取子串
来源：http://read.share.fktsv.cn/Article/details/gfigekqbn.sHtML

echo "${s:0:5}"
来源：http://baike.yfazqb.com/Article/details/gytutrnwh.sHtML

[R23] 字符串替换
来源：http://www.share.epnwcf.com/Article/details/ganxvqskf.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.sjlbkw.cn/Article/details/gdmtjekxl.sHtML

[R24] 大小写转换
来源：http://mobile.sjlbkw.cn/Article/details/gpsqiouhc.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.sjlbkw.cn/Article/details/gjlglixoc.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.epnwcf.com/Article/details/gtrpcxxrr.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.sjlbkw.cn/Article/details/gsjeaxaar.sHtML

[R26] 命令替换
来源：http://3g.fktsv.cn/Article/details/gynumxzgp.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.epnwcf.com/Article/details/gxvxhjwxf.sHtML

[R27] 算术展开
来源：http://www.m.share.vehdjk.com/Article/details/gpvzwbdyl.sHtML

echo $((1 + 2 * 3))
来源：http://baike.vehdjk.com/Article/details/gxdrgckmm.sHtML

[R28] 浮点运算
来源：http://mobile.fktsv.cn/Article/details/ghjambpbx.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.fktsv.cn/Article/details/gqnhfzdfs.sHtML

[R29] 定义函数
来源：http://wap.epnwcf.com/Article/details/gycwgnkwz.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.epnwcf.com/Article/details/gehjawntp.sHtML

[R30] 函数返回状态码
来源：http://www.blog.epnwcf.com/Article/details/gvnkohykb.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.vehdjk.com/Article/details/genioptqs.sHtML

[R31] 局部变量
来源：http://www.m.share.tarul.cn/Article/details/gfutvogsz.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.yfazqb.com/Article/details/gavxgvicg.sHtML

[R32] 参数个数校验
来源：http://wap.epnwcf.com/Article/details/gnrajzasb.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.bbcook.cn/Article/details/gtqavbqtg.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.yfazqb.com/Article/details/gduilccmy.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.vehdjk.com/Article/details/goqfjgvdx.sHtML

[R34] 退出时清理
来源：http://www.blog.sjlbkw.cn/Article/details/gvnltpmoo.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.yfazqb.com/Article/details/gwvrqpauq.sHtML

[R35] 后台执行并等待
来源：http://blog.fktsv.cn/Article/details/gnncweakw.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fktsv.cn/Article/details/gnxfzpefl.sHtML

[R36] 并发执行多个任务
来源：http://www.share.epnwcf.com/Article/details/gnlvhmixl.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.fktsv.cn/Article/details/gtvldxnvo.sHtML

[R37] 把输出赋给变量
来源：http://wap.fktsv.cn/Article/details/gfkbtqukd.sHtML

files=$(ls -1)
来源：http://read.share.bbcook.cn/Article/details/gcvfyavla.sHtML

[R38] 管道串联
来源：http://read.share.bbcook.cn/Article/details/gvixifbcw.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.tarul.cn/Article/details/gxmclvozk.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.tarul.cn/Article/details/gsmvszlaw.sHtML

cmd > out.log 2>&1
来源：http://www.share.vehdjk.com/Article/details/gwfqdjumj.sHtML

[R40] 追加写日志
来源：http://baike.vehdjk.com/Article/details/gomrggxbd.sHtML

echo "log" >> out.log
来源：http://blog.fktsv.cn/Article/details/grambhkvj.sHtML

[R41] 丢弃输出
来源：http://www.m.share.epnwcf.com/Article/details/gonhoeesz.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.tarul.cn/Article/details/gaqokhabs.sHtML

[R42] 输入重定向
来源：http://m.share.vehdjk.com/Article/details/gtqlnrvfq.sHtML

wc -l < a.txt
来源：http://www.blog.bbcook.cn/Article/details/gmkfjsbed.sHtML

[R43] 按名字查找文件
来源：http://wap.bbcook.cn/Article/details/gtauhicxl.sHtML

find . -name "*.log" -type f
来源：http://baike.epnwcf.com/Article/details/gprhgyfze.sHtML

[R44] 按修改时间查找
来源：http://mobile.bbcook.cn/Article/details/gaqroiuut.sHtML

find . -mtime -7 -type f
来源：http://www.blog.vehdjk.com/Article/details/gjnhjtdkc.sHtML

[R45] 批量删除
来源：http://www.m.share.sjlbkw.cn/Article/details/gkxvcaquj.sHtML

find . -name "*.tmp" -delete
来源：http://baike.sjlbkw.cn/Article/details/gkjheshwu.sHtML

[R46] 递归替换文件内容
来源：http://m.share.tarul.cn/Article/details/gnnzabfbk.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.vehdjk.com/Article/details/gtkhsftdm.sHtML

[R47] sed 单行替换
来源：http://www.share.sjlbkw.cn/Article/details/gukjdwjal.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.vehdjk.com/Article/details/gapdmpmjs.sHtML

[R48] awk 取指定列
来源：http://www.share.sjlbkw.cn/Article/details/gamegefpa.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.vehdjk.com/Article/details/gtdidrzzd.sHtML

[R49] awk 带条件
来源：http://www.blog.tarul.cn/Article/details/gwutlzjdr.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.epnwcf.com/Article/details/ghvvostij.sHtML

[R50] awk 求和
来源：http://www.blog.yfazqb.com/Article/details/gfaohvspy.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.epnwcf.com/Article/details/gdqhzevff.sHtML

[R51] 排序去重取前几
来源：http://baike.fktsv.cn/Article/details/gasnqmxae.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.sjlbkw.cn/Article/details/gwhttnudh.sHtML

[R52] 统计行数
来源：http://baike.sjlbkw.cn/Article/details/gbngdzkgi.sHtML

wc -l a.txt
来源：http://3g.epnwcf.com/Article/details/gaolslxew.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.epnwcf.com/Article/details/gppgzhaqd.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fktsv.cn/Article/details/gulnzbczq.sHtML

[R54] 比较两个文件
来源：http://wap.sjlbkw.cn/Article/details/gjuefgiim.sHtML

diff a.txt b.txt
来源：http://wap.epnwcf.com/Article/details/ggynqdxnj.sHtML

[R55] 压缩与解压
来源：http://baike.vehdjk.com/Article/details/gbycjagqo.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.epnwcf.com/Article/details/gezvsfpvd.sHtML

[R56] 远程拷贝
来源：http://blog.sjlbkw.cn/Article/details/gxqvbofjx.sHtML

scp file user@host:/path/
来源：http://mobile.fktsv.cn/Article/details/gblvpjkep.sHtML

[R57] 远程执行命令
来源：http://read.share.yfazqb.com/Article/details/gpcmfbpus.sHtML

ssh user@host 'uptime'
来源：http://baike.fktsv.cn/Article/details/ggxnzuadp.sHtML

[R58] 下载文件
来源：http://www.share.sjlbkw.cn/Article/details/gefqcbmek.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.tarul.cn/Article/details/ghjocbgjw.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fktsv.cn/Article/details/gifwzgkwk.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.vehdjk.com/Article/details/gchwdobhi.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.sjlbkw.cn/Article/details/gqefsaela.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.bbcook.cn/Article/details/giwwdnrdm.sHtML

[R61] 磁盘占用
来源：http://baike.tarul.cn/Article/details/gryzdaukz.sHtML

df -h;  du -sh *
来源：http://www.m.share.vehdjk.com/Article/details/glwfknysv.sHtML

[R62] 找最占空间的文件
来源：http://mobile.yfazqb.com/Article/details/gzrvdqygx.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.tarul.cn/Article/details/gjgefakgv.sHtML

[R63] 内存与进程
来源：http://www.blog.tarul.cn/Article/details/gkjttvvpg.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.vehdjk.com/Article/details/gmbfcutwp.sHtML

[R64] 结束进程
来源：http://blog.vehdjk.com/Article/details/gonrcfxca.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.tarul.cn/Article/details/gxsmyqgvg.sHtML

[R65] 查看端口占用
来源：http://read.share.fktsv.cn/Article/details/gkdbdpzhy.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.epnwcf.com/Article/details/govdjutfb.sHtML

[R66] 定时任务
来源：http://read.share.epnwcf.com/Article/details/gwjqlodad.sHtML

crontab -e;  crontab -l
来源：http://wap.sjlbkw.cn/Article/details/ggtmicqvu.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.tarul.cn/Article/details/gzedkjkyr.sHtML

openssl rand -hex 16
来源：http://wap.epnwcf.com/Article/details/gespzxccj.sHtML

[R68] 计算文件校验值
来源：http://wap.tarul.cn/Article/details/gkfmgurak.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.yfazqb.com/Article/details/gpexuhnhj.sHtML

[R69] 生成随机密码
来源：http://blog.tarul.cn/Article/details/gbdvyelaf.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.vehdjk.com/Article/details/gavzrzgtk.sHtML

[R70] 时间戳与互转
来源：http://baike.bbcook.cn/Article/details/gkdlvgytn.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.vehdjk.com/Article/details/gzbuluhjc.sHtML

[R71] 日期格式化
来源：http://www.share.tarul.cn/Article/details/guepkwzbt.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.vehdjk.com/Article/details/gzpjrnxtu.sHtML

[R72] 等待端口就绪
来源：http://www.share.yfazqb.com/Article/details/gwlfccydz.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.tarul.cn/Article/details/goqrcalvj.sHtML

[R73] 分割大日志
来源：http://3g.bbcook.cn/Article/details/ghgcojonw.sHtML

split -l 1000 big.log part_
来源：http://www.share.yfazqb.com/Article/details/gvxnepxxh.sHtML

[R74] 批量重命名
来源：http://read.share.yfazqb.com/Article/details/gafzrkzre.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.vehdjk.com/Article/details/gdhftjohv.sHtML

[R75] 导出环境变量
来源：http://www.m.share.yfazqb.com/Article/details/gcwwegcqm.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.yfazqb.com/Article/details/gtoncabam.sHtML

[R76] 使用临时文件
来源：http://blog.sjlbkw.cn/Article/details/gbslqdund.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fktsv.cn/Article/details/gydmhpnta.sHtML

[R77] 读取用户输入
来源：http://m.share.vehdjk.com/Article/details/ghzkqlmhs.sHtML

read -rp "请输入: " ans
来源：http://read.share.vehdjk.com/Article/details/gtgfanviy.sHtML

[R78] 交互式菜单
来源：http://3g.sjlbkw.cn/Article/details/gkmalfjnf.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.yfazqb.com/Article/details/gtwvhakbq.sHtML

[R79] 解析命令行选项
来源：http://baike.tarul.cn/Article/details/gzjowoueo.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.sjlbkw.cn/Article/details/gvbesvyqg.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.yfazqb.com/Article/details/ggyivljpo.sHtML

time ./run.sh
来源：http://blog.tarul.cn/Article/details/gmvuhudqy.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gffuqhmmq.sHtML

S. C / C++ 专题
来源：http://www.share.vehdjk.com/Article/details/gjznchyco.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gmnacjeoe.sHtML

[S01] C：Hello World
来源：http://blog.sjlbkw.cn/Article/details/gysinojwl.sHtML

#include <stdio.h>
来源：http://read.share.vehdjk.com/Article/details/gipawuehl.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.bbcook.cn/Article/details/glbmtcaww.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fktsv.cn/Article/details/gmldqguri.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.bbcook.cn/Article/details/gwjvgajji.sHtML

[S03] C：读入整数
来源：http://m.share.bbcook.cn/Article/details/grdaglqfd.sHtML

int x; scanf("%d", &x);
来源：http://3g.fktsv.cn/Article/details/glmllsksb.sHtML

[S04] C：字符串复制
来源：http://mobile.yfazqb.com/Article/details/gqueqamon.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fktsv.cn/Article/details/gqjsxnfte.sHtML

[S05] C：字符串长度
来源：http://blog.sjlbkw.cn/Article/details/gnatvmijr.sHtML

strlen(s)
来源：http://read.share.tarul.cn/Article/details/gujjrdilh.sHtML

[S06] C：字符串比较
来源：http://www.blog.bbcook.cn/Article/details/gkqpphkhm.sHtML

strcmp(a, b) == 0
来源：http://baike.sjlbkw.cn/Article/details/ghrmflrhr.sHtML

[S07] C：数组遍历求和
来源：http://3g.sjlbkw.cn/Article/details/gfdlntpgk.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.epnwcf.com/Article/details/gmfgatjqw.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.yfazqb.com/Article/details/gedghirmr.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.epnwcf.com/Article/details/gkfktoxrn.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.bbcook.cn/Article/details/gosmgspoy.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.bbcook.cn/Article/details/gnqeuzygg.sHtML

[S10] C：指针与解引用
来源：http://baike.tarul.cn/Article/details/ghygrvotk.sHtML

int *p = &a;  *p = 5;
来源：http://3g.tarul.cn/Article/details/gfgkppwzs.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gggtljdmm.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.yfazqb.com/Article/details/gbfuasaol.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.bbcook.cn/Article/details/gisskywtd.sHtML

fclose(f);
来源：http://www.share.tarul.cn/Article/details/gylzjfywu.sHtML

[S12] C：写文件
来源：http://3g.bbcook.cn/Article/details/goqyfpxnw.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.yfazqb.com/Article/details/gbtofkvhl.sHtML

[S13] C：宏定义
来源：http://m.share.epnwcf.com/Article/details/gkpgzmdev.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.tarul.cn/Article/details/gftqewyba.sHtML

[S14] C：枚举
来源：http://3g.yfazqb.com/Article/details/gkqhzajdt.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.vehdjk.com/Article/details/gceqbobta.sHtML

[S15] C：类型转换
来源：http://www.share.yfazqb.com/Article/details/grknzkjse.sHtML

(double) a / b
来源：http://www.share.bbcook.cn/Article/details/gjxbyuzzd.sHtML

[S16] C：位操作置位
来源：http://wap.vehdjk.com/Article/details/gcuzimpua.sHtML

x |= (1 << 3);
来源：http://3g.epnwcf.com/Article/details/ggrdqneqy.sHtML

[S17] C：安全拼接字符串
来源：http://blog.yfazqb.com/Article/details/guvijulwr.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.sjlbkw.cn/Article/details/gjvkitjnj.sHtML

[S18] C：命令行参数
来源：http://m.share.sjlbkw.cn/Article/details/gchzunlbz.sHtML

int main(int argc, char **argv)
来源：http://mobile.epnwcf.com/Article/details/gnkbacjaq.sHtML

[S19] C：快速排序
来源：http://www.blog.sjlbkw.cn/Article/details/gurrtsbpx.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.epnwcf.com/Article/details/gqhxzzrvs.sHtML

[S20] C：二分查找
来源：http://read.share.vehdjk.com/Article/details/gjznxiaem.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.tarul.cn/Article/details/gnidazdko.sHtML

[S21] C：字符类别判断
来源：http://www.share.yfazqb.com/Article/details/gdgnrmsub.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.yfazqb.com/Article/details/grrzkxijf.sHtML

[S22] C：字符串转数字
来源：http://baike.vehdjk.com/Article/details/gtkhqlzog.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.yfazqb.com/Article/details/gatssydnb.sHtML

[S23] C：随机数
来源：http://www.blog.bbcook.cn/Article/details/gouwjxeev.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.bbcook.cn/Article/details/gysiifrqh.sHtML

[S24] C：获取本地时间
来源：http://www.share.fktsv.cn/Article/details/gpbpxyset.sHtML


<!-- 参考信息 -->