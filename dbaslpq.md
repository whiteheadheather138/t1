代发 wailian999

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.vehdjk.com/Article/details/ghgiozjcn.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fktsv.cn/Article/details/gdnjgnssc.sHtML

[Q47] 与平均值比较
来源：http://www.share.vehdjk.com/Article/details/glsfcdqxx.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.sjlbkw.cn/Article/details/gnkrbwbvp.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.vehdjk.com/Article/details/geqnziqke.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.fktsv.cn/Article/details/gbnncbhfo.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.fktsv.cn/Article/details/gfnotomsf.sHtML

[Q49] 更新单行
来源：http://wap.yfazqb.com/Article/details/graddahja.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.tarul.cn/Article/details/grgedxqkd.sHtML

[Q50] 批量更新
来源：http://3g.yfazqb.com/Article/details/gxzpdpfqt.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.tarul.cn/Article/details/grvqhogow.sHtML

[Q51] 用子查询更新
来源：http://www.share.bbcook.cn/Article/details/gwtjneopr.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.epnwcf.com/Article/details/geqqaigiu.sHtML

[Q52] 删除指定行
来源：http://blog.tarul.cn/Article/details/gdhcmcufm.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.sjlbkw.cn/Article/details/gdnwcnphu.sHtML

[Q53] 按条件删除
来源：http://www.share.bbcook.cn/Article/details/grcjuzedt.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.sjlbkw.cn/Article/details/gosfljexi.sHtML

[Q54] 清空表
来源：http://www.blog.bbcook.cn/Article/details/gfcpsutrx.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.epnwcf.com/Article/details/gkfvrjyow.sHtML

[Q55] 排名（并列占位）
来源：http://wap.fktsv.cn/Article/details/guvhysuls.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.epnwcf.com/Article/details/gwqyjcfww.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.fktsv.cn/Article/details/gewbzrbeb.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.epnwcf.com/Article/details/gjvbvgyzk.sHtML

[Q57] 行号
来源：http://www.share.yfazqb.com/Article/details/gypucrvas.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.tarul.cn/Article/details/gtrtfxclh.sHtML

[Q58] 累计求和
来源：http://baike.yfazqb.com/Article/details/gtrligrfq.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.epnwcf.com/Article/details/gdfwtqiwf.sHtML

[Q59] 分组内累计
来源：http://3g.yfazqb.com/Article/details/gjfvthocr.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.yfazqb.com/Article/details/gjttcctlt.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.bbcook.cn/Article/details/gxgiysquh.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.yfazqb.com/Article/details/gqjhnmnfd.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.epnwcf.com/Article/details/gipgalrpk.sHtML

[Q61] 移动平均
来源：http://www.share.vehdjk.com/Article/details/gskkitpsu.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.fktsv.cn/Article/details/glhplefuo.sHtML

[Q62] 分组占比
来源：http://www.share.vehdjk.com/Article/details/gntfjkrpx.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.sjlbkw.cn/Article/details/gtcaxgwgd.sHtML

[Q63] 开启事务
来源：http://wap.sjlbkw.cn/Article/details/glyuvgimv.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.bbcook.cn/Article/details/ghagpegvg.sHtML

[Q64] 提交事务
来源：http://www.m.share.fktsv.cn/Article/details/gduaupvko.sHtML

COMMIT;
来源：http://read.share.vehdjk.com/Article/details/gnaskolsx.sHtML

[Q65] 回滚事务
来源：http://3g.sjlbkw.cn/Article/details/gpvduqfzs.sHtML

ROLLBACK;
来源：http://www.blog.bbcook.cn/Article/details/gaopxsnjb.sHtML

[Q66] 行锁查询
来源：http://baike.fktsv.cn/Article/details/gduuhyhrh.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.epnwcf.com/Article/details/goavmrdmq.sHtML

[Q67] 设置隔离级别
来源：http://wap.tarul.cn/Article/details/gmzuyswco.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.epnwcf.com/Article/details/gffymtsfa.sHtML

[Q68] 保存点
来源：http://mobile.bbcook.cn/Article/details/grhkitprb.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.fktsv.cn/Article/details/grgoikmpg.sHtML

ROLLBACK TO sp1;
来源：http://mobile.tarul.cn/Article/details/gsqscwdpp.sHtML

[Q69] 查看执行计划
来源：http://3g.yfazqb.com/Article/details/gydyzbijt.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.yfazqb.com/Article/details/gsodcelsk.sHtML

