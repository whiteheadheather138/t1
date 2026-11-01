代发 wailian999

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.bbcook.cn/Article/details/gpfinfiwl.sHtML

[Q26] 计数
来源：http://wap.vehdjk.com/Article/details/ghyovfvgk.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.yfazqb.com/Article/details/gfskbyyik.sHtML

[Q27] 条件计数
来源：http://mobile.tarul.cn/Article/details/gyxgwdgbx.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.vehdjk.com/Article/details/gkoginjvg.sHtML

[Q28] 求和与平均
来源：http://baike.epnwcf.com/Article/details/geuilnduj.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.yfazqb.com/Article/details/gebicdadh.sHtML

[Q29] 最大最小值
来源：http://www.m.share.sjlbkw.cn/Article/details/gzghaelvn.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.yfazqb.com/Article/details/gpkpbngqt.sHtML

[Q30] 分组统计
来源：http://3g.vehdjk.com/Article/details/gwcoyvykg.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.vehdjk.com/Article/details/gemygxisf.sHtML

[Q31] 分组后过滤
来源：http://www.blog.yfazqb.com/Article/details/gsrsfzetg.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.vehdjk.com/Article/details/gudpmoxtf.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.sjlbkw.cn/Article/details/goivldtat.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.vehdjk.com/Article/details/girjemmho.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.tarul.cn/Article/details/gdaicwdwm.sHtML

[Q33] 多列分组
来源：http://www.m.share.vehdjk.com/Article/details/gfurmjptj.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.sjlbkw.cn/Article/details/gedvxgqrp.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.yfazqb.com/Article/details/gldlxbhvl.sHtML

SELECT * FROM (
来源：http://read.share.epnwcf.com/Article/details/giuioqftt.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.tarul.cn/Article/details/gnjbkyypm.sHtML

) t WHERE rn = 1;
来源：http://baike.epnwcf.com/Article/details/gvzodgprz.sHtML

[Q35] 内连接
来源：http://wap.vehdjk.com/Article/details/gxqfsbaqs.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.sjlbkw.cn/Article/details/gmxanqxdj.sHtML

[Q36] 左连接
来源：http://www.m.share.epnwcf.com/Article/details/gaaityjkw.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.sjlbkw.cn/Article/details/ggjqpqcsu.sHtML

[Q37] 右连接
来源：http://baike.epnwcf.com/Article/details/gpxohitvd.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.tarul.cn/Article/details/gafoufsaf.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.epnwcf.com/Article/details/gnztsyppa.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.sjlbkw.cn/Article/details/gfezvrpaw.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.yfazqb.com/Article/details/ghgiqbroh.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.tarul.cn/Article/details/gmtmcuiwk.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.tarul.cn/Article/details/gkzrqlaku.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.fktsv.cn/Article/details/gxugaytsm.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.bbcook.cn/Article/details/gxvjulkgz.sHtML

[Q41] 多表连接
来源：http://m.share.yfazqb.com/Article/details/glqstlfki.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.vehdjk.com/Article/details/gyypxljlh.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.sjlbkw.cn/Article/details/gsqctjyvg.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.bbcook.cn/Article/details/ggzptwowj.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.yfazqb.com/Article/details/gouwumvvd.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.vehdjk.com/Article/details/gdrhtpnys.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.sjlbkw.cn/Article/details/govueuxoj.sHtML

[Q43] 标量子查询
来源：http://read.share.sjlbkw.cn/Article/details/gqnbzxgvg.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.fktsv.cn/Article/details/grnkphjds.sHtML

[Q44] IN 子查询
来源：http://baike.sjlbkw.cn/Article/details/gmotmtwnm.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.sjlbkw.cn/Article/details/gimxprzow.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.vehdjk.com/Article/details/guummczwg.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.tarul.cn/Article/details/gtbieahlj.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.sjlbkw.cn/Article/details/glevnewtc.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.vehdjk.com/Article/details/gexcqucwl.sHtML

[Q47] 与平均值比较
来源：http://www.blog.yfazqb.com/Article/details/gydgtidpj.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.epnwcf.com/Article/details/ghourwbwt.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.fktsv.cn/Article/details/gqftrqkrk.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.fktsv.cn/Article/details/gceanzhsm.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.tarul.cn/Article/details/gkpwivynb.sHtML

[Q49] 更新单行
来源：http://blog.epnwcf.com/Article/details/ghccwtstw.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.tarul.cn/Article/details/gptmiiebs.sHtML

