代发 wailian999

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.sjlbkw.cn/Article/details/gnypfsvne.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.vehdjk.com/Article/details/gzagfsbzp.sHtML

[Q35] 内连接
来源：http://www.share.bbcook.cn/Article/details/gblhroyxt.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.yfazqb.com/Article/details/gyjtxrvee.sHtML

[Q36] 左连接
来源：http://baike.tarul.cn/Article/details/goaoexfhx.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.tarul.cn/Article/details/gpljcthzh.sHtML

[Q37] 右连接
来源：http://www.blog.vehdjk.com/Article/details/gttgyajei.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.bbcook.cn/Article/details/glukqzyrf.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.fktsv.cn/Article/details/gqoioipck.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.fktsv.cn/Article/details/ghyhhvjew.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.bbcook.cn/Article/details/giqlxdmnl.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.epnwcf.com/Article/details/gqbosnaft.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.yfazqb.com/Article/details/geywlzjgt.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.vehdjk.com/Article/details/ggqvyetjv.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.vehdjk.com/Article/details/gglclqsas.sHtML

[Q41] 多表连接
来源：http://wap.vehdjk.com/Article/details/gedhyexsp.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.tarul.cn/Article/details/gueqzycek.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.fktsv.cn/Article/details/gvmtlbzby.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.bbcook.cn/Article/details/gbmthscpe.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.sjlbkw.cn/Article/details/gqlhawzhu.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.vehdjk.com/Article/details/gnrffcysn.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.vehdjk.com/Article/details/gqvocxvvq.sHtML

[Q43] 标量子查询
来源：http://read.share.vehdjk.com/Article/details/goflwsztk.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.epnwcf.com/Article/details/ghhvsmstt.sHtML

[Q44] IN 子查询
来源：http://3g.sjlbkw.cn/Article/details/gdqhqjqlw.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.epnwcf.com/Article/details/gishuqiuv.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.fktsv.cn/Article/details/gbhjoieii.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.epnwcf.com/Article/details/gfalfvmki.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.bbcook.cn/Article/details/gzgpuolzb.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.tarul.cn/Article/details/grgvurizg.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.vehdjk.com/Article/details/giptdkmwi.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.vehdjk.com/Article/details/gwgzpgznu.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.tarul.cn/Article/details/ghkapuvuq.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.vehdjk.com/Article/details/gsmlhjrwm.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.bbcook.cn/Article/details/gpjeuyqqv.sHtML

[Q49] 更新单行
来源：http://baike.yfazqb.com/Article/details/ggwjigofr.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.yfazqb.com/Article/details/gkbuhqezy.sHtML

[Q50] 批量更新
来源：http://baike.epnwcf.com/Article/details/gzkkvtzdh.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.sjlbkw.cn/Article/details/gblveectw.sHtML

[Q51] 用子查询更新
来源：http://read.share.vehdjk.com/Article/details/gvihnqyhe.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.fktsv.cn/Article/details/gyhghiopt.sHtML

[Q52] 删除指定行
来源：http://www.blog.sjlbkw.cn/Article/details/gleslwzsy.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.vehdjk.com/Article/details/gajwwldoq.sHtML

[Q53] 按条件删除
来源：http://3g.vehdjk.com/Article/details/gwurrdpgd.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.bbcook.cn/Article/details/gdeakkhpw.sHtML

[Q54] 清空表
来源：http://3g.bbcook.cn/Article/details/gmvppbver.sHtML

TRUNCATE TABLE logs;
来源：http://3g.fktsv.cn/Article/details/gsicxcuwz.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.sjlbkw.cn/Article/details/glmgbkgew.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.epnwcf.com/Article/details/gsuiiucwx.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.vehdjk.com/Article/details/gfngxeevk.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.bbcook.cn/Article/details/gitlxcwng.sHtML

[Q57] 行号
来源：http://3g.bbcook.cn/Article/details/gevltvqoc.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.vehdjk.com/Article/details/gevvtkfpi.sHtML

[Q58] 累计求和
来源：http://www.m.share.yfazqb.com/Article/details/glnegpknq.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.tarul.cn/Article/details/gnjudvhnq.sHtML

[Q59] 分组内累计
来源：http://blog.yfazqb.com/Article/details/govzwsxvi.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.tarul.cn/Article/details/gnygodpza.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.fktsv.cn/Article/details/gtiebcnyw.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.yfazqb.com/Article/details/guiuebckp.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.tarul.cn/Article/details/gwpgqykdx.sHtML