[Q70] 更新统计信息
来源：http://baike.tarul.cn/Article/details/gjhwiwwit.sHtML

ANALYZE TABLE users;
来源：http://read.share.epnwcf.com/Article/details/gzxcyziqk.sHtML

[Q71] 查看建表语句
来源：http://baike.tarul.cn/Article/details/gcslobsgi.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.epnwcf.com/Article/details/gvcolivno.sHtML

[Q72] 查看索引
来源：http://m.share.fktsv.cn/Article/details/gdsvpbxxj.sHtML

SHOW INDEX FROM users;
来源：http://3g.bbcook.cn/Article/details/gmdnqmaes.sHtML

[Q73] 查看表状态
来源：http://read.share.vehdjk.com/Article/details/gcacbniia.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.bbcook.cn/Article/details/gtpwdlrrc.sHtML

[Q74] 强制使用索引
来源：http://www.share.bbcook.cn/Article/details/gxblffjii.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.bbcook.cn/Article/details/gvmrqqdzt.sHtML

[Q75] 日期格式化
来源：http://www.m.share.fktsv.cn/Article/details/gugeldtqc.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.tarul.cn/Article/details/gudrtyjwp.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.yfazqb.com/Article/details/gzussuzgl.sHtML

[Q76] 按天统计
来源：http://www.m.share.fktsv.cn/Article/details/gxlvalmwb.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.vehdjk.com/Article/details/gfcmlosxy.sHtML

[Q77] 时间加减
来源：http://www.share.bbcook.cn/Article/details/gfkwemdbl.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.vehdjk.com/Article/details/girgziook.sHtML

[Q78] 当前时间
来源：http://wap.yfazqb.com/Article/details/gskdazqfb.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.epnwcf.com/Article/details/gnuzwcqpj.sHtML

[Q79] 字符串拼接
来源：http://blog.sjlbkw.cn/Article/details/gzqatozoy.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.sjlbkw.cn/Article/details/gndjuhtme.sHtML

[Q80] 字符串截取
来源：http://www.share.sjlbkw.cn/Article/details/gozxmhuaq.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.vehdjk.com/Article/details/gryobdvxi.sHtML

[Q81] 字符串替换
来源：http://baike.bbcook.cn/Article/details/gevockflf.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.fktsv.cn/Article/details/gatgnaorb.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.bbcook.cn/Article/details/gwbjahrzd.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.yfazqb.com/Article/details/gsdphcblu.sHtML

[Q83] 大小写转换
来源：http://wap.sjlbkw.cn/Article/details/ggvnihlxv.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.vehdjk.com/Article/details/gedcgsond.sHtML

[Q84] 去除首尾空格
来源：http://mobile.epnwcf.com/Article/details/ggoemgrzn.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.tarul.cn/Article/details/gmqsepozp.sHtML

[Q85] 数值取整
来源：http://mobile.epnwcf.com/Article/details/gzwxmktql.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.fktsv.cn/Article/details/gcvthcmck.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.epnwcf.com/Article/details/gfgtzgiwm.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.epnwcf.com/Article/details/gjydcymzb.sHtML

[Q87] JSON 字段做条件
来源：http://blog.bbcook.cn/Article/details/gatvdhxyn.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.yfazqb.com/Article/details/goytphgmd.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.tarul.cn/Article/details/gmcneiicg.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.bbcook.cn/Article/details/ghpilxowf.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.tarul.cn/Article/details/gnovhmnvu.sHtML

[Q89] 判断表是否存在
来源：http://mobile.epnwcf.com/Article/details/gzpjywldg.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.sjlbkw.cn/Article/details/guvuaoeky.sHtML

[Q90] 生成序号列
来源：http://baike.vehdjk.com/Article/details/ghbwijfpz.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.bbcook.cn/Article/details/gxazxvanf.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/glisxeqlz.sHtML

R. Bash 专题
来源：http://www.blog.vehdjk.com/Article/details/gjyilljrm.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/goudoywks.sHtML

[R01] shebang 与严格模式
来源：http://read.share.yfazqb.com/Article/details/gyenviebm.sHtML

#!/usr/bin/env bash
来源：http://wap.fktsv.cn/Article/details/gznzyrpgr.sHtML

set -euo pipefail
来源：http://www.m.share.sjlbkw.cn/Article/details/gcxzxfaxm.sHtML

[R02] 变量赋值与使用
来源：http://wap.sjlbkw.cn/Article/details/gxhkkpnlv.sHtML