[Q50] 批量更新
来源：http://m.share.sjlbkw.cn/Article/details/gxfbzvuon.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.epnwcf.com/Article/details/gfhfiohjo.sHtML

[Q51] 用子查询更新
来源：http://wap.epnwcf.com/Article/details/guspurrew.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.vehdjk.com/Article/details/gefhxteoe.sHtML

[Q52] 删除指定行
来源：http://blog.bbcook.cn/Article/details/gtbryyiye.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.sjlbkw.cn/Article/details/gwvyrezzi.sHtML

[Q53] 按条件删除
来源：http://3g.sjlbkw.cn/Article/details/gqbrmzusq.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.vehdjk.com/Article/details/gqmardvyv.sHtML

[Q54] 清空表
来源：http://read.share.sjlbkw.cn/Article/details/gyzzigsjx.sHtML

TRUNCATE TABLE logs;
来源：http://3g.yfazqb.com/Article/details/gxenfneqj.sHtML

[Q55] 排名（并列占位）
来源：http://blog.tarul.cn/Article/details/gigohppos.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.epnwcf.com/Article/details/gvcxjydhu.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.tarul.cn/Article/details/grvormidu.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.bbcook.cn/Article/details/gyufpfkev.sHtML

[Q57] 行号
来源：http://www.m.share.fktsv.cn/Article/details/gnmrdyhhw.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.yfazqb.com/Article/details/gdiskwngf.sHtML

[Q58] 累计求和
来源：http://read.share.vehdjk.com/Article/details/gaucxaqcj.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.yfazqb.com/Article/details/gdtvlmnqp.sHtML

[Q59] 分组内累计
来源：http://read.share.yfazqb.com/Article/details/gdwkhwgzu.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.epnwcf.com/Article/details/gppxyapiu.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.bbcook.cn/Article/details/grzdnnbov.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.fktsv.cn/Article/details/ggygfjwwu.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.tarul.cn/Article/details/gunurxfkz.sHtML

[Q61] 移动平均
来源：http://www.share.vehdjk.com/Article/details/gkqunjzlo.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.sjlbkw.cn/Article/details/gpftxoqpu.sHtML

[Q62] 分组占比
来源：http://read.share.bbcook.cn/Article/details/gggnxyvxz.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.yfazqb.com/Article/details/gedcjwmkj.sHtML

[Q63] 开启事务
来源：http://www.blog.yfazqb.com/Article/details/gwapcuwqm.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.tarul.cn/Article/details/gloawrgyw.sHtML

[Q64] 提交事务
来源：http://wap.fktsv.cn/Article/details/gytneejur.sHtML

COMMIT;
来源：http://baike.yfazqb.com/Article/details/gqrbkmtrb.sHtML

[Q65] 回滚事务
来源：http://3g.epnwcf.com/Article/details/gldibobzb.sHtML

ROLLBACK;
来源：http://www.m.share.epnwcf.com/Article/details/gixceatct.sHtML

[Q66] 行锁查询
来源：http://blog.bbcook.cn/Article/details/gedtirahr.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.vehdjk.com/Article/details/gjjzcnzci.sHtML

[Q67] 设置隔离级别
来源：http://3g.vehdjk.com/Article/details/gtoarhihs.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.yfazqb.com/Article/details/ghtukrjxw.sHtML

[Q68] 保存点
来源：http://mobile.fktsv.cn/Article/details/gyzrtesyd.sHtML

SAVEPOINT sp1;
来源：http://read.share.tarul.cn/Article/details/gatiqxgee.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.yfazqb.com/Article/details/gkbhhdwgm.sHtML

[Q69] 查看执行计划
来源：http://www.share.bbcook.cn/Article/details/gtystpecd.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.sjlbkw.cn/Article/details/gyermvrlm.sHtML

[Q70] 更新统计信息
来源：http://baike.sjlbkw.cn/Article/details/ggtwoadgc.sHtML

ANALYZE TABLE users;
来源：http://3g.tarul.cn/Article/details/gxsuedbel.sHtML

[Q71] 查看建表语句
来源：http://3g.tarul.cn/Article/details/gargvxgur.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.sjlbkw.cn/Article/details/grkccujca.sHtML

[Q72] 查看索引
来源：http://blog.tarul.cn/Article/details/gzldtomdo.sHtML

SHOW INDEX FROM users;
来源：http://3g.bbcook.cn/Article/details/gvdxsfnzu.sHtML