[Q61] 移动平均
来源：http://www.m.share.bbcook.cn/Article/details/ghqsjvnzz.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.vehdjk.com/Article/details/gnwxvtmbr.sHtML

[Q62] 分组占比
来源：http://mobile.bbcook.cn/Article/details/gkkkntmqa.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.sjlbkw.cn/Article/details/gwdekqtnw.sHtML

[Q63] 开启事务
来源：http://read.share.vehdjk.com/Article/details/gyboaenim.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.bbcook.cn/Article/details/gatykkplk.sHtML

[Q64] 提交事务
来源：http://mobile.tarul.cn/Article/details/gjkewxvhm.sHtML

COMMIT;
来源：http://www.m.share.sjlbkw.cn/Article/details/gxslniykc.sHtML

[Q65] 回滚事务
来源：http://wap.bbcook.cn/Article/details/gfcbfpytz.sHtML

ROLLBACK;
来源：http://wap.sjlbkw.cn/Article/details/gsahdonev.sHtML

[Q66] 行锁查询
来源：http://wap.vehdjk.com/Article/details/gqkgvycqg.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.yfazqb.com/Article/details/gtdzdbaqo.sHtML

[Q67] 设置隔离级别
来源：http://blog.tarul.cn/Article/details/ggreupsci.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.vehdjk.com/Article/details/gnvnlwmil.sHtML

[Q68] 保存点
来源：http://m.share.fktsv.cn/Article/details/gytqtwdds.sHtML

SAVEPOINT sp1;
来源：http://m.share.fktsv.cn/Article/details/gatfyyyfu.sHtML

ROLLBACK TO sp1;
来源：http://blog.fktsv.cn/Article/details/gdghmrubc.sHtML

[Q69] 查看执行计划
来源：http://www.share.fktsv.cn/Article/details/glmazevil.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.fktsv.cn/Article/details/gdvsrxtdo.sHtML

[Q70] 更新统计信息
来源：http://www.blog.vehdjk.com/Article/details/guwswtlws.sHtML

ANALYZE TABLE users;
来源：http://wap.bbcook.cn/Article/details/gkewentfo.sHtML

[Q71] 查看建表语句
来源：http://m.share.fktsv.cn/Article/details/gtlehvbwp.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.bbcook.cn/Article/details/gniwyudxv.sHtML

[Q72] 查看索引
来源：http://www.m.share.epnwcf.com/Article/details/gimvkzkpr.sHtML

SHOW INDEX FROM users;
来源：http://www.share.vehdjk.com/Article/details/grywrjvmz.sHtML

[Q73] 查看表状态
来源：http://www.share.epnwcf.com/Article/details/geqbonavb.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.vehdjk.com/Article/details/ggvkalhva.sHtML

[Q74] 强制使用索引
来源：http://m.share.fktsv.cn/Article/details/gmtuyvutu.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.vehdjk.com/Article/details/ghheuorpx.sHtML

[Q75] 日期格式化
来源：http://mobile.sjlbkw.cn/Article/details/gnlymswno.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.tarul.cn/Article/details/gmmpbbiap.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.tarul.cn/Article/details/gpeadjxgf.sHtML

[Q76] 按天统计
来源：http://3g.sjlbkw.cn/Article/details/gkyuyeidx.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.fktsv.cn/Article/details/gdevgqlbq.sHtML

[Q77] 时间加减
来源：http://www.share.tarul.cn/Article/details/gasuorymx.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.vehdjk.com/Article/details/gsvrlftjx.sHtML

[Q78] 当前时间
来源：http://mobile.epnwcf.com/Article/details/guugxgael.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.sjlbkw.cn/Article/details/gijdnhcpi.sHtML

[Q79] 字符串拼接
来源：http://m.share.vehdjk.com/Article/details/gkvwoywcm.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.bbcook.cn/Article/details/gpvmjvnky.sHtML

[Q80] 字符串截取
来源：http://wap.bbcook.cn/Article/details/gktyvvpyi.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.vehdjk.com/Article/details/gokzxvthi.sHtML

[Q81] 字符串替换
来源：http://read.share.sjlbkw.cn/Article/details/gfugysnzt.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.epnwcf.com/Article/details/gaqcffvky.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.tarul.cn/Article/details/gemmpxkqk.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.yfazqb.com/Article/details/gueydfaqu.sHtML

