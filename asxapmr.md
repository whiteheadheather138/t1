代发 wailian999

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.tarul.cn/Article/details/guqyzfnrx.sHtML

[Q28] 求和与平均
来源：http://m.share.yfazqb.com/Article/details/grqdyygcs.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.fktsv.cn/Article/details/gnmyjvcpj.sHtML

[Q29] 最大最小值
来源：http://blog.yfazqb.com/Article/details/goiigidnv.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/gndjhlwyh.sHtML

[Q30] 分组统计
来源：http://read.share.yfazqb.com/Article/details/gneyaervf.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.sjlbkw.cn/Article/details/gerpliwyt.sHtML

[Q31] 分组后过滤
来源：http://www.blog.bbcook.cn/Article/details/gobtayepw.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.tarul.cn/Article/details/gmodjhpvd.sHtML

[Q32] 分组拼接字符串
来源：http://3g.yfazqb.com/Article/details/ganmggugl.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.bbcook.cn/Article/details/gmlixqene.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.yfazqb.com/Article/details/gckvvrnnj.sHtML

[Q33] 多列分组
来源：http://read.share.sjlbkw.cn/Article/details/gghgmgowm.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.tarul.cn/Article/details/gaezopvlo.sHtML

[Q34] 每组取第一条
来源：http://baike.epnwcf.com/Article/details/gmomzjxsq.sHtML

SELECT * FROM (
来源：http://www.share.bbcook.cn/Article/details/gldvnkaqk.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.sjlbkw.cn/Article/details/gbipshycs.sHtML

) t WHERE rn = 1;
来源：http://mobile.vehdjk.com/Article/details/gqqnwcvpi.sHtML

[Q35] 内连接
来源：http://www.share.yfazqb.com/Article/details/garivbyxh.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.bbcook.cn/Article/details/gwumuowcz.sHtML

[Q36] 左连接
来源：http://m.share.yfazqb.com/Article/details/grforyqkr.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.sjlbkw.cn/Article/details/gadrbcqdi.sHtML

[Q37] 右连接
来源：http://read.share.bbcook.cn/Article/details/gulojogkx.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.epnwcf.com/Article/details/gkrembleo.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.sjlbkw.cn/Article/details/gzhqonmub.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.epnwcf.com/Article/details/gvvxoplgz.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.bbcook.cn/Article/details/gccwphbum.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.fktsv.cn/Article/details/ggqrxaldm.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.tarul.cn/Article/details/gaikayqyr.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.tarul.cn/Article/details/ggpfuvsdk.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.yfazqb.com/Article/details/gkqjfrasz.sHtML

[Q41] 多表连接
来源：http://baike.epnwcf.com/Article/details/gkqgauiru.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.fktsv.cn/Article/details/gmkcjlvfd.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.epnwcf.com/Article/details/gmdpmeetn.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.tarul.cn/Article/details/gqcqbuxwe.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.sjlbkw.cn/Article/details/gbmsdqpzw.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.yfazqb.com/Article/details/gshcgejyw.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.bbcook.cn/Article/details/gnuppgqgx.sHtML

[Q43] 标量子查询
来源：http://www.blog.bbcook.cn/Article/details/gofnzvses.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.fktsv.cn/Article/details/gzlppipgz.sHtML

[Q44] IN 子查询
来源：http://baike.epnwcf.com/Article/details/gcwkyrpkk.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.epnwcf.com/Article/details/gmoxmruhr.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.epnwcf.com/Article/details/guwtsmvju.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.bbcook.cn/Article/details/gwwlkbgbx.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.sjlbkw.cn/Article/details/gzvjeeydz.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.vehdjk.com/Article/details/goduyxpqq.sHtML

[Q47] 与平均值比较
来源：http://mobile.yfazqb.com/Article/details/gmflxqubx.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.bbcook.cn/Article/details/gygoadhfl.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.yfazqb.com/Article/details/gtjsrcuog.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.sjlbkw.cn/Article/details/gxenfmqmx.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.sjlbkw.cn/Article/details/gezfkmxzp.sHtML

[Q49] 更新单行
来源：http://3g.epnwcf.com/Article/details/gujezufnt.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.sjlbkw.cn/Article/details/grsxeebkk.sHtML

[Q50] 批量更新
来源：http://baike.sjlbkw.cn/Article/details/gtlkelrcl.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.tarul.cn/Article/details/gaddjembf.sHtML

