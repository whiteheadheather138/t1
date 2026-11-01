代发 wailian999

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.vehdjk.com/Article/details/gfyyzhlqb.sHtML

[Q22] 排序
来源：http://baike.sjlbkw.cn/Article/details/ghzrnnnva.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.vehdjk.com/Article/details/gkiedbwcq.sHtML

[Q23] 分页
来源：http://blog.epnwcf.com/Article/details/gkkqyrvgh.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.sjlbkw.cn/Article/details/gjpfkwzbr.sHtML

[Q24] 去重
来源：http://baike.yfazqb.com/Article/details/giwszrdqu.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.yfazqb.com/Article/details/gomrghdmb.sHtML

[Q25] 只取前 N 条
来源：http://blog.epnwcf.com/Article/details/gaywolqah.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.fktsv.cn/Article/details/gyjlwdmyx.sHtML

[Q26] 计数
来源：http://baike.yfazqb.com/Article/details/glprwjqfo.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.bbcook.cn/Article/details/gocrfehbd.sHtML

[Q27] 条件计数
来源：http://blog.sjlbkw.cn/Article/details/gsjapebac.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.yfazqb.com/Article/details/gdcmpsnpe.sHtML

[Q28] 求和与平均
来源：http://m.share.sjlbkw.cn/Article/details/gpwqckjxf.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.vehdjk.com/Article/details/gpkmlpesg.sHtML

[Q29] 最大最小值
来源：http://blog.sjlbkw.cn/Article/details/gdztdltre.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/gplyyerzm.sHtML

[Q30] 分组统计
来源：http://mobile.fktsv.cn/Article/details/glfkekhse.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.fktsv.cn/Article/details/gbxyokkqo.sHtML

[Q31] 分组后过滤
来源：http://m.share.sjlbkw.cn/Article/details/gddlkfjpk.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.bbcook.cn/Article/details/grjqwnkkt.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.fktsv.cn/Article/details/gigimiiuu.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.yfazqb.com/Article/details/gobsynxwv.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.yfazqb.com/Article/details/gnzrpqxwa.sHtML

[Q33] 多列分组
来源：http://m.share.fktsv.cn/Article/details/gubovghkr.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.vehdjk.com/Article/details/gqvhfuxfx.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.yfazqb.com/Article/details/gdaaldcyd.sHtML

SELECT * FROM (
来源：http://m.share.tarul.cn/Article/details/gjljhlcdy.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.bbcook.cn/Article/details/goxwdewau.sHtML

) t WHERE rn = 1;
来源：http://3g.tarul.cn/Article/details/gbsnaqvoa.sHtML

[Q35] 内连接
来源：http://wap.fktsv.cn/Article/details/gqwdlqemt.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fktsv.cn/Article/details/gouavsfwi.sHtML

[Q36] 左连接
来源：http://3g.epnwcf.com/Article/details/gmquvqovo.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.yfazqb.com/Article/details/gltatxnwh.sHtML

[Q37] 右连接
来源：http://m.share.vehdjk.com/Article/details/gkoohtayh.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.fktsv.cn/Article/details/grvjwkljk.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.bbcook.cn/Article/details/gnebsercc.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.tarul.cn/Article/details/gkhljdedj.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.tarul.cn/Article/details/gbetfbqjb.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.sjlbkw.cn/Article/details/gwuuhzevk.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.sjlbkw.cn/Article/details/gqbtyqwvd.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.tarul.cn/Article/details/gdvlvbhxv.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.vehdjk.com/Article/details/gngnbrlcb.sHtML

[Q41] 多表连接
来源：http://3g.vehdjk.com/Article/details/gniegxzzh.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.tarul.cn/Article/details/gytdokkfd.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.fktsv.cn/Article/details/gycztltxf.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.yfazqb.com/Article/details/gnekxcrep.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.bbcook.cn/Article/details/gtltqroub.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.vehdjk.com/Article/details/gtrcnnqyx.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.fktsv.cn/Article/details/gzryjflgs.sHtML

[Q43] 标量子查询
来源：http://www.share.sjlbkw.cn/Article/details/gftwjkvrt.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.epnwcf.com/Article/details/gukhjlvpi.sHtML

[Q44] IN 子查询
来源：http://blog.tarul.cn/Article/details/gcoanrvsy.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.yfazqb.com/Article/details/gibrlmpif.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.vehdjk.com/Article/details/gmittwqby.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.bbcook.cn/Article/details/gfzdifiqu.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.tarul.cn/Article/details/gzejcyjcf.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.vehdjk.com/Article/details/gqlrlhiqx.sHtML