[Q83] 大小写转换
来源：http://mobile.yfazqb.com/Article/details/gknvmrpmo.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.sjlbkw.cn/Article/details/gjuxemkrg.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.vehdjk.com/Article/details/ghllxzpub.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.epnwcf.com/Article/details/gsddwizmw.sHtML

[Q85] 数值取整
来源：http://3g.vehdjk.com/Article/details/godzwserl.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.tarul.cn/Article/details/gkojgarlj.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.epnwcf.com/Article/details/gzowjlzty.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.tarul.cn/Article/details/gyljjvdnv.sHtML

[Q87] JSON 字段做条件
来源：http://wap.epnwcf.com/Article/details/ggtlfkpla.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.yfazqb.com/Article/details/gwrnplwdh.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.sjlbkw.cn/Article/details/gmakhoubg.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.bbcook.cn/Article/details/gbtcnhpxo.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/gbahxckyl.sHtML

[Q89] 判断表是否存在
来源：http://blog.tarul.cn/Article/details/gaekmyjzf.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.sjlbkw.cn/Article/details/geeulvwag.sHtML

[Q90] 生成序号列
来源：http://wap.bbcook.cn/Article/details/gletzlauo.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.epnwcf.com/Article/details/gyrxolydi.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gqgwlavsc.sHtML

R. Bash 专题
来源：http://baike.vehdjk.com/Article/details/gfpmzqzxd.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gfzrpmpol.sHtML

[R01] shebang 与严格模式
来源：http://3g.tarul.cn/Article/details/gsunixoup.sHtML

#!/usr/bin/env bash
来源：http://mobile.sjlbkw.cn/Article/details/grdnrkmnh.sHtML

set -euo pipefail
来源：http://wap.vehdjk.com/Article/details/gcnrxpcgw.sHtML

[R02] 变量赋值与使用
来源：http://wap.fktsv.cn/Article/details/gfiuuavni.sHtML

name="Tom"; echo "$name"
来源：http://www.share.yfazqb.com/Article/details/gfxxurdcq.sHtML

[R03] 只读变量
来源：http://3g.yfazqb.com/Article/details/gxwobazmd.sHtML

readonly PI=3.14
来源：http://www.share.sjlbkw.cn/Article/details/galvptnpq.sHtML

[R04] 位置参数
来源：http://wap.tarul.cn/Article/details/gkqzlnyvl.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.vehdjk.com/Article/details/gvjenzstr.sHtML

[R05] 参数默认值
来源：http://wap.sjlbkw.cn/Article/details/gtivhjomy.sHtML

name="${1:-default}"
来源：http://wap.yfazqb.com/Article/details/ghrvxsies.sHtML

[R06] 判断命令是否存在
来源：http://blog.epnwcf.com/Article/details/gfonkbycv.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.epnwcf.com/Article/details/gaiuihyuh.sHtML

[R07] if 判断文件
来源：http://mobile.tarul.cn/Article/details/gfsyciusz.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.sjlbkw.cn/Article/details/gkkpryvwp.sHtML

[R08] 数值比较
来源：http://blog.yfazqb.com/Article/details/gavqgxnhz.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.bbcook.cn/Article/details/gnnfqyrer.sHtML

[R09] 字符串比较
来源：http://wap.fktsv.cn/Article/details/gkghbcwds.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.fktsv.cn/Article/details/grxejtjqe.sHtML

[R10] 正则匹配
来源：http://3g.epnwcf.com/Article/details/garlkzmoc.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.sjlbkw.cn/Article/details/gqctlsebv.sHtML

[R11] case 多分支
来源：http://www.share.sjlbkw.cn/Article/details/glfcpadag.sHtML

case "$1" in
来源：http://wap.tarul.cn/Article/details/gssmbuvys.sHtML

start) echo "启动" ;;
来源：http://www.m.share.bbcook.cn/Article/details/gcvfbabzy.sHtML

stop)  echo "停止" ;;
来源：http://www.share.vehdjk.com/Article/details/gswsusmud.sHtML

*)     echo "未知命令" ;;
来源：http://wap.epnwcf.com/Article/details/giwuvqgzs.sHtML

esac
来源：http://mobile.bbcook.cn/Article/details/gnmttdqlx.sHtML

[R12] for 遍历文件
来源：http://mobile.bbcook.cn/Article/details/gdnbknukl.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.bbcook.cn/Article/details/glvucvvgw.sHtML