name="Tom"; echo "$name"
来源：http://m.share.epnwcf.com/Article/details/ghuwzngpg.sHtML

[R03] 只读变量
来源：http://m.share.fktsv.cn/Article/details/gywpjyevo.sHtML

readonly PI=3.14
来源：http://3g.sjlbkw.cn/Article/details/gdpgyovdc.sHtML

[R04] 位置参数
来源：http://wap.vehdjk.com/Article/details/gthgyhuak.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.epnwcf.com/Article/details/guqmrjvum.sHtML

[R05] 参数默认值
来源：http://www.share.tarul.cn/Article/details/gkrzcmnwe.sHtML

name="${1:-default}"
来源：http://m.share.tarul.cn/Article/details/gejsoiwup.sHtML

[R06] 判断命令是否存在
来源：http://m.share.fktsv.cn/Article/details/ghwefanns.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.bbcook.cn/Article/details/gzjtvauwh.sHtML

[R07] if 判断文件
来源：http://m.share.tarul.cn/Article/details/gulucwwic.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.bbcook.cn/Article/details/gpsaryrct.sHtML

[R08] 数值比较
来源：http://www.blog.bbcook.cn/Article/details/gfahrnhtw.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.vehdjk.com/Article/details/gdtsthzbw.sHtML

[R09] 字符串比较
来源：http://www.m.share.epnwcf.com/Article/details/gscgsuflg.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.tarul.cn/Article/details/galgmtstb.sHtML

[R10] 正则匹配
来源：http://m.share.sjlbkw.cn/Article/details/gtoapbuyj.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.yfazqb.com/Article/details/gdxphdhkw.sHtML

[R11] case 多分支
来源：http://read.share.bbcook.cn/Article/details/gqwybkkzf.sHtML

case "$1" in
来源：http://www.m.share.epnwcf.com/Article/details/gccezmnyr.sHtML

start) echo "启动" ;;
来源：http://3g.bbcook.cn/Article/details/gmbxexgub.sHtML

stop)  echo "停止" ;;
来源：http://m.share.yfazqb.com/Article/details/gysdbaqqf.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.sjlbkw.cn/Article/details/gfhbxyvwn.sHtML

esac
来源：http://wap.sjlbkw.cn/Article/details/gawcwzloq.sHtML

[R12] for 遍历文件
来源：http://mobile.sjlbkw.cn/Article/details/gmlkraxgq.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.vehdjk.com/Article/details/gguhycvrx.sHtML

[R13] for 计数循环
来源：http://www.blog.bbcook.cn/Article/details/gfllajtas.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.epnwcf.com/Article/details/gxvlzapts.sHtML

[R14] C 风格 for
来源：http://3g.fktsv.cn/Article/details/gygugkxgr.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.bbcook.cn/Article/details/giacecqbj.sHtML

[R15] while 逐行读文件
来源：http://mobile.epnwcf.com/Article/details/gcfsipazn.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.vehdjk.com/Article/details/gojfcucdt.sHtML

[R16] until 等待条件
来源：http://read.share.yfazqb.com/Article/details/gdumumrrg.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fktsv.cn/Article/details/gkmybbfyt.sHtML

[R17] 数组定义与取值
来源：http://3g.epnwcf.com/Article/details/gjrkmmieb.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.sjlbkw.cn/Article/details/gttokxicn.sHtML

[R18] 遍历数组
来源：http://wap.sjlbkw.cn/Article/details/gkfrjbzje.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.fktsv.cn/Article/details/gnejaqlan.sHtML

[R19] 数组长度
来源：http://mobile.tarul.cn/Article/details/gypyvsarl.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.sjlbkw.cn/Article/details/gljvssaen.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.epnwcf.com/Article/details/gbxxbdhdf.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.yfazqb.com/Article/details/gljzxipsx.sHtML

[R21] 字符串长度
来源：http://m.share.vehdjk.com/Article/details/gvhzcloty.sHtML

echo "${#s}"
来源：http://wap.epnwcf.com/Article/details/gatmvvekz.sHtML

[R22] 截取子串
来源：http://m.share.vehdjk.com/Article/details/gsswqvnnm.sHtML

echo "${s:0:5}"
来源：http://www.m.share.vehdjk.com/Article/details/ggmkdyqwf.sHtML

[R23] 字符串替换
来源：http://www.m.share.bbcook.cn/Article/details/gbaeffsdz.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.vehdjk.com/Article/details/gfmzqjwty.sHtML