[Q47] 与平均值比较
来源：http://baike.fktsv.cn/Article/details/gxuzpspoe.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.yfazqb.com/Article/details/gmsyopxfo.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.bbcook.cn/Article/details/gtnezunbk.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.epnwcf.com/Article/details/gqiuxqbfx.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.vehdjk.com/Article/details/gwmnwvpai.sHtML

[Q49] 更新单行
来源：http://www.share.vehdjk.com/Article/details/gyjbnzgnb.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.sjlbkw.cn/Article/details/gxzzhndhg.sHtML

[Q50] 批量更新
来源：http://www.m.share.fktsv.cn/Article/details/gvfmdzwfr.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.fktsv.cn/Article/details/gsnavwpis.sHtML

[Q51] 用子查询更新
来源：http://m.share.vehdjk.com/Article/details/gnxondgdn.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.fktsv.cn/Article/details/groxtukud.sHtML

[Q52] 删除指定行
来源：http://www.m.share.vehdjk.com/Article/details/gjzajzpzr.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.sjlbkw.cn/Article/details/gqizvspls.sHtML

[Q53] 按条件删除
来源：http://www.m.share.yfazqb.com/Article/details/gjqswfegx.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.sjlbkw.cn/Article/details/gmpnfgtfg.sHtML

[Q54] 清空表
来源：http://m.share.vehdjk.com/Article/details/gjvuormcw.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.epnwcf.com/Article/details/gclmntoxp.sHtML

[Q55] 排名（并列占位）
来源：http://3g.tarul.cn/Article/details/gemcoflfu.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.sjlbkw.cn/Article/details/glwyngvxp.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.vehdjk.com/Article/details/gdgyvagaz.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.fktsv.cn/Article/details/gauxpjnak.sHtML

[Q57] 行号
来源：http://read.share.sjlbkw.cn/Article/details/grjfzrxbt.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/gexxnvuwg.sHtML

[Q58] 累计求和
来源：http://read.share.fktsv.cn/Article/details/gafpigtia.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.sjlbkw.cn/Article/details/gxjchzdtr.sHtML

[Q59] 分组内累计
来源：http://wap.yfazqb.com/Article/details/gwlexlycu.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.sjlbkw.cn/Article/details/gepavsude.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.vehdjk.com/Article/details/gfzbibexc.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.epnwcf.com/Article/details/gbbziwucc.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.epnwcf.com/Article/details/guyqplokd.sHtML

[Q61] 移动平均
来源：http://www.share.yfazqb.com/Article/details/glbzrytgo.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.epnwcf.com/Article/details/gbaqqusds.sHtML

[Q62] 分组占比
来源：http://blog.bbcook.cn/Article/details/gbyhefrdx.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.bbcook.cn/Article/details/gdoavdrvr.sHtML

[Q63] 开启事务
来源：http://www.blog.bbcook.cn/Article/details/gzljuywqa.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.vehdjk.com/Article/details/gwwabaies.sHtML

[Q64] 提交事务
来源：http://www.blog.fktsv.cn/Article/details/gpojtzdhj.sHtML

COMMIT;
来源：http://mobile.epnwcf.com/Article/details/gukqsddan.sHtML

[Q65] 回滚事务
来源：http://www.blog.vehdjk.com/Article/details/gekidijfm.sHtML

ROLLBACK;
来源：http://www.share.epnwcf.com/Article/details/gaxnyqxxm.sHtML

[Q66] 行锁查询
来源：http://www.blog.yfazqb.com/Article/details/gbvrlaizw.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.bbcook.cn/Article/details/gqebbhqtu.sHtML

[Q67] 设置隔离级别
来源：http://read.share.vehdjk.com/Article/details/gaquofudn.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.sjlbkw.cn/Article/details/gsnzanhig.sHtML

[Q68] 保存点
来源：http://m.share.fktsv.cn/Article/details/gztssugrz.sHtML

SAVEPOINT sp1;
来源：http://www.blog.bbcook.cn/Article/details/gyvjwwhhp.sHtML

ROLLBACK TO sp1;
来源：http://blog.tarul.cn/Article/details/gemgzxelx.sHtML

[Q69] 查看执行计划
来源：http://mobile.yfazqb.com/Article/details/gqwikueba.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.tarul.cn/Article/details/gsxycuuiq.sHtML