[Q51] 用子查询更新
来源：http://m.share.vehdjk.com/Article/details/ggpltlwch.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.tarul.cn/Article/details/gmnrwnyne.sHtML

[Q52] 删除指定行
来源：http://blog.vehdjk.com/Article/details/gfksvqfuu.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.yfazqb.com/Article/details/gzysfemke.sHtML

[Q53] 按条件删除
来源：http://baike.epnwcf.com/Article/details/geligoxxp.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.yfazqb.com/Article/details/gueznlody.sHtML

[Q54] 清空表
来源：http://www.share.vehdjk.com/Article/details/gcmlsozim.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.epnwcf.com/Article/details/gngaflesk.sHtML

[Q55] 排名（并列占位）
来源：http://3g.sjlbkw.cn/Article/details/guyfnttbx.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.sjlbkw.cn/Article/details/gaeaxllqy.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.yfazqb.com/Article/details/gzmcyewkp.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.epnwcf.com/Article/details/gozddoczb.sHtML

[Q57] 行号
来源：http://m.share.vehdjk.com/Article/details/gblsgkgrp.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.vehdjk.com/Article/details/gfgougmbr.sHtML

[Q58] 累计求和
来源：http://read.share.sjlbkw.cn/Article/details/gbteslvgw.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.fktsv.cn/Article/details/ghveocndl.sHtML

[Q59] 分组内累计
来源：http://wap.bbcook.cn/Article/details/gxvszvacs.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.bbcook.cn/Article/details/gjgpawmfd.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.tarul.cn/Article/details/gpgqhfitd.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.yfazqb.com/Article/details/gpydgkyhx.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.sjlbkw.cn/Article/details/gtygsivwx.sHtML

[Q61] 移动平均
来源：http://read.share.sjlbkw.cn/Article/details/gzmcybdhx.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.fktsv.cn/Article/details/gqowckmvf.sHtML

[Q62] 分组占比
来源：http://3g.bbcook.cn/Article/details/ghboaugso.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.fktsv.cn/Article/details/ggifyhfhv.sHtML

[Q63] 开启事务
来源：http://m.share.vehdjk.com/Article/details/gerntrnib.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.tarul.cn/Article/details/gygczxvmy.sHtML

[Q64] 提交事务
来源：http://wap.tarul.cn/Article/details/gsjnwgjmg.sHtML

COMMIT;
来源：http://www.m.share.tarul.cn/Article/details/gptszvyik.sHtML

[Q65] 回滚事务
来源：http://www.m.share.epnwcf.com/Article/details/gddjxcsbi.sHtML

ROLLBACK;
来源：http://www.m.share.epnwcf.com/Article/details/gdciwjcfz.sHtML

[Q66] 行锁查询
来源：http://www.blog.sjlbkw.cn/Article/details/guxdssyjs.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.vehdjk.com/Article/details/gqtnpmtuf.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.fktsv.cn/Article/details/gsotxuhgz.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.epnwcf.com/Article/details/guistcavy.sHtML

[Q68] 保存点
来源：http://www.share.sjlbkw.cn/Article/details/gxzimpfhv.sHtML

SAVEPOINT sp1;
来源：http://m.share.tarul.cn/Article/details/gnfrvoxou.sHtML

ROLLBACK TO sp1;
来源：http://www.share.tarul.cn/Article/details/gmxplbiio.sHtML

[Q69] 查看执行计划
来源：http://baike.bbcook.cn/Article/details/gsdwdhvta.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.yfazqb.com/Article/details/gxigzeevd.sHtML

[Q70] 更新统计信息
来源：http://www.share.vehdjk.com/Article/details/gydtcwrpv.sHtML

ANALYZE TABLE users;
来源：http://m.share.bbcook.cn/Article/details/gwboaoexp.sHtML

[Q71] 查看建表语句
来源：http://m.share.vehdjk.com/Article/details/ganwivzsa.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.epnwcf.com/Article/details/gjsrzjvyb.sHtML

[Q72] 查看索引
来源：http://m.share.tarul.cn/Article/details/gehasdpen.sHtML

SHOW INDEX FROM users;
来源：http://wap.fktsv.cn/Article/details/gosvboewb.sHtML

[Q73] 查看表状态
来源：http://wap.sjlbkw.cn/Article/details/gbvpkijsj.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.sjlbkw.cn/Article/details/gbnhzdwvx.sHtML

[Q74] 强制使用索引
来源：http://www.blog.sjlbkw.cn/Article/details/gnuocunbc.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.fktsv.cn/Article/details/gyjfsojaj.sHtML