[R24] 大小写转换
来源：http://baike.fktsv.cn/Article/details/gjwpmvrzf.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.tarul.cn/Article/details/godlxhcxu.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.vehdjk.com/Article/details/gcxebpqtv.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.tarul.cn/Article/details/gnbswtiyj.sHtML

[R26] 命令替换
来源：http://www.blog.yfazqb.com/Article/details/gqpygubyn.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.yfazqb.com/Article/details/goranrbmp.sHtML

[R27] 算术展开
来源：http://mobile.fktsv.cn/Article/details/gcjrbwymu.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.sjlbkw.cn/Article/details/gzuclwoem.sHtML

[R28] 浮点运算
来源：http://blog.vehdjk.com/Article/details/gckqgeksk.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.yfazqb.com/Article/details/gfetinaek.sHtML

[R29] 定义函数
来源：http://wap.bbcook.cn/Article/details/gszeqneff.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.bbcook.cn/Article/details/gbqsalmxs.sHtML

[R30] 函数返回状态码
来源：http://wap.epnwcf.com/Article/details/gpetjfktj.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.yfazqb.com/Article/details/gskwsrczl.sHtML

[R31] 局部变量
来源：http://m.share.fktsv.cn/Article/details/gxvdwjcpx.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.vehdjk.com/Article/details/gajyrvkik.sHtML

[R32] 参数个数校验
来源：http://www.blog.fktsv.cn/Article/details/gsrokhtqu.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.yfazqb.com/Article/details/gyfybaxjd.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.epnwcf.com/Article/details/gtincofcr.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.vehdjk.com/Article/details/gpqdpthms.sHtML

[R34] 退出时清理
来源：http://read.share.epnwcf.com/Article/details/gourvxalf.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fktsv.cn/Article/details/ggnihyvfn.sHtML

[R35] 后台执行并等待
来源：http://mobile.epnwcf.com/Article/details/gctjkugvp.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.sjlbkw.cn/Article/details/gwfvdnljc.sHtML

[R36] 并发执行多个任务
来源：http://3g.tarul.cn/Article/details/gfqwaebwa.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.fktsv.cn/Article/details/gmfdwmpme.sHtML

[R37] 把输出赋给变量
来源：http://blog.vehdjk.com/Article/details/giutwqpbz.sHtML

files=$(ls -1)
来源：http://m.share.bbcook.cn/Article/details/gefeellsc.sHtML

[R38] 管道串联
来源：http://read.share.yfazqb.com/Article/details/gsowbhlai.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.yfazqb.com/Article/details/gvdhiilwa.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fktsv.cn/Article/details/gzcilwrue.sHtML

cmd > out.log 2>&1
来源：http://3g.yfazqb.com/Article/details/grhbcneas.sHtML

[R40] 追加写日志
来源：http://baike.epnwcf.com/Article/details/gnisyqlwn.sHtML

echo "log" >> out.log
来源：http://www.blog.bbcook.cn/Article/details/gwtlzunup.sHtML

[R41] 丢弃输出
来源：http://www.share.epnwcf.com/Article/details/gcpwgfdhu.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.epnwcf.com/Article/details/gbxpgwtcj.sHtML

[R42] 输入重定向
来源：http://read.share.tarul.cn/Article/details/grvidgdrr.sHtML

wc -l < a.txt
来源：http://blog.tarul.cn/Article/details/grgzuiffj.sHtML

[R43] 按名字查找文件
来源：http://www.share.vehdjk.com/Article/details/gygewdmxj.sHtML

find . -name "*.log" -type f
来源：http://m.share.fktsv.cn/Article/details/gllglslau.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.tarul.cn/Article/details/gluuqmpgv.sHtML

find . -mtime -7 -type f
来源：http://www.share.fktsv.cn/Article/details/gmnziogww.sHtML

[R45] 批量删除
来源：http://www.share.bbcook.cn/Article/details/gwbpagfyo.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.sjlbkw.cn/Article/details/gqoctwpfg.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.sjlbkw.cn/Article/details/ggtxzajiq.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.epnwcf.com/Article/details/gvkcpaqjz.sHtML

[R47] sed 单行替换
来源：http://www.blog.vehdjk.com/Article/details/goelkzufv.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.fktsv.cn/Article/details/gqgidlhzl.sHtML

[R48] awk 取指定列
来源：http://baike.sjlbkw.cn/Article/details/gyhqupilx.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.vehdjk.com/Article/details/ggztyueni.sHtML

[R49] awk 带条件
来源：http://m.share.vehdjk.com/Article/details/gvircwmvk.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.sjlbkw.cn/Article/details/gybohsyrg.sHtML