[Q70] 更新统计信息
来源：http://3g.yfazqb.com/Article/details/gflstcbjj.sHtML

ANALYZE TABLE users;
来源：http://blog.bbcook.cn/Article/details/gvnriaeoj.sHtML

[Q71] 查看建表语句
来源：http://mobile.sjlbkw.cn/Article/details/gervojzfg.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.tarul.cn/Article/details/gaszxiomm.sHtML

[Q72] 查看索引
来源：http://baike.vehdjk.com/Article/details/gbfxtwwhs.sHtML

SHOW INDEX FROM users;
来源：http://3g.sjlbkw.cn/Article/details/gxjnkysmn.sHtML

[Q73] 查看表状态
来源：http://www.share.vehdjk.com/Article/details/gjfkiplxi.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.tarul.cn/Article/details/gzrfagsox.sHtML

[Q74] 强制使用索引
来源：http://www.share.fktsv.cn/Article/details/gxxhrrbld.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.vehdjk.com/Article/details/gwusvvgch.sHtML

[Q75] 日期格式化
来源：http://read.share.bbcook.cn/Article/details/gfcffalzy.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.tarul.cn/Article/details/gtgbvjojz.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.epnwcf.com/Article/details/gifxuiagg.sHtML

[Q76] 按天统计
来源：http://www.blog.sjlbkw.cn/Article/details/grsjkghzy.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.sjlbkw.cn/Article/details/gbnyxugrt.sHtML

[Q77] 时间加减
来源：http://read.share.sjlbkw.cn/Article/details/grlxbmbdx.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.epnwcf.com/Article/details/gkacnteba.sHtML

[Q78] 当前时间
来源：http://www.blog.vehdjk.com/Article/details/gjiblfrum.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.bbcook.cn/Article/details/gkybdakol.sHtML

[Q79] 字符串拼接
来源：http://www.blog.vehdjk.com/Article/details/gesjhtgtm.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.epnwcf.com/Article/details/gflmzcmim.sHtML

[Q80] 字符串截取
来源：http://www.m.share.sjlbkw.cn/Article/details/gemazmgsf.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.tarul.cn/Article/details/gsgkvftke.sHtML

[Q81] 字符串替换
来源：http://m.share.bbcook.cn/Article/details/gpsgnxsfi.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.vehdjk.com/Article/details/gumcfwpvu.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.tarul.cn/Article/details/gduirpink.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.fktsv.cn/Article/details/gsdoljhrt.sHtML

[Q83] 大小写转换
来源：http://www.blog.fktsv.cn/Article/details/gyvqyadtd.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.epnwcf.com/Article/details/goufmmawb.sHtML

[Q84] 去除首尾空格
来源：http://www.share.yfazqb.com/Article/details/ghnsexxjr.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.fktsv.cn/Article/details/gacouwdij.sHtML

[Q85] 数值取整
来源：http://3g.vehdjk.com/Article/details/ggrtsrbrs.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.bbcook.cn/Article/details/gywfvgxgr.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.tarul.cn/Article/details/gnnkcneha.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.vehdjk.com/Article/details/gdreefvbj.sHtML

[Q87] JSON 字段做条件
来源：http://baike.fktsv.cn/Article/details/gcaobjnfe.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.sjlbkw.cn/Article/details/gorxtborg.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.fktsv.cn/Article/details/gfpdkhogt.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.tarul.cn/Article/details/glqvjkpaw.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.yfazqb.com/Article/details/gfqhwdgfh.sHtML

[Q89] 判断表是否存在
来源：http://blog.vehdjk.com/Article/details/gooukzeut.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.epnwcf.com/Article/details/gzfzskdvs.sHtML

[Q90] 生成序号列
来源：http://blog.epnwcf.com/Article/details/gpljgekwz.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.fktsv.cn/Article/details/gkeyzcgjd.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/ggfoifolp.sHtML

R. Bash 专题
来源：http://baike.fktsv.cn/Article/details/gayqargsu.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gmnesirdw.sHtML

[R01] shebang 与严格模式
来源：http://wap.epnwcf.com/Article/details/gzaigobgn.sHtML

#!/usr/bin/env bash
来源：http://www.share.yfazqb.com/Article/details/gpbzpokuv.sHtML

set -euo pipefail
来源：http://3g.epnwcf.com/Article/details/gehxuxawz.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.epnwcf.com/Article/details/gwrvwkghk.sHtML