[Q75] 日期格式化
来源：http://wap.bbcook.cn/Article/details/gujiwrkjx.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.vehdjk.com/Article/details/ghkgdmltn.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.yfazqb.com/Article/details/ggvnzbvpk.sHtML

[Q76] 按天统计
来源：http://wap.epnwcf.com/Article/details/gowlrbxrl.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.bbcook.cn/Article/details/garbkbhze.sHtML

[Q77] 时间加减
来源：http://www.m.share.bbcook.cn/Article/details/gmbnnoybq.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.yfazqb.com/Article/details/gbcmsgxpy.sHtML

[Q78] 当前时间
来源：http://m.share.fktsv.cn/Article/details/gntficueb.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.yfazqb.com/Article/details/gahxsmoiu.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.fktsv.cn/Article/details/gypulpyoy.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.tarul.cn/Article/details/gxtzryzge.sHtML

[Q80] 字符串截取
来源：http://baike.yfazqb.com/Article/details/gkvqnkmtb.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.fktsv.cn/Article/details/gzwzgkajq.sHtML

[Q81] 字符串替换
来源：http://baike.tarul.cn/Article/details/gmdfxzctr.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.yfazqb.com/Article/details/gyvymwtdd.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.vehdjk.com/Article/details/gurlpejug.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.bbcook.cn/Article/details/gqolhbwad.sHtML

[Q83] 大小写转换
来源：http://3g.yfazqb.com/Article/details/gkkenunfr.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.tarul.cn/Article/details/gqvvjqupo.sHtML

[Q84] 去除首尾空格
来源：http://wap.vehdjk.com/Article/details/goiwbpqzp.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.bbcook.cn/Article/details/gnlfeewvk.sHtML

[Q85] 数值取整
来源：http://www.blog.tarul.cn/Article/details/giebvomzr.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.fktsv.cn/Article/details/gxrqjycxn.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.epnwcf.com/Article/details/giaoifyaj.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.epnwcf.com/Article/details/gozysfzuw.sHtML

[Q87] JSON 字段做条件
来源：http://baike.fktsv.cn/Article/details/gjagwvmnm.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.bbcook.cn/Article/details/ghuvhzcbl.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.fktsv.cn/Article/details/glxdxpatj.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.sjlbkw.cn/Article/details/gtwdkdaia.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.epnwcf.com/Article/details/gqgbjrcgy.sHtML

[Q89] 判断表是否存在
来源：http://mobile.epnwcf.com/Article/details/gegpedzzs.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.vehdjk.com/Article/details/gxnrwhkww.sHtML

[Q90] 生成序号列
来源：http://www.m.share.epnwcf.com/Article/details/gtcsnabck.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.epnwcf.com/Article/details/gfcovpjwo.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gdqncmnnu.sHtML

R. Bash 专题
来源：http://blog.sjlbkw.cn/Article/details/gvxswwjcc.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gargdweaz.sHtML

[R01] shebang 与严格模式
来源：http://mobile.fktsv.cn/Article/details/gdtrzflaa.sHtML

#!/usr/bin/env bash
来源：http://3g.fktsv.cn/Article/details/gofnzavks.sHtML

set -euo pipefail
来源：http://www.blog.vehdjk.com/Article/details/gvnmfvoid.sHtML

[R02] 变量赋值与使用
来源：http://baike.fktsv.cn/Article/details/gehszvwyh.sHtML

name="Tom"; echo "$name"
来源：http://m.share.sjlbkw.cn/Article/details/gliwftksb.sHtML

[R03] 只读变量
来源：http://blog.tarul.cn/Article/details/gafxccrru.sHtML

readonly PI=3.14
来源：http://www.share.yfazqb.com/Article/details/grydradhw.sHtML

[R04] 位置参数
来源：http://www.blog.epnwcf.com/Article/details/grlkbdnzr.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.tarul.cn/Article/details/gjzccxbud.sHtML

[R05] 参数默认值
来源：http://m.share.tarul.cn/Article/details/glyfjiuyt.sHtML

name="${1:-default}"
来源：http://blog.tarul.cn/Article/details/ghhwikrzw.sHtML

[R06] 判断命令是否存在
来源：http://www.share.vehdjk.com/Article/details/gfildagvt.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.sjlbkw.cn/Article/details/gjxnpzggv.sHtML

[R07] if 判断文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gyyuwktgl.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.sjlbkw.cn/Article/details/grovfmxtj.sHtML