[R13] for 计数循环
来源：http://wap.epnwcf.com/Article/details/gdnxroxfn.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.yfazqb.com/Article/details/gwhfzhigh.sHtML

[R14] C 风格 for
来源：http://www.blog.tarul.cn/Article/details/gmvlpckny.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.epnwcf.com/Article/details/gejeshhye.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.yfazqb.com/Article/details/gupbufnee.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.fktsv.cn/Article/details/gjakvydjc.sHtML

[R16] until 等待条件
来源：http://wap.bbcook.cn/Article/details/ginkruqxs.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.sjlbkw.cn/Article/details/gflntpuez.sHtML

[R17] 数组定义与取值
来源：http://baike.sjlbkw.cn/Article/details/glwcuphft.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.bbcook.cn/Article/details/gkuozwfvk.sHtML

[R18] 遍历数组
来源：http://read.share.sjlbkw.cn/Article/details/glhgubdbd.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.fktsv.cn/Article/details/gkxzbbojq.sHtML

[R19] 数组长度
来源：http://wap.fktsv.cn/Article/details/gipxxpbqq.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.epnwcf.com/Article/details/geekahuil.sHtML

[R20] 关联数组（字典）
来源：http://m.share.bbcook.cn/Article/details/gaxmrmake.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.epnwcf.com/Article/details/guiwyqgyt.sHtML

[R21] 字符串长度
来源：http://mobile.vehdjk.com/Article/details/gqscvohqh.sHtML

echo "${#s}"
来源：http://mobile.epnwcf.com/Article/details/gocsialdq.sHtML

[R22] 截取子串
来源：http://read.share.sjlbkw.cn/Article/details/gwxbbewng.sHtML

echo "${s:0:5}"
来源：http://read.share.sjlbkw.cn/Article/details/gtdltvchq.sHtML

[R23] 字符串替换
来源：http://read.share.bbcook.cn/Article/details/gypgyopoj.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.sjlbkw.cn/Article/details/gloijwdtv.sHtML

[R24] 大小写转换
来源：http://mobile.tarul.cn/Article/details/gtxdycyke.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.vehdjk.com/Article/details/ggandrrlg.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.tarul.cn/Article/details/gzmrigyob.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.tarul.cn/Article/details/ggrexjshy.sHtML

[R26] 命令替换
来源：http://wap.yfazqb.com/Article/details/gjuypjmkr.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.bbcook.cn/Article/details/gfzvpetwv.sHtML

[R27] 算术展开
来源：http://www.share.epnwcf.com/Article/details/gbnxrpadg.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.epnwcf.com/Article/details/gvbygctjt.sHtML

[R28] 浮点运算
来源：http://www.m.share.yfazqb.com/Article/details/gwwqcztpi.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.epnwcf.com/Article/details/grqejpbmh.sHtML

[R29] 定义函数
来源：http://m.share.sjlbkw.cn/Article/details/glsvyaxqm.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.bbcook.cn/Article/details/gjzuhdyiu.sHtML

[R30] 函数返回状态码
来源：http://read.share.sjlbkw.cn/Article/details/gfteghkpl.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.epnwcf.com/Article/details/gximrcxxb.sHtML

[R31] 局部变量
来源：http://3g.epnwcf.com/Article/details/gkoeeiuse.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.yfazqb.com/Article/details/gvwzispgt.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fktsv.cn/Article/details/gesshjxfy.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.yfazqb.com/Article/details/gdthanvex.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fktsv.cn/Article/details/gcwhipdkj.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.fktsv.cn/Article/details/gnkxpcyti.sHtML

[R34] 退出时清理
来源：http://read.share.bbcook.cn/Article/details/gredastwu.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.bbcook.cn/Article/details/gqovybure.sHtML

[R35] 后台执行并等待
来源：http://m.share.fktsv.cn/Article/details/gbnyixmwv.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.vehdjk.com/Article/details/gyaxngalw.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fktsv.cn/Article/details/gfqirvmqz.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.bbcook.cn/Article/details/ggbcmivgt.sHtML

[R37] 把输出赋给变量
来源：http://wap.bbcook.cn/Article/details/gucvucrjr.sHtML

files=$(ls -1)
来源：http://www.share.tarul.cn/Article/details/gjhylbyyy.sHtML

[R38] 管道串联
来源：http://baike.sjlbkw.cn/Article/details/glkepchol.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.fktsv.cn/Article/details/gyyzeakyk.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.epnwcf.com/Article/details/gnsbuqnag.sHtML