name="Tom"; echo "$name"
来源：http://m.share.yfazqb.com/Article/details/grvzdmiii.sHtML

[R03] 只读变量
来源：http://m.share.yfazqb.com/Article/details/gyepyfqnj.sHtML

readonly PI=3.14
来源：http://3g.bbcook.cn/Article/details/gmlxxvgmk.sHtML

[R04] 位置参数
来源：http://read.share.bbcook.cn/Article/details/grignggpq.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.vehdjk.com/Article/details/gexyiryct.sHtML

[R05] 参数默认值
来源：http://read.share.sjlbkw.cn/Article/details/gglxqcdys.sHtML

name="${1:-default}"
来源：http://www.share.vehdjk.com/Article/details/gkyauqgvx.sHtML

[R06] 判断命令是否存在
来源：http://read.share.fktsv.cn/Article/details/gtmyttslg.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.sjlbkw.cn/Article/details/gazjhvmhe.sHtML

[R07] if 判断文件
来源：http://mobile.tarul.cn/Article/details/gxfpryzij.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.epnwcf.com/Article/details/gngveqxes.sHtML

[R08] 数值比较
来源：http://read.share.sjlbkw.cn/Article/details/gnitavcnb.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.yfazqb.com/Article/details/gbtmodxrd.sHtML

[R09] 字符串比较
来源：http://read.share.fktsv.cn/Article/details/gmoikcehb.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.epnwcf.com/Article/details/gyhqrucqy.sHtML

[R10] 正则匹配
来源：http://blog.tarul.cn/Article/details/guvnoqfsm.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.epnwcf.com/Article/details/gygktqjqr.sHtML

[R11] case 多分支
来源：http://www.blog.tarul.cn/Article/details/grrlddsrm.sHtML

case "$1" in
来源：http://read.share.vehdjk.com/Article/details/gnbporxhe.sHtML

start) echo "启动" ;;
来源：http://mobile.fktsv.cn/Article/details/ghpijucws.sHtML

stop)  echo "停止" ;;
来源：http://m.share.sjlbkw.cn/Article/details/govcodrdv.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.fktsv.cn/Article/details/grmwtqtpn.sHtML

esac
来源：http://www.blog.epnwcf.com/Article/details/groqipicg.sHtML

[R12] for 遍历文件
来源：http://www.blog.yfazqb.com/Article/details/gyuzehlbd.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.vehdjk.com/Article/details/gkheiomko.sHtML

[R13] for 计数循环
来源：http://www.share.sjlbkw.cn/Article/details/gijexfcyy.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.sjlbkw.cn/Article/details/gbugqhvnf.sHtML

[R14] C 风格 for
来源：http://mobile.yfazqb.com/Article/details/gmshvwhzp.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fktsv.cn/Article/details/gzpqkrrfj.sHtML

[R15] while 逐行读文件
来源：http://blog.vehdjk.com/Article/details/grvpyybet.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.fktsv.cn/Article/details/giytmkemx.sHtML

[R16] until 等待条件
来源：http://wap.epnwcf.com/Article/details/gwkgpfaan.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.yfazqb.com/Article/details/glwednleh.sHtML

[R17] 数组定义与取值
来源：http://www.share.epnwcf.com/Article/details/gfqjtkfpb.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.sjlbkw.cn/Article/details/gvjnxojwe.sHtML

[R18] 遍历数组
来源：http://3g.bbcook.cn/Article/details/gxekeiawm.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.bbcook.cn/Article/details/gfhoywdyg.sHtML

[R19] 数组长度
来源：http://wap.epnwcf.com/Article/details/gcvvfjkxv.sHtML

echo "${#arr[@]}"
来源：http://m.share.epnwcf.com/Article/details/gpdlecwkd.sHtML

[R20] 关联数组（字典）
来源：http://m.share.sjlbkw.cn/Article/details/guxnujgzw.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.bbcook.cn/Article/details/gjjsormvo.sHtML

[R21] 字符串长度
来源：http://www.m.share.tarul.cn/Article/details/genqtnepe.sHtML

echo "${#s}"
来源：http://www.m.share.vehdjk.com/Article/details/gkniicsci.sHtML

[R22] 截取子串
来源：http://www.blog.yfazqb.com/Article/details/gmfqcenom.sHtML

echo "${s:0:5}"
来源：http://wap.sjlbkw.cn/Article/details/gcfjbvbsz.sHtML