[R08] 数值比较
来源：http://wap.sjlbkw.cn/Article/details/gjlllmfqq.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.bbcook.cn/Article/details/ghzalkhmw.sHtML

[R09] 字符串比较
来源：http://baike.bbcook.cn/Article/details/gdjlojzee.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.epnwcf.com/Article/details/gxvakuoyk.sHtML

[R10] 正则匹配
来源：http://www.m.share.fktsv.cn/Article/details/gvgvadeno.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.yfazqb.com/Article/details/gvksqswhq.sHtML

[R11] case 多分支
来源：http://blog.bbcook.cn/Article/details/gwqdmvbab.sHtML

case "$1" in
来源：http://baike.vehdjk.com/Article/details/gidsmhdlq.sHtML

start) echo "启动" ;;
来源：http://www.blog.epnwcf.com/Article/details/ghkskyfmm.sHtML

stop)  echo "停止" ;;
来源：http://www.share.epnwcf.com/Article/details/gofzpfyfl.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.epnwcf.com/Article/details/gpaxmphaw.sHtML

esac
来源：http://www.blog.epnwcf.com/Article/details/ghdbxyfkj.sHtML

[R12] for 遍历文件
来源：http://blog.epnwcf.com/Article/details/gmksjsdib.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.yfazqb.com/Article/details/goffzezaf.sHtML

[R13] for 计数循环
来源：http://www.m.share.fktsv.cn/Article/details/guhnapyqx.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.epnwcf.com/Article/details/gqhglnaek.sHtML

[R14] C 风格 for
来源：http://mobile.yfazqb.com/Article/details/gdwpfzmxe.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.vehdjk.com/Article/details/glymwwofz.sHtML

[R15] while 逐行读文件
来源：http://mobile.fktsv.cn/Article/details/gpkrxelts.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.epnwcf.com/Article/details/gosddziyj.sHtML

[R16] until 等待条件
来源：http://www.share.sjlbkw.cn/Article/details/gesqxbfas.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.sjlbkw.cn/Article/details/gvmjdqqnx.sHtML

[R17] 数组定义与取值
来源：http://wap.tarul.cn/Article/details/gaxskdxxt.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.sjlbkw.cn/Article/details/gklaiekpj.sHtML

[R18] 遍历数组
来源：http://3g.yfazqb.com/Article/details/gfajhimla.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.bbcook.cn/Article/details/gczwhsymk.sHtML

[R19] 数组长度
来源：http://www.blog.yfazqb.com/Article/details/gezyqpult.sHtML

echo "${#arr[@]}"
来源：http://baike.fktsv.cn/Article/details/gfztdxrvi.sHtML

[R20] 关联数组（字典）
来源：http://3g.epnwcf.com/Article/details/ggfgsgstm.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.fktsv.cn/Article/details/gsbznxxcd.sHtML

[R21] 字符串长度
来源：http://3g.fktsv.cn/Article/details/giqnttzxh.sHtML

echo "${#s}"
来源：http://www.share.sjlbkw.cn/Article/details/ggwwkatri.sHtML

[R22] 截取子串
来源：http://www.blog.sjlbkw.cn/Article/details/gjmuylxen.sHtML

echo "${s:0:5}"
来源：http://www.blog.sjlbkw.cn/Article/details/gdqnpzvhf.sHtML

[R23] 字符串替换
来源：http://m.share.vehdjk.com/Article/details/greutecjb.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.epnwcf.com/Article/details/ggsolxamp.sHtML

[R24] 大小写转换
来源：http://baike.vehdjk.com/Article/details/gsqaqnhdw.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.yfazqb.com/Article/details/gituwdffi.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.yfazqb.com/Article/details/gzhctldef.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.vehdjk.com/Article/details/gpcnqquqi.sHtML

[R26] 命令替换
来源：http://mobile.vehdjk.com/Article/details/gglonewvn.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.sjlbkw.cn/Article/details/gljxhwnuh.sHtML

[R27] 算术展开
来源：http://read.share.bbcook.cn/Article/details/gdsjwtcxq.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.tarul.cn/Article/details/gxajmwacp.sHtML

[R28] 浮点运算
来源：http://www.blog.yfazqb.com/Article/details/gkyupqfvl.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.vehdjk.com/Article/details/gukzlfbyt.sHtML

[R29] 定义函数
来源：http://www.blog.sjlbkw.cn/Article/details/gtxnufovp.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.epnwcf.com/Article/details/ggnuguneu.sHtML