[R50] awk 求和
来源：http://read.share.bbcook.cn/Article/details/gzupdlnez.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.vehdjk.com/Article/details/gpsvfmref.sHtML

[R51] 排序去重取前几
来源：http://blog.bbcook.cn/Article/details/gadebxdvt.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.vehdjk.com/Article/details/ghybjbtei.sHtML

[R52] 统计行数
来源：http://www.share.sjlbkw.cn/Article/details/gzyfjdjbn.sHtML

wc -l a.txt
来源：http://read.share.tarul.cn/Article/details/ghjznjlno.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.vehdjk.com/Article/details/gxcguqskq.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.bbcook.cn/Article/details/glsstcute.sHtML

[R54] 比较两个文件
来源：http://blog.bbcook.cn/Article/details/gnybhgwgv.sHtML

diff a.txt b.txt
来源：http://wap.bbcook.cn/Article/details/gbtszkdek.sHtML

[R55] 压缩与解压
来源：http://www.m.share.bbcook.cn/Article/details/gzbuftryh.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.tarul.cn/Article/details/gqnxrejnh.sHtML

[R56] 远程拷贝
来源：http://mobile.vehdjk.com/Article/details/grsfovbhq.sHtML

scp file user@host:/path/
来源：http://baike.vehdjk.com/Article/details/gzafsgbom.sHtML

[R57] 远程执行命令
来源：http://blog.yfazqb.com/Article/details/ggnuqunjm.sHtML

ssh user@host 'uptime'
来源：http://baike.tarul.cn/Article/details/ghpkhmrcx.sHtML

[R58] 下载文件
来源：http://www.blog.sjlbkw.cn/Article/details/gdkujsibo.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.epnwcf.com/Article/details/giqjwrlgm.sHtML

[R59] 发 POST JSON
来源：http://3g.tarul.cn/Article/details/gabtqrxgq.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.tarul.cn/Article/details/gacfqjroh.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.bbcook.cn/Article/details/gapadrhha.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.vehdjk.com/Article/details/gqcddvyce.sHtML

[R61] 磁盘占用
来源：http://blog.epnwcf.com/Article/details/gdciibory.sHtML

df -h;  du -sh *
来源：http://baike.fktsv.cn/Article/details/gsxfwoqjk.sHtML

[R62] 找最占空间的文件
来源：http://wap.vehdjk.com/Article/details/gevjwwwls.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.sjlbkw.cn/Article/details/gjsquanhh.sHtML

[R63] 内存与进程
来源：http://www.share.bbcook.cn/Article/details/gfzuzwujh.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.vehdjk.com/Article/details/gemqdzxcp.sHtML

[R64] 结束进程
来源：http://3g.yfazqb.com/Article/details/gwdmkrjlx.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.epnwcf.com/Article/details/gvwwelmmq.sHtML

[R65] 查看端口占用
来源：http://mobile.epnwcf.com/Article/details/gfqyhzxwc.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.tarul.cn/Article/details/ggbgfyifr.sHtML

[R66] 定时任务
来源：http://3g.sjlbkw.cn/Article/details/gpzapnurr.sHtML

crontab -e;  crontab -l
来源：http://www.blog.bbcook.cn/Article/details/gqjctostx.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fktsv.cn/Article/details/gwpivnxvn.sHtML

openssl rand -hex 16
来源：http://www.m.share.epnwcf.com/Article/details/gumbfmels.sHtML

[R68] 计算文件校验值
来源：http://blog.tarul.cn/Article/details/gksrvokca.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.epnwcf.com/Article/details/gqgzdbdhg.sHtML

[R69] 生成随机密码
来源：http://3g.epnwcf.com/Article/details/ggvtricik.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.tarul.cn/Article/details/gwylbxazf.sHtML

[R70] 时间戳与互转
来源：http://m.share.tarul.cn/Article/details/gjaedzoci.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fktsv.cn/Article/details/gpmzdlxce.sHtML

[R71] 日期格式化
来源：http://www.m.share.yfazqb.com/Article/details/gfnygukjs.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.vehdjk.com/Article/details/gpaukgxcl.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.yfazqb.com/Article/details/gbfhnncpg.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.yfazqb.com/Article/details/ggxsurado.sHtML

[R73] 分割大日志
来源：http://wap.epnwcf.com/Article/details/giiuucfzi.sHtML

split -l 1000 big.log part_
来源：http://wap.vehdjk.com/Article/details/gasqwhoqg.sHtML