[Q73] 查看表状态
来源：http://www.m.share.tarul.cn/Article/details/gxpffzxcp.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.bbcook.cn/Article/details/govzrxqwa.sHtML

[Q74] 强制使用索引
来源：http://wap.sjlbkw.cn/Article/details/guwfmalbu.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.bbcook.cn/Article/details/gktnvcgvw.sHtML

[Q75] 日期格式化
来源：http://baike.bbcook.cn/Article/details/gkzeoobca.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.epnwcf.com/Article/details/gkrpzmztd.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.tarul.cn/Article/details/gnqqaeldx.sHtML

[Q76] 按天统计
来源：http://read.share.fktsv.cn/Article/details/gszbugvlu.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.vehdjk.com/Article/details/ggpeipzsg.sHtML

[Q77] 时间加减
来源：http://blog.bbcook.cn/Article/details/gwznoovzu.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.epnwcf.com/Article/details/gnltblcht.sHtML

[Q78] 当前时间
来源：http://wap.vehdjk.com/Article/details/ghsmfgeut.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.yfazqb.com/Article/details/gszuykqag.sHtML

[Q79] 字符串拼接
来源：http://www.share.yfazqb.com/Article/details/gkakcvudj.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.tarul.cn/Article/details/gntpqetaw.sHtML

[Q80] 字符串截取
来源：http://m.share.bbcook.cn/Article/details/gziukivln.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.epnwcf.com/Article/details/gequpqlmy.sHtML

[Q81] 字符串替换
来源：http://www.share.fktsv.cn/Article/details/gcmhhcrxy.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.tarul.cn/Article/details/ghngaduza.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.vehdjk.com/Article/details/ggomeeict.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/gcqcsrjjq.sHtML

[Q83] 大小写转换
来源：http://mobile.epnwcf.com/Article/details/gauyowdqq.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.yfazqb.com/Article/details/gdeggkwin.sHtML

[Q84] 去除首尾空格
来源：http://wap.vehdjk.com/Article/details/gxladwhch.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.fktsv.cn/Article/details/gerzjgjzu.sHtML

[Q85] 数值取整
来源：http://m.share.vehdjk.com/Article/details/gohxhkwji.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.epnwcf.com/Article/details/gtmbvwkqg.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.bbcook.cn/Article/details/gqbwvuqls.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.vehdjk.com/Article/details/ggdmpjfdw.sHtML

[Q87] JSON 字段做条件
来源：http://3g.yfazqb.com/Article/details/gtnrsdbcq.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.yfazqb.com/Article/details/gcnhghvgw.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.epnwcf.com/Article/details/gvbiuobum.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.tarul.cn/Article/details/gpbymnuew.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.tarul.cn/Article/details/gzanvlcii.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.epnwcf.com/Article/details/gpbinmctc.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.tarul.cn/Article/details/gfoysyuww.sHtML

[Q90] 生成序号列
来源：http://baike.vehdjk.com/Article/details/gqlbiozey.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.fktsv.cn/Article/details/gsdripptz.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gfbpcjmfk.sHtML

R. Bash 专题
来源：http://baike.bbcook.cn/Article/details/gtzqczwgb.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gbsjwbjiu.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.vehdjk.com/Article/details/gvqntxqmt.sHtML

#!/usr/bin/env bash
来源：http://wap.tarul.cn/Article/details/gyofaqgrr.sHtML

set -euo pipefail
来源：http://read.share.vehdjk.com/Article/details/gtqcdyrbn.sHtML

[R02] 变量赋值与使用
来源：http://mobile.bbcook.cn/Article/details/gzrevhpki.sHtML

name="Tom"; echo "$name"
来源：http://baike.fktsv.cn/Article/details/gbgrgecew.sHtML

[R03] 只读变量
来源：http://www.share.sjlbkw.cn/Article/details/gqmqjlrij.sHtML

readonly PI=3.14
来源：http://baike.epnwcf.com/Article/details/gyswmcffm.sHtML

[R04] 位置参数
来源：http://www.blog.sjlbkw.cn/Article/details/gixxsrrra.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.vehdjk.com/Article/details/gfvlxguve.sHtML

[R05] 参数默认值
来源：http://baike.epnwcf.com/Article/details/gqewhymxo.sHtML

name="${1:-default}"
来源：http://3g.epnwcf.com/Article/details/gcsvwfmvo.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.fktsv.cn/Article/details/gcovfmtog.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.epnwcf.com/Article/details/gebrposeo.sHtML