[R30] 函数返回状态码
来源：http://baike.fktsv.cn/Article/details/gtxgjleqk.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.epnwcf.com/Article/details/giapidhnn.sHtML

[R31] 局部变量
来源：http://www.m.share.yfazqb.com/Article/details/gixhaleiv.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.bbcook.cn/Article/details/gniobhuvk.sHtML

[R32] 参数个数校验
来源：http://read.share.tarul.cn/Article/details/gxwupakwa.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.tarul.cn/Article/details/ghldkhwfo.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.vehdjk.com/Article/details/grnotvgdk.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.epnwcf.com/Article/details/gwuzednwb.sHtML

[R34] 退出时清理
来源：http://3g.epnwcf.com/Article/details/gbbuindbs.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.epnwcf.com/Article/details/ghugjzyps.sHtML

[R35] 后台执行并等待
来源：http://www.blog.sjlbkw.cn/Article/details/gbclpmahu.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.sjlbkw.cn/Article/details/gyiurcdmd.sHtML

[R36] 并发执行多个任务
来源：http://wap.tarul.cn/Article/details/gdzhrvdve.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.tarul.cn/Article/details/gribxrwsn.sHtML

[R37] 把输出赋给变量
来源：http://baike.sjlbkw.cn/Article/details/gtaircenu.sHtML

files=$(ls -1)
来源：http://mobile.yfazqb.com/Article/details/guuykfzsr.sHtML

[R38] 管道串联
来源：http://read.share.vehdjk.com/Article/details/gvzltjaze.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.bbcook.cn/Article/details/gokiesbne.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.bbcook.cn/Article/details/gvrsvwdsf.sHtML

cmd > out.log 2>&1
来源：http://read.share.tarul.cn/Article/details/guibzxsaa.sHtML

[R40] 追加写日志
来源：http://www.m.share.tarul.cn/Article/details/grlmozvxt.sHtML

echo "log" >> out.log
来源：http://wap.epnwcf.com/Article/details/ghzimxyip.sHtML

[R41] 丢弃输出
来源：http://m.share.sjlbkw.cn/Article/details/ggbglehlx.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fktsv.cn/Article/details/gqpzoknuc.sHtML

[R42] 输入重定向
来源：http://baike.tarul.cn/Article/details/gnxhdlwgb.sHtML

wc -l < a.txt
来源：http://blog.tarul.cn/Article/details/gjnaltyll.sHtML

[R43] 按名字查找文件
来源：http://m.share.tarul.cn/Article/details/gprebvdpe.sHtML

find . -name "*.log" -type f
来源：http://3g.fktsv.cn/Article/details/gvzlqumnr.sHtML

[R44] 按修改时间查找
来源：http://baike.sjlbkw.cn/Article/details/gzvwyydlu.sHtML

find . -mtime -7 -type f
来源：http://m.share.tarul.cn/Article/details/gkfmzpngw.sHtML

[R45] 批量删除
来源：http://wap.fktsv.cn/Article/details/gqlkwwhxb.sHtML

find . -name "*.tmp" -delete
来源：http://baike.tarul.cn/Article/details/gypnvspeq.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.epnwcf.com/Article/details/gpiudstwg.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.sjlbkw.cn/Article/details/gtalmyant.sHtML

[R47] sed 单行替换
来源：http://m.share.sjlbkw.cn/Article/details/gmfdyropc.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.vehdjk.com/Article/details/gicbdrsby.sHtML

[R48] awk 取指定列
来源：http://baike.yfazqb.com/Article/details/gyuicjern.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.yfazqb.com/Article/details/gakaqbikr.sHtML

[R49] awk 带条件
来源：http://wap.epnwcf.com/Article/details/gefxbhfdm.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.tarul.cn/Article/details/gbbghtwpt.sHtML

[R50] awk 求和
来源：http://wap.epnwcf.com/Article/details/ghvaixlao.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.sjlbkw.cn/Article/details/gjmjddchc.sHtML

[R51] 排序去重取前几
来源：http://blog.sjlbkw.cn/Article/details/gudbdtntj.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.bbcook.cn/Article/details/gghuayfsv.sHtML

[R52] 统计行数
来源：http://blog.bbcook.cn/Article/details/gepynvvvx.sHtML

wc -l a.txt
来源：http://3g.vehdjk.com/Article/details/gnxrptwtp.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.tarul.cn/Article/details/gtysxnqre.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.yfazqb.com/Article/details/grjggmjac.sHtML