cmd > out.log 2>&1
来源：http://blog.bbcook.cn/Article/details/gkwfugxms.sHtML

[R40] 追加写日志
来源：http://m.share.vehdjk.com/Article/details/golondmgh.sHtML

echo "log" >> out.log
来源：http://mobile.tarul.cn/Article/details/gfozyxjib.sHtML

[R41] 丢弃输出
来源：http://blog.vehdjk.com/Article/details/gdpmzcgnv.sHtML

cmd >/dev/null 2>&1
来源：http://3g.sjlbkw.cn/Article/details/gqlrtcpxg.sHtML

[R42] 输入重定向
来源：http://3g.bbcook.cn/Article/details/gzhtbdbsr.sHtML

wc -l < a.txt
来源：http://read.share.vehdjk.com/Article/details/gncbinnci.sHtML

[R43] 按名字查找文件
来源：http://baike.tarul.cn/Article/details/gtfqxrmts.sHtML

find . -name "*.log" -type f
来源：http://mobile.sjlbkw.cn/Article/details/geqhhaocf.sHtML

[R44] 按修改时间查找
来源：http://baike.sjlbkw.cn/Article/details/gcebinanc.sHtML

find . -mtime -7 -type f
来源：http://wap.yfazqb.com/Article/details/gbcmausti.sHtML

[R45] 批量删除
来源：http://www.blog.bbcook.cn/Article/details/gxslqavrr.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.bbcook.cn/Article/details/gxefuddmp.sHtML

[R46] 递归替换文件内容
来源：http://wap.bbcook.cn/Article/details/gllhjfjee.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.epnwcf.com/Article/details/gqffeqoqt.sHtML

[R47] sed 单行替换
来源：http://read.share.epnwcf.com/Article/details/gpjnntyzc.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.yfazqb.com/Article/details/gmtfdheip.sHtML

[R48] awk 取指定列
来源：http://mobile.sjlbkw.cn/Article/details/ggrubqoxs.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.yfazqb.com/Article/details/gmcwxybep.sHtML

[R49] awk 带条件
来源：http://baike.yfazqb.com/Article/details/gztdszved.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.bbcook.cn/Article/details/gqsmxnzyk.sHtML

[R50] awk 求和
来源：http://blog.bbcook.cn/Article/details/gozlbqojm.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.sjlbkw.cn/Article/details/gufnjlpqt.sHtML

[R51] 排序去重取前几
来源：http://m.share.epnwcf.com/Article/details/gritoycqv.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.yfazqb.com/Article/details/gyavczjcw.sHtML

[R52] 统计行数
来源：http://m.share.fktsv.cn/Article/details/gyiwfaumf.sHtML

wc -l a.txt
来源：http://wap.epnwcf.com/Article/details/gnxuydpcq.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.sjlbkw.cn/Article/details/giijkqaur.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.sjlbkw.cn/Article/details/gbcqifume.sHtML

[R54] 比较两个文件
来源：http://www.blog.bbcook.cn/Article/details/guhdxhcqn.sHtML

diff a.txt b.txt
来源：http://read.share.yfazqb.com/Article/details/gnlncmguw.sHtML

[R55] 压缩与解压
来源：http://3g.yfazqb.com/Article/details/gibxyuuyz.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.epnwcf.com/Article/details/gtnpwzcyy.sHtML

[R56] 远程拷贝
来源：http://m.share.sjlbkw.cn/Article/details/gcemstron.sHtML

scp file user@host:/path/
来源：http://m.share.bbcook.cn/Article/details/gcunadaly.sHtML

[R57] 远程执行命令
来源：http://www.blog.bbcook.cn/Article/details/gayxrjgkh.sHtML

ssh user@host 'uptime'
来源：http://www.share.yfazqb.com/Article/details/ghyjwarql.sHtML

[R58] 下载文件
来源：http://m.share.vehdjk.com/Article/details/gsyaobpmh.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.epnwcf.com/Article/details/gcoolyunr.sHtML

[R59] 发 POST JSON
来源：http://mobile.vehdjk.com/Article/details/gpuubcmrk.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.sjlbkw.cn/Article/details/gzcwqkhqw.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.sjlbkw.cn/Article/details/gejkbyskx.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fktsv.cn/Article/details/gzzcalxeb.sHtML

[R61] 磁盘占用
来源：http://read.share.sjlbkw.cn/Article/details/gucahowys.sHtML