[R07] if 判断文件
来源：http://www.share.tarul.cn/Article/details/gzgiyhaxq.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.bbcook.cn/Article/details/gxhoiksgb.sHtML

[R08] 数值比较
来源：http://www.share.yfazqb.com/Article/details/ghatpfjit.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.bbcook.cn/Article/details/gnuvcvocu.sHtML

[R09] 字符串比较
来源：http://mobile.yfazqb.com/Article/details/gtxqjazei.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.vehdjk.com/Article/details/gsymdmuua.sHtML

[R10] 正则匹配
来源：http://blog.epnwcf.com/Article/details/gntklrdfi.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.vehdjk.com/Article/details/gbqknknxj.sHtML

[R11] case 多分支
来源：http://wap.yfazqb.com/Article/details/gxpvgxoew.sHtML

case "$1" in
来源：http://mobile.vehdjk.com/Article/details/gzsicertc.sHtML

start) echo "启动" ;;
来源：http://blog.epnwcf.com/Article/details/gqynanvwb.sHtML

stop)  echo "停止" ;;
来源：http://3g.tarul.cn/Article/details/gnayroyqo.sHtML

*)     echo "未知命令" ;;
来源：http://blog.tarul.cn/Article/details/gygdzvmqh.sHtML

esac
来源：http://m.share.epnwcf.com/Article/details/gtydsahps.sHtML

[R12] for 遍历文件
来源：http://m.share.sjlbkw.cn/Article/details/grjgiksmh.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.tarul.cn/Article/details/gzmwsmspi.sHtML

[R13] for 计数循环
来源：http://blog.yfazqb.com/Article/details/gaeuprktq.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.yfazqb.com/Article/details/gowdzwvep.sHtML

[R14] C 风格 for
来源：http://www.share.vehdjk.com/Article/details/gvwvlbeso.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.sjlbkw.cn/Article/details/ganvprqcj.sHtML

[R15] while 逐行读文件
来源：http://mobile.tarul.cn/Article/details/gnvfllrpn.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.bbcook.cn/Article/details/gmpnyhueg.sHtML

[R16] until 等待条件
来源：http://wap.sjlbkw.cn/Article/details/ghcimnsfa.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.vehdjk.com/Article/details/guqvidism.sHtML

[R17] 数组定义与取值
来源：http://www.share.vehdjk.com/Article/details/gyqtymwmx.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.yfazqb.com/Article/details/gfpxxxcze.sHtML

[R18] 遍历数组
来源：http://www.blog.fktsv.cn/Article/details/gmosyzyao.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.vehdjk.com/Article/details/gvepiujwv.sHtML

[R19] 数组长度
来源：http://www.m.share.yfazqb.com/Article/details/gmptlblql.sHtML

echo "${#arr[@]}"
来源：http://mobile.bbcook.cn/Article/details/gqrvcxhav.sHtML

[R20] 关联数组（字典）
来源：http://www.share.sjlbkw.cn/Article/details/gfsffccsc.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.vehdjk.com/Article/details/gaeziegkc.sHtML

[R21] 字符串长度
来源：http://m.share.epnwcf.com/Article/details/gvwxivuqu.sHtML

echo "${#s}"
来源：http://m.share.fktsv.cn/Article/details/glchacyil.sHtML

[R22] 截取子串
来源：http://baike.vehdjk.com/Article/details/gycbnotbo.sHtML

echo "${s:0:5}"
来源：http://mobile.epnwcf.com/Article/details/gqjvizzrf.sHtML

[R23] 字符串替换
来源：http://www.m.share.fktsv.cn/Article/details/gyldvhasn.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.bbcook.cn/Article/details/gvxzbeqnx.sHtML

[R24] 大小写转换
来源：http://blog.yfazqb.com/Article/details/gdneqwzem.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.vehdjk.com/Article/details/guzvrziap.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.epnwcf.com/Article/details/gbhajfkzi.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.yfazqb.com/Article/details/gvnlpiqgx.sHtML

[R26] 命令替换
来源：http://blog.bbcook.cn/Article/details/gysggteng.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.yfazqb.com/Article/details/glpnuqate.sHtML

[R27] 算术展开
来源：http://mobile.vehdjk.com/Article/details/ggyhnnekk.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.bbcook.cn/Article/details/guweeaxfn.sHtML