[R23] 字符串替换
来源：http://www.blog.tarul.cn/Article/details/gkmapmtph.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.yfazqb.com/Article/details/gcwhnhzzo.sHtML

[R24] 大小写转换
来源：http://m.share.epnwcf.com/Article/details/gopweejrc.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.yfazqb.com/Article/details/gmaahmrkc.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.vehdjk.com/Article/details/gbcinwkwx.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.vehdjk.com/Article/details/gsnkaemwa.sHtML

[R26] 命令替换
来源：http://wap.fktsv.cn/Article/details/gluabnwpq.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.epnwcf.com/Article/details/gturmvqac.sHtML

[R27] 算术展开
来源：http://blog.bbcook.cn/Article/details/gixrljmeh.sHtML

echo $((1 + 2 * 3))
来源：http://wap.tarul.cn/Article/details/gxvbtegeb.sHtML

[R28] 浮点运算
来源：http://blog.vehdjk.com/Article/details/ghtzfygni.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fktsv.cn/Article/details/ggjwzkdnk.sHtML

[R29] 定义函数
来源：http://baike.yfazqb.com/Article/details/gcnqcgrgx.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.fktsv.cn/Article/details/geystipku.sHtML

[R30] 函数返回状态码
来源：http://www.blog.vehdjk.com/Article/details/gaxcedeil.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.sjlbkw.cn/Article/details/gkerdkrwj.sHtML

[R31] 局部变量
来源：http://baike.vehdjk.com/Article/details/gzbxzjmse.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.yfazqb.com/Article/details/goowwfojt.sHtML

[R32] 参数个数校验
来源：http://www.blog.vehdjk.com/Article/details/glefpcanr.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.epnwcf.com/Article/details/gubzpzjsi.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.sjlbkw.cn/Article/details/gbzxosenx.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fktsv.cn/Article/details/gfiipxvat.sHtML

[R34] 退出时清理
来源：http://baike.sjlbkw.cn/Article/details/gfwhtyzhw.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.sjlbkw.cn/Article/details/gkowsgkzm.sHtML

[R35] 后台执行并等待
来源：http://3g.yfazqb.com/Article/details/gxcpxeryx.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.yfazqb.com/Article/details/gbqevnbsq.sHtML

[R36] 并发执行多个任务
来源：http://www.share.bbcook.cn/Article/details/gifylisav.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.bbcook.cn/Article/details/gvtfueupg.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.yfazqb.com/Article/details/gaxvmdvco.sHtML

files=$(ls -1)
来源：http://blog.vehdjk.com/Article/details/gnjyxlrwi.sHtML

[R38] 管道串联
来源：http://www.blog.yfazqb.com/Article/details/gmlwxagaz.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.sjlbkw.cn/Article/details/gjlfpgrdt.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.vehdjk.com/Article/details/gkpfarqlx.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.sjlbkw.cn/Article/details/gnyudpwes.sHtML

[R40] 追加写日志
来源：http://www.blog.tarul.cn/Article/details/gxspcrmnt.sHtML

echo "log" >> out.log
来源：http://www.blog.epnwcf.com/Article/details/gdhldptsy.sHtML

[R41] 丢弃输出
来源：http://www.share.epnwcf.com/Article/details/gykailvkw.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.sjlbkw.cn/Article/details/gwvvrbahw.sHtML

[R42] 输入重定向
来源：http://blog.tarul.cn/Article/details/gkveaalho.sHtML

wc -l < a.txt
来源：http://baike.fktsv.cn/Article/details/gzqjodmdl.sHtML

[R43] 按名字查找文件
来源：http://www.share.fktsv.cn/Article/details/gznezzcwr.sHtML

find . -name "*.log" -type f
来源：http://www.blog.sjlbkw.cn/Article/details/gkwxjdmhp.sHtML

[R44] 按修改时间查找
来源：http://www.share.sjlbkw.cn/Article/details/gdinuhhpm.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.epnwcf.com/Article/details/geosdfhvy.sHtML

[R45] 批量删除
来源：http://mobile.bbcook.cn/Article/details/gfzfatjyg.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.epnwcf.com/Article/details/gdqvomnlo.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fktsv.cn/Article/details/gucxvkngi.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fktsv.cn/Article/details/gnqtvampc.sHtML

[R47] sed 单行替换
来源：http://blog.fktsv.cn/Article/details/gyljpoqnd.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.yfazqb.com/Article/details/gqsrjxtmq.sHtML