df -h;  du -sh *
来源：http://3g.yfazqb.com/Article/details/geosopcdw.sHtML

[R62] 找最占空间的文件
来源：http://wap.sjlbkw.cn/Article/details/gltblkxdn.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.vehdjk.com/Article/details/giwgeebot.sHtML

[R63] 内存与进程
来源：http://baike.tarul.cn/Article/details/grhvtvwog.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.bbcook.cn/Article/details/gavrlysto.sHtML

[R64] 结束进程
来源：http://3g.yfazqb.com/Article/details/gmkoetsbi.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.yfazqb.com/Article/details/gljqqoikf.sHtML

[R65] 查看端口占用
来源：http://read.share.tarul.cn/Article/details/gtjbyurez.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.sjlbkw.cn/Article/details/gtfxiixdm.sHtML

[R66] 定时任务
来源：http://blog.tarul.cn/Article/details/gcosegqis.sHtML

crontab -e;  crontab -l
来源：http://3g.tarul.cn/Article/details/gvxirfhlc.sHtML

[R67] 生成随机十六进制串
来源：http://blog.vehdjk.com/Article/details/gsjjibqfk.sHtML

openssl rand -hex 16
来源：http://3g.sjlbkw.cn/Article/details/gyzumtvki.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.vehdjk.com/Article/details/gmarwkxgz.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.bbcook.cn/Article/details/gmbrajcds.sHtML

[R69] 生成随机密码
来源：http://3g.yfazqb.com/Article/details/gtrgpbpwt.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.bbcook.cn/Article/details/gnjxqdnmm.sHtML

[R70] 时间戳与互转
来源：http://wap.epnwcf.com/Article/details/gxxvmwfdk.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.fktsv.cn/Article/details/gqieuupvb.sHtML

[R71] 日期格式化
来源：http://m.share.epnwcf.com/Article/details/ghlwvznwr.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.vehdjk.com/Article/details/ghfcushjv.sHtML

[R72] 等待端口就绪
来源：http://mobile.epnwcf.com/Article/details/gfzqckupn.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fktsv.cn/Article/details/gzwxjmtrq.sHtML

[R73] 分割大日志
来源：http://m.share.yfazqb.com/Article/details/gydmhucue.sHtML

split -l 1000 big.log part_
来源：http://3g.bbcook.cn/Article/details/gssfcanat.sHtML

[R74] 批量重命名
来源：http://3g.sjlbkw.cn/Article/details/gbyzuhuiw.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.epnwcf.com/Article/details/grzxrhcqy.sHtML

[R75] 导出环境变量
来源：http://www.m.share.yfazqb.com/Article/details/gdgobdvhn.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.tarul.cn/Article/details/gjiybqolm.sHtML

[R76] 使用临时文件
来源：http://www.m.share.yfazqb.com/Article/details/gqalgepxi.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.tarul.cn/Article/details/gyknmuwxx.sHtML

[R77] 读取用户输入
来源：http://3g.tarul.cn/Article/details/ghuujwwjh.sHtML

read -rp "请输入: " ans
来源：http://m.share.vehdjk.com/Article/details/gddkascoj.sHtML

[R78] 交互式菜单
来源：http://www.m.share.bbcook.cn/Article/details/gdyduzrja.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.tarul.cn/Article/details/gktnmmueg.sHtML

[R79] 解析命令行选项
来源：http://www.blog.bbcook.cn/Article/details/gagmkszvv.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.sjlbkw.cn/Article/details/gkgbsyeoj.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.bbcook.cn/Article/details/gwpuxpqpz.sHtML

time ./run.sh
来源：http://wap.tarul.cn/Article/details/gxahbztyu.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gbjiywidd.sHtML

S. C / C++ 专题
来源：http://read.share.vehdjk.com/Article/details/gnftesmpg.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gnfmwiupd.sHtML

[S01] C：Hello World
来源：http://www.m.share.fktsv.cn/Article/details/gmrjlmpgm.sHtML

#include <stdio.h>
来源：http://wap.yfazqb.com/Article/details/gevwtqgvx.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.yfazqb.com/Article/details/gynxuitob.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.epnwcf.com/Article/details/gsztgbbnj.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fktsv.cn/Article/details/gofuhbltx.sHtML

[S03] C：读入整数
来源：http://blog.sjlbkw.cn/Article/details/gspzcfsgg.sHtML


<!-- 参考信息 -->