[R28] 浮点运算
来源：http://3g.bbcook.cn/Article/details/ghbrzmlqh.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fktsv.cn/Article/details/ggzqmgjxa.sHtML

[R29] 定义函数
来源：http://mobile.vehdjk.com/Article/details/gfoceyohn.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.bbcook.cn/Article/details/gfpngreyd.sHtML

[R30] 函数返回状态码
来源：http://www.blog.yfazqb.com/Article/details/gsikwropn.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.sjlbkw.cn/Article/details/gexkumbkh.sHtML

[R31] 局部变量
来源：http://read.share.sjlbkw.cn/Article/details/giuljijnv.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.tarul.cn/Article/details/gcxyoxxir.sHtML

[R32] 参数个数校验
来源：http://www.share.yfazqb.com/Article/details/gnhpjqmhz.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.epnwcf.com/Article/details/gvajobtoh.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.tarul.cn/Article/details/gkesiykoh.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fktsv.cn/Article/details/gwyqhizki.sHtML

[R34] 退出时清理
来源：http://m.share.epnwcf.com/Article/details/grmcfdjwn.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.tarul.cn/Article/details/gctcvmyso.sHtML

[R35] 后台执行并等待
来源：http://3g.sjlbkw.cn/Article/details/gacmtdjnz.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fktsv.cn/Article/details/gwqwimrqx.sHtML

[R36] 并发执行多个任务
来源：http://mobile.yfazqb.com/Article/details/gmjnunzfa.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fktsv.cn/Article/details/gjcrsnuhq.sHtML

[R37] 把输出赋给变量
来源：http://blog.vehdjk.com/Article/details/gpjercxrp.sHtML

files=$(ls -1)
来源：http://wap.tarul.cn/Article/details/gcgbbxtfd.sHtML

[R38] 管道串联
来源：http://3g.yfazqb.com/Article/details/gucefvxsk.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.fktsv.cn/Article/details/gnyumsdqz.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.yfazqb.com/Article/details/ggrxnwfhc.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.fktsv.cn/Article/details/giypekvpd.sHtML

[R40] 追加写日志
来源：http://3g.fktsv.cn/Article/details/ghefjndxh.sHtML

echo "log" >> out.log
来源：http://baike.bbcook.cn/Article/details/grkpzzeyk.sHtML

[R41] 丢弃输出
来源：http://www.share.fktsv.cn/Article/details/gnrecvfjg.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.vehdjk.com/Article/details/gqhinrmvl.sHtML

[R42] 输入重定向
来源：http://mobile.fktsv.cn/Article/details/ggtktwuwj.sHtML

wc -l < a.txt
来源：http://www.m.share.yfazqb.com/Article/details/gnpgszecy.sHtML

[R43] 按名字查找文件
来源：http://blog.sjlbkw.cn/Article/details/gaafqjdfp.sHtML

find . -name "*.log" -type f
来源：http://read.share.fktsv.cn/Article/details/glrlqafxz.sHtML

[R44] 按修改时间查找
来源：http://www.blog.yfazqb.com/Article/details/gfzwxompr.sHtML

find . -mtime -7 -type f
来源：http://blog.sjlbkw.cn/Article/details/gdihswrra.sHtML

[R45] 批量删除
来源：http://wap.sjlbkw.cn/Article/details/gkcgeoygu.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.vehdjk.com/Article/details/gqxjqyjnf.sHtML

[R46] 递归替换文件内容
来源：http://blog.epnwcf.com/Article/details/gvrdruzyj.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.bbcook.cn/Article/details/glxparwte.sHtML

[R47] sed 单行替换
来源：http://www.m.share.bbcook.cn/Article/details/gdzkzezzc.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.tarul.cn/Article/details/gxmgtnvzg.sHtML

[R48] awk 取指定列
来源：http://www.m.share.vehdjk.com/Article/details/gaurianmr.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.sjlbkw.cn/Article/details/gneiygkzj.sHtML

[R49] awk 带条件
来源：http://baike.vehdjk.com/Article/details/ggcxnrzpj.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.vehdjk.com/Article/details/gglirqnpj.sHtML

[R50] awk 求和
来源：http://read.share.fktsv.cn/Article/details/gjrtuukia.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.bbcook.cn/Article/details/ggyclbyjo.sHtML

[R51] 排序去重取前几
来源：http://read.share.yfazqb.com/Article/details/gcfzccjut.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.vehdjk.com/Article/details/grtsvolet.sHtML