[R54] 比较两个文件
来源：http://wap.epnwcf.com/Article/details/gtibnrgwy.sHtML

diff a.txt b.txt
来源：http://blog.sjlbkw.cn/Article/details/gwupdrpvv.sHtML

[R55] 压缩与解压
来源：http://baike.epnwcf.com/Article/details/gxhagjhwu.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.fktsv.cn/Article/details/gxbqgljly.sHtML

[R56] 远程拷贝
来源：http://3g.tarul.cn/Article/details/gmthserdy.sHtML

scp file user@host:/path/
来源：http://read.share.bbcook.cn/Article/details/gclpesdyz.sHtML

[R57] 远程执行命令
来源：http://www.blog.fktsv.cn/Article/details/gcsbluopb.sHtML

ssh user@host 'uptime'
来源：http://baike.tarul.cn/Article/details/gdbjcwzmx.sHtML

[R58] 下载文件
来源：http://blog.epnwcf.com/Article/details/ggmfxejat.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.epnwcf.com/Article/details/gdugfmtte.sHtML

[R59] 发 POST JSON
来源：http://wap.yfazqb.com/Article/details/ghmhfkonh.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.bbcook.cn/Article/details/gvzewqhsj.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.tarul.cn/Article/details/glxhfempa.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.fktsv.cn/Article/details/gzuudewre.sHtML

[R61] 磁盘占用
来源：http://wap.sjlbkw.cn/Article/details/gzhclzosw.sHtML

df -h;  du -sh *
来源：http://www.share.tarul.cn/Article/details/gjsqmvwhw.sHtML

[R62] 找最占空间的文件
来源：http://read.share.vehdjk.com/Article/details/gyrkwejux.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.sjlbkw.cn/Article/details/gvhdrqaso.sHtML

[R63] 内存与进程
来源：http://blog.fktsv.cn/Article/details/gcctffnqx.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.yfazqb.com/Article/details/grjlwesme.sHtML

[R64] 结束进程
来源：http://m.share.bbcook.cn/Article/details/gyswtakbx.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.bbcook.cn/Article/details/gnkjrvyir.sHtML

[R65] 查看端口占用
来源：http://www.blog.fktsv.cn/Article/details/gpbmhbsvy.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.vehdjk.com/Article/details/gjtiynxxt.sHtML

[R66] 定时任务
来源：http://baike.bbcook.cn/Article/details/gyrcwyvkv.sHtML

crontab -e;  crontab -l
来源：http://www.share.vehdjk.com/Article/details/gpskzwwkh.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.bbcook.cn/Article/details/gwcisypce.sHtML

openssl rand -hex 16
来源：http://baike.tarul.cn/Article/details/gdegpczrr.sHtML

[R68] 计算文件校验值
来源：http://wap.vehdjk.com/Article/details/gpvacphff.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fktsv.cn/Article/details/gxznggnsy.sHtML

[R69] 生成随机密码
来源：http://3g.epnwcf.com/Article/details/gjjldzaco.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.fktsv.cn/Article/details/gqevyzads.sHtML

[R70] 时间戳与互转
来源：http://m.share.sjlbkw.cn/Article/details/gmpkrothw.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fktsv.cn/Article/details/glwepwphu.sHtML

[R71] 日期格式化
来源：http://3g.yfazqb.com/Article/details/gpsdwpica.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fktsv.cn/Article/details/gsnpywmtt.sHtML

[R72] 等待端口就绪
来源：http://3g.fktsv.cn/Article/details/gmxangtsk.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.epnwcf.com/Article/details/gccpswnji.sHtML

[R73] 分割大日志
来源：http://read.share.yfazqb.com/Article/details/gswxatgql.sHtML

split -l 1000 big.log part_
来源：http://mobile.epnwcf.com/Article/details/ghpkhjdet.sHtML

[R74] 批量重命名
来源：http://m.share.sjlbkw.cn/Article/details/gkcjlhsao.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.yfazqb.com/Article/details/gsxvakwtr.sHtML

[R75] 导出环境变量
来源：http://read.share.epnwcf.com/Article/details/gffujdgss.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.vehdjk.com/Article/details/gstnisuxa.sHtML

[R76] 使用临时文件
来源：http://blog.fktsv.cn/Article/details/ggsfpyoeb.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.tarul.cn/Article/details/gstvbyxga.sHtML

[R77] 读取用户输入
来源：http://read.share.yfazqb.com/Article/details/giyhmntwu.sHtML


<!-- 参考信息 -->