[R74] 批量重命名
来源：http://3g.epnwcf.com/Article/details/gklmcdnrn.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.tarul.cn/Article/details/gaipoltsk.sHtML

[R75] 导出环境变量
来源：http://www.m.share.yfazqb.com/Article/details/gvokkinhv.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.sjlbkw.cn/Article/details/gwvpqmerw.sHtML

[R76] 使用临时文件
来源：http://www.share.yfazqb.com/Article/details/grrgdwutk.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.yfazqb.com/Article/details/gxayxyaik.sHtML

[R77] 读取用户输入
来源：http://www.share.tarul.cn/Article/details/gfnubnnnz.sHtML

read -rp "请输入: " ans
来源：http://wap.bbcook.cn/Article/details/gmlvoejdg.sHtML

[R78] 交互式菜单
来源：http://3g.bbcook.cn/Article/details/gndujlaob.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.epnwcf.com/Article/details/grxbupxoo.sHtML

[R79] 解析命令行选项
来源：http://read.share.epnwcf.com/Article/details/guehwizbo.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.yfazqb.com/Article/details/gqetfxauw.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.yfazqb.com/Article/details/ganxwxima.sHtML

time ./run.sh
来源：http://www.m.share.tarul.cn/Article/details/gyknkceka.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gfpurpdke.sHtML

S. C / C++ 专题
来源：http://mobile.yfazqb.com/Article/details/gxhdtscom.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gmsomuqcn.sHtML

[S01] C：Hello World
来源：http://wap.epnwcf.com/Article/details/gegyvgsjt.sHtML

#include <stdio.h>
来源：http://www.blog.fktsv.cn/Article/details/gwfkpxznc.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.yfazqb.com/Article/details/gjzyuekdx.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fktsv.cn/Article/details/ghfexpqfl.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.vehdjk.com/Article/details/gtaqerafi.sHtML

[S03] C：读入整数
来源：http://blog.tarul.cn/Article/details/ghgwwecdp.sHtML

int x; scanf("%d", &x);
来源：http://blog.tarul.cn/Article/details/gpqxyqbth.sHtML

[S04] C：字符串复制
来源：http://www.share.sjlbkw.cn/Article/details/gsxhreyzl.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.vehdjk.com/Article/details/gitpxbjui.sHtML

[S05] C：字符串长度
来源：http://www.share.tarul.cn/Article/details/gifmfbbtg.sHtML

strlen(s)
来源：http://m.share.fktsv.cn/Article/details/gpsitczzi.sHtML

[S06] C：字符串比较
来源：http://mobile.sjlbkw.cn/Article/details/ggslakzfj.sHtML

strcmp(a, b) == 0
来源：http://3g.epnwcf.com/Article/details/gvyecnqcq.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.bbcook.cn/Article/details/gifqtohme.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fktsv.cn/Article/details/gjevbmobm.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.epnwcf.com/Article/details/ggadzbuzk.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.vehdjk.com/Article/details/gvuncwcdz.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.tarul.cn/Article/details/gvokptbyu.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.sjlbkw.cn/Article/details/gkgfwbdll.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.sjlbkw.cn/Article/details/gdvawmmxr.sHtML

int *p = &a;  *p = 5;
来源：http://wap.sjlbkw.cn/Article/details/gtnksbqaz.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.yfazqb.com/Article/details/gdrmfgdbt.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.bbcook.cn/Article/details/gqnawnhtp.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.vehdjk.com/Article/details/gdjigzlpo.sHtML

fclose(f);
来源：http://wap.vehdjk.com/Article/details/gkrljdxad.sHtML

[S12] C：写文件
来源：http://www.blog.fktsv.cn/Article/details/ghxohqvic.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.tarul.cn/Article/details/gqezwreld.sHtML

[S13] C：宏定义
来源：http://www.share.tarul.cn/Article/details/gerbbobai.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.yfazqb.com/Article/details/gnznmuoai.sHtML

[S14] C：枚举
来源：http://mobile.bbcook.cn/Article/details/ggzedbcil.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.bbcook.cn/Article/details/goyurqbvi.sHtML

[S15] C：类型转换
来源：http://m.share.fktsv.cn/Article/details/geacdhhid.sHtML

(double) a / b
来源：http://wap.epnwcf.com/Article/details/gwjgbcycs.sHtML

[S16] C：位操作置位
来源：http://www.share.sjlbkw.cn/Article/details/gagaixlnr.sHtML


<!-- 参考信息 -->