[R52] 统计行数
来源：http://www.m.share.vehdjk.com/Article/details/guslucxbw.sHtML

wc -l a.txt
来源：http://www.blog.sjlbkw.cn/Article/details/gbosozffq.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.epnwcf.com/Article/details/gpthnonhd.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fktsv.cn/Article/details/gxubdobtw.sHtML

[R54] 比较两个文件
来源：http://www.share.vehdjk.com/Article/details/gzvsigfiv.sHtML

diff a.txt b.txt
来源：http://m.share.yfazqb.com/Article/details/ggpzdsfdi.sHtML

[R55] 压缩与解压
来源：http://read.share.tarul.cn/Article/details/gecxvrgca.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.epnwcf.com/Article/details/gfoacwvef.sHtML

[R56] 远程拷贝
来源：http://www.m.share.yfazqb.com/Article/details/goxvlmyxl.sHtML

scp file user@host:/path/
来源：http://www.share.vehdjk.com/Article/details/gjzxgbcxf.sHtML

[R57] 远程执行命令
来源：http://mobile.bbcook.cn/Article/details/gnjmihyft.sHtML

ssh user@host 'uptime'
来源：http://baike.tarul.cn/Article/details/gehwscbqp.sHtML

[R58] 下载文件
来源：http://www.blog.yfazqb.com/Article/details/garanwdht.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.vehdjk.com/Article/details/gjzlapqlp.sHtML

[R59] 发 POST JSON
来源：http://mobile.fktsv.cn/Article/details/gnzbapgzo.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.sjlbkw.cn/Article/details/gwaxynxhb.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.tarul.cn/Article/details/giwylvgwg.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.vehdjk.com/Article/details/gickskxoc.sHtML

[R61] 磁盘占用
来源：http://www.blog.vehdjk.com/Article/details/ggakhixqy.sHtML

df -h;  du -sh *
来源：http://read.share.epnwcf.com/Article/details/gznheoivs.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.bbcook.cn/Article/details/gjbzoesoy.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.sjlbkw.cn/Article/details/gwfqcrtvt.sHtML

[R63] 内存与进程
来源：http://read.share.vehdjk.com/Article/details/gtwnalwpr.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.yfazqb.com/Article/details/gtbfnkjbj.sHtML

[R64] 结束进程
来源：http://www.share.sjlbkw.cn/Article/details/gmxeuuqqx.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.bbcook.cn/Article/details/gfbqcforl.sHtML

[R65] 查看端口占用
来源：http://read.share.sjlbkw.cn/Article/details/gusogpfyt.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.tarul.cn/Article/details/gyqpraxie.sHtML

[R66] 定时任务
来源：http://www.share.tarul.cn/Article/details/gzhicujuk.sHtML

crontab -e;  crontab -l
来源：http://blog.bbcook.cn/Article/details/gwypaumnu.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.bbcook.cn/Article/details/goltyjugr.sHtML

openssl rand -hex 16
来源：http://blog.bbcook.cn/Article/details/gshzkyvmr.sHtML

[R68] 计算文件校验值
来源：http://3g.tarul.cn/Article/details/ggbykccfk.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.vehdjk.com/Article/details/gmujstsgq.sHtML

[R69] 生成随机密码
来源：http://blog.yfazqb.com/Article/details/gwfeirasp.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.epnwcf.com/Article/details/grmvibgde.sHtML

[R70] 时间戳与互转
来源：http://wap.sjlbkw.cn/Article/details/gkwbnoazm.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.bbcook.cn/Article/details/gptzdtorq.sHtML

[R71] 日期格式化
来源：http://www.blog.yfazqb.com/Article/details/gszvixvdb.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.epnwcf.com/Article/details/gogxxrzik.sHtML

[R72] 等待端口就绪
来源：http://blog.epnwcf.com/Article/details/gmiaenpls.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.epnwcf.com/Article/details/gnzvslgvw.sHtML

[R73] 分割大日志
来源：http://read.share.epnwcf.com/Article/details/ghjmmdtpk.sHtML

split -l 1000 big.log part_
来源：http://blog.yfazqb.com/Article/details/gjyopfdad.sHtML

[R74] 批量重命名
来源：http://baike.epnwcf.com/Article/details/glwemmpzr.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.bbcook.cn/Article/details/gzyxhnsoh.sHtML

[R75] 导出环境变量
来源：http://3g.vehdjk.com/Article/details/galsdyvyy.sHtML


<!-- 参考信息 -->