[R48] awk 取指定列
来源：http://blog.fktsv.cn/Article/details/gxmrvgbal.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.bbcook.cn/Article/details/gjmunufza.sHtML

[R49] awk 带条件
来源：http://3g.tarul.cn/Article/details/gzcidsyxk.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.tarul.cn/Article/details/gvztbysmb.sHtML

[R50] awk 求和
来源：http://m.share.yfazqb.com/Article/details/gvaptsykx.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.tarul.cn/Article/details/grqxdlgik.sHtML

[R51] 排序去重取前几
来源：http://www.share.fktsv.cn/Article/details/gatiqaljl.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.bbcook.cn/Article/details/gcliwpius.sHtML

[R52] 统计行数
来源：http://www.m.share.fktsv.cn/Article/details/gwawndjvn.sHtML

wc -l a.txt
来源：http://www.blog.vehdjk.com/Article/details/gpgaldbbh.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.yfazqb.com/Article/details/gykepkxfj.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.vehdjk.com/Article/details/gspbwphqi.sHtML

[R54] 比较两个文件
来源：http://www.share.fktsv.cn/Article/details/gtfniwltf.sHtML

diff a.txt b.txt
来源：http://wap.bbcook.cn/Article/details/gpefgksyx.sHtML

[R55] 压缩与解压
来源：http://baike.fktsv.cn/Article/details/gdupkyhju.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.tarul.cn/Article/details/gkhytugxn.sHtML

[R56] 远程拷贝
来源：http://www.blog.tarul.cn/Article/details/gurzdtxal.sHtML

scp file user@host:/path/
来源：http://3g.fktsv.cn/Article/details/gqhxyofwu.sHtML

[R57] 远程执行命令
来源：http://www.m.share.sjlbkw.cn/Article/details/gofucevzv.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.yfazqb.com/Article/details/goabhikil.sHtML

[R58] 下载文件
来源：http://www.share.tarul.cn/Article/details/gvhetdrja.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.epnwcf.com/Article/details/gtygkjsld.sHtML

[R59] 发 POST JSON
来源：http://baike.fktsv.cn/Article/details/gqjuxguqs.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.bbcook.cn/Article/details/gvgpxtfbv.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.yfazqb.com/Article/details/gvrsdpvck.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.fktsv.cn/Article/details/gqggqifrn.sHtML

[R61] 磁盘占用
来源：http://read.share.yfazqb.com/Article/details/gqzneaqvr.sHtML

df -h;  du -sh *
来源：http://read.share.epnwcf.com/Article/details/gpskujdlt.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.epnwcf.com/Article/details/gsgfvzyex.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.vehdjk.com/Article/details/gnbbcfbzx.sHtML

[R63] 内存与进程
来源：http://blog.epnwcf.com/Article/details/gickkyhxy.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.yfazqb.com/Article/details/gimybukmv.sHtML

[R64] 结束进程
来源：http://wap.vehdjk.com/Article/details/geqhpcwpe.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.sjlbkw.cn/Article/details/gshurgkqd.sHtML

[R65] 查看端口占用
来源：http://wap.fktsv.cn/Article/details/gbspenazy.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.yfazqb.com/Article/details/gviihzgts.sHtML

[R66] 定时任务
来源：http://blog.bbcook.cn/Article/details/gzxbhxmtn.sHtML

crontab -e;  crontab -l
来源：http://www.blog.epnwcf.com/Article/details/gukpizkss.sHtML

[R67] 生成随机十六进制串
来源：http://wap.sjlbkw.cn/Article/details/gdbzhdpbb.sHtML

openssl rand -hex 16
来源：http://www.m.share.fktsv.cn/Article/details/gmpqqufgo.sHtML

[R68] 计算文件校验值
来源：http://read.share.vehdjk.com/Article/details/gumvpurvh.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.vehdjk.com/Article/details/guccjmtwc.sHtML

[R69] 生成随机密码
来源：http://m.share.fktsv.cn/Article/details/giwxkdiky.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.epnwcf.com/Article/details/gxhjisxfg.sHtML

[R70] 时间戳与互转
来源：http://3g.yfazqb.com/Article/details/groyzkkoc.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fktsv.cn/Article/details/gfisjtudi.sHtML

[R71] 日期格式化
来源：http://www.blog.sjlbkw.cn/Article/details/gwcowdywt.sHtML


<!-- 参考信息 -->