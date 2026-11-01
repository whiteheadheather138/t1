代发 wailian999

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.epnwcf.com/Article/details/glakowims.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.bbcook.cn/Article/details/gmxdjzhko.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.tarul.cn/Article/details/ghfwzbrqh.sHtML

[Q19] 范围查询
来源：http://blog.yfazqb.com/Article/details/gtzhpxsfl.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.tarul.cn/Article/details/gmqsxbprw.sHtML

[Q20] IN 列表
来源：http://blog.vehdjk.com/Article/details/ghnmcalll.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.bbcook.cn/Article/details/gvwpwiwgb.sHtML

[Q21] 空值判断
来源：http://mobile.vehdjk.com/Article/details/gxyleelzq.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.sjlbkw.cn/Article/details/gmdsjilln.sHtML

[Q22] 排序
来源：http://www.share.bbcook.cn/Article/details/gtmblivry.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.yfazqb.com/Article/details/ghmvjbwoo.sHtML

[Q23] 分页
来源：http://read.share.epnwcf.com/Article/details/gwtyykssg.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.tarul.cn/Article/details/gnedrmhys.sHtML

[Q24] 去重
来源：http://wap.vehdjk.com/Article/details/gwoeuazdz.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.vehdjk.com/Article/details/gabapoamb.sHtML

[Q25] 只取前 N 条
来源：http://read.share.epnwcf.com/Article/details/gjbzbwmym.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.epnwcf.com/Article/details/gwcvaokqt.sHtML

[Q26] 计数
来源：http://blog.tarul.cn/Article/details/gnlezcifs.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.sjlbkw.cn/Article/details/gmtipndqg.sHtML

[Q27] 条件计数
来源：http://blog.yfazqb.com/Article/details/gudruuqve.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.fktsv.cn/Article/details/gvcltjedt.sHtML

[Q28] 求和与平均
来源：http://blog.vehdjk.com/Article/details/gfwkyfwdv.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.fktsv.cn/Article/details/gzzmnlmni.sHtML

[Q29] 最大最小值
来源：http://www.share.sjlbkw.cn/Article/details/gfotxqdee.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.epnwcf.com/Article/details/gqktquohu.sHtML

[Q30] 分组统计
来源：http://m.share.bbcook.cn/Article/details/gmnkmzblu.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.sjlbkw.cn/Article/details/gecxddbcb.sHtML

[Q31] 分组后过滤
来源：http://wap.sjlbkw.cn/Article/details/gftomdxse.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.yfazqb.com/Article/details/gejmcjmxk.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.tarul.cn/Article/details/gmmmhzgic.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.fktsv.cn/Article/details/gzglpyyqa.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.bbcook.cn/Article/details/gpxlalnpa.sHtML

[Q33] 多列分组
来源：http://www.share.fktsv.cn/Article/details/gxqisngaf.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.sjlbkw.cn/Article/details/guhozissa.sHtML

[Q34] 每组取第一条
来源：http://www.share.sjlbkw.cn/Article/details/gfrmmmlfk.sHtML

SELECT * FROM (
来源：http://3g.sjlbkw.cn/Article/details/gddoqumsz.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.sjlbkw.cn/Article/details/ggtpqxpry.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.sjlbkw.cn/Article/details/gmyaptrur.sHtML

[Q35] 内连接
来源：http://baike.sjlbkw.cn/Article/details/gzattiknf.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.fktsv.cn/Article/details/gifisfpfl.sHtML

[Q36] 左连接
来源：http://baike.vehdjk.com/Article/details/gwtbkxpke.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.yfazqb.com/Article/details/gsesflomj.sHtML

[Q37] 右连接
来源：http://m.share.fktsv.cn/Article/details/gyvodhura.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.fktsv.cn/Article/details/gvbseycdu.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.sjlbkw.cn/Article/details/gsemcaofi.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.bbcook.cn/Article/details/gtxsuiexf.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.bbcook.cn/Article/details/graxqyrql.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.sjlbkw.cn/Article/details/glosljchy.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.vehdjk.com/Article/details/glrqvoqqt.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.epnwcf.com/Article/details/gzjwttwut.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.tarul.cn/Article/details/ggftdbfrp.sHtML

[Q41] 多表连接
来源：http://mobile.epnwcf.com/Article/details/gfbfddppg.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.epnwcf.com/Article/details/glyrxvjdb.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.yfazqb.com/Article/details/grmwqxscj.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.yfazqb.com/Article/details/gxjcrzhoj.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.yfazqb.com/Article/details/gdpobmwzu.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.epnwcf.com/Article/details/gkzleofhi.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.vehdjk.com/Article/details/gqqftxrtt.sHtML

[Q43] 标量子查询
来源：http://wap.bbcook.cn/Article/details/gohupvrad.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.tarul.cn/Article/details/gmotvskdm.sHtML

[Q44] IN 子查询
来源：http://baike.vehdjk.com/Article/details/gilcgihfg.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.vehdjk.com/Article/details/gxkzfckva.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.tarul.cn/Article/details/gjuwcocca.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.epnwcf.com/Article/details/grrqqitdu.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.sjlbkw.cn/Article/details/grurfeubf.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.epnwcf.com/Article/details/gwwqrqxoy.sHtML

[Q47] 与平均值比较
来源：http://blog.epnwcf.com/Article/details/gbiqhilkt.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.tarul.cn/Article/details/gwtrkirem.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.vehdjk.com/Article/details/gweajpgdp.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.sjlbkw.cn/Article/details/glehjqxbe.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.fktsv.cn/Article/details/gfoyauneu.sHtML

[Q49] 更新单行
来源：http://mobile.tarul.cn/Article/details/gbjcwlvoj.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.fktsv.cn/Article/details/gllglzyra.sHtML

[Q50] 批量更新
来源：http://www.share.epnwcf.com/Article/details/gmcyzglwh.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.epnwcf.com/Article/details/gcxygeufw.sHtML

[Q51] 用子查询更新
来源：http://3g.sjlbkw.cn/Article/details/gjqxgzpqz.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.yfazqb.com/Article/details/gshaeuudi.sHtML

[Q52] 删除指定行
来源：http://m.share.tarul.cn/Article/details/gclxfakhb.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.tarul.cn/Article/details/gvlcazgrn.sHtML

[Q53] 按条件删除
来源：http://wap.vehdjk.com/Article/details/gwjcmuhdh.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.vehdjk.com/Article/details/gahcveevn.sHtML

[Q54] 清空表
来源：http://blog.vehdjk.com/Article/details/gfiwtrbcm.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.bbcook.cn/Article/details/gwywoctnw.sHtML

[Q55] 排名（并列占位）
来源：http://baike.bbcook.cn/Article/details/gdyumlnpk.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.fktsv.cn/Article/details/gqzhklrfi.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.sjlbkw.cn/Article/details/gevwthvzw.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.epnwcf.com/Article/details/gtixcaral.sHtML

[Q57] 行号
来源：http://mobile.bbcook.cn/Article/details/gvmmcranl.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.tarul.cn/Article/details/gfjotvocw.sHtML

[Q58] 累计求和
来源：http://www.share.epnwcf.com/Article/details/guorgsxyd.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.epnwcf.com/Article/details/gxypskbgs.sHtML

[Q59] 分组内累计
来源：http://mobile.epnwcf.com/Article/details/gczplsoln.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.sjlbkw.cn/Article/details/gulhfopkr.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.bbcook.cn/Article/details/gujfzydqh.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.fktsv.cn/Article/details/gsdtrdnru.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.tarul.cn/Article/details/gglfoxcry.sHtML

[Q61] 移动平均
来源：http://read.share.yfazqb.com/Article/details/gxyvcnjfz.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.bbcook.cn/Article/details/gziisasad.sHtML

[Q62] 分组占比
来源：http://www.blog.vehdjk.com/Article/details/gdthdxazd.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.vehdjk.com/Article/details/gqnliqwmv.sHtML

[Q63] 开启事务
来源：http://wap.bbcook.cn/Article/details/guwtaotbf.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.bbcook.cn/Article/details/gpygvrfpb.sHtML

[Q64] 提交事务
来源：http://www.blog.tarul.cn/Article/details/gxrytzwgd.sHtML

COMMIT;
来源：http://3g.vehdjk.com/Article/details/gpiyyfkrp.sHtML

[Q65] 回滚事务
来源：http://www.blog.vehdjk.com/Article/details/gsppqahqk.sHtML

ROLLBACK;
来源：http://www.m.share.sjlbkw.cn/Article/details/gnmtadowo.sHtML

[Q66] 行锁查询
来源：http://www.share.sjlbkw.cn/Article/details/gykpudqqm.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.vehdjk.com/Article/details/gropzpyst.sHtML

[Q67] 设置隔离级别
来源：http://wap.tarul.cn/Article/details/glgwdwpwa.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.sjlbkw.cn/Article/details/gnvmzrtkj.sHtML

[Q68] 保存点
来源：http://www.share.fktsv.cn/Article/details/gvjuiiwvo.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.bbcook.cn/Article/details/gftirkavs.sHtML

ROLLBACK TO sp1;
来源：http://read.share.yfazqb.com/Article/details/gvektcoph.sHtML

[Q69] 查看执行计划
来源：http://mobile.vehdjk.com/Article/details/gwsxgteoc.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.fktsv.cn/Article/details/gdrjceizz.sHtML

[Q70] 更新统计信息
来源：http://m.share.bbcook.cn/Article/details/gdvozyesp.sHtML

ANALYZE TABLE users;
来源：http://mobile.fktsv.cn/Article/details/gxbnbpmno.sHtML

[Q71] 查看建表语句
来源：http://wap.vehdjk.com/Article/details/grocuydfg.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.vehdjk.com/Article/details/gigqxabhq.sHtML

[Q72] 查看索引
来源：http://3g.epnwcf.com/Article/details/goxnrfzxi.sHtML

SHOW INDEX FROM users;
来源：http://mobile.tarul.cn/Article/details/gjtskpqij.sHtML

[Q73] 查看表状态
来源：http://wap.fktsv.cn/Article/details/gqpnvhvev.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.epnwcf.com/Article/details/guhhjedvx.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.vehdjk.com/Article/details/gfggusrno.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.sjlbkw.cn/Article/details/gegilpgiu.sHtML

[Q75] 日期格式化
来源：http://3g.bbcook.cn/Article/details/gxittsrcg.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.vehdjk.com/Article/details/gahavwrxu.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.epnwcf.com/Article/details/gwvssrykd.sHtML

[Q76] 按天统计
来源：http://www.blog.yfazqb.com/Article/details/gmqgttdtg.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.fktsv.cn/Article/details/gviwfxtdh.sHtML

[Q77] 时间加减
来源：http://www.blog.fktsv.cn/Article/details/ghizonddc.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.sjlbkw.cn/Article/details/gujwyoayc.sHtML

[Q78] 当前时间
来源：http://mobile.yfazqb.com/Article/details/gjllfkohi.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.sjlbkw.cn/Article/details/gxumwubhv.sHtML

[Q79] 字符串拼接
来源：http://3g.fktsv.cn/Article/details/gblgofqhq.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.fktsv.cn/Article/details/gxaefavgg.sHtML

[Q80] 字符串截取
来源：http://www.share.epnwcf.com/Article/details/gkccdpcfi.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.bbcook.cn/Article/details/guaexarnd.sHtML

[Q81] 字符串替换
来源：http://baike.fktsv.cn/Article/details/ggjwhqbxb.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.epnwcf.com/Article/details/gbzzlmmhb.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.tarul.cn/Article/details/gjxjkxjtc.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.vehdjk.com/Article/details/grpiomfwm.sHtML

[Q83] 大小写转换
来源：http://baike.vehdjk.com/Article/details/gosrelntu.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.vehdjk.com/Article/details/gtdhbjpbh.sHtML

[Q84] 去除首尾空格
来源：http://www.share.bbcook.cn/Article/details/gehntjvag.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.vehdjk.com/Article/details/gsdneplyl.sHtML

[Q85] 数值取整
来源：http://www.m.share.epnwcf.com/Article/details/gptbendtm.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.bbcook.cn/Article/details/gzqhlmycy.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.fktsv.cn/Article/details/gptbdygap.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.sjlbkw.cn/Article/details/gvbuqwdpo.sHtML

[Q87] JSON 字段做条件
来源：http://wap.vehdjk.com/Article/details/gweuiqbeh.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.epnwcf.com/Article/details/gcapcdnac.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.vehdjk.com/Article/details/glugwvciw.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.fktsv.cn/Article/details/granmxtip.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.yfazqb.com/Article/details/ggicygznw.sHtML

[Q89] 判断表是否存在
来源：http://baike.sjlbkw.cn/Article/details/grdtswyyd.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.fktsv.cn/Article/details/goofuhhfp.sHtML

[Q90] 生成序号列
来源：http://www.m.share.sjlbkw.cn/Article/details/gofkcilat.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.tarul.cn/Article/details/gpzcsfhok.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gwsqvgcuw.sHtML

R. Bash 专题
来源：http://wap.yfazqb.com/Article/details/gpqjprjiz.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gqqazsjqr.sHtML

[R01] shebang 与严格模式
来源：http://mobile.vehdjk.com/Article/details/gxiysslgd.sHtML

#!/usr/bin/env bash
来源：http://mobile.fktsv.cn/Article/details/gavuassvj.sHtML

set -euo pipefail
来源：http://www.blog.yfazqb.com/Article/details/gcqewewhe.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.fktsv.cn/Article/details/grzibbpki.sHtML

name="Tom"; echo "$name"
来源：http://baike.epnwcf.com/Article/details/grxkqxhgx.sHtML

[R03] 只读变量
来源：http://m.share.bbcook.cn/Article/details/glazyjzsm.sHtML

readonly PI=3.14
来源：http://blog.yfazqb.com/Article/details/gjmnbshac.sHtML

[R04] 位置参数
来源：http://www.share.yfazqb.com/Article/details/gdliqlpbd.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.sjlbkw.cn/Article/details/gzckqrpno.sHtML

[R05] 参数默认值
来源：http://m.share.vehdjk.com/Article/details/gvneaywjw.sHtML

name="${1:-default}"
来源：http://www.share.tarul.cn/Article/details/ggplcvqld.sHtML

[R06] 判断命令是否存在
来源：http://m.share.bbcook.cn/Article/details/gotlvmyec.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.vehdjk.com/Article/details/gwylobtps.sHtML

[R07] if 判断文件
来源：http://www.blog.sjlbkw.cn/Article/details/ghknvzoog.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.tarul.cn/Article/details/gjdeppbzj.sHtML

[R08] 数值比较
来源：http://baike.bbcook.cn/Article/details/gmbzwpclc.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.fktsv.cn/Article/details/gcsyubywr.sHtML

[R09] 字符串比较
来源：http://wap.vehdjk.com/Article/details/gedopgcpk.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.fktsv.cn/Article/details/glnvuuxie.sHtML

[R10] 正则匹配
来源：http://mobile.tarul.cn/Article/details/gunjffrns.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.yfazqb.com/Article/details/gkgxtdssy.sHtML

[R11] case 多分支
来源：http://blog.sjlbkw.cn/Article/details/gbakejooh.sHtML

case "$1" in
来源：http://m.share.sjlbkw.cn/Article/details/gmkehkqak.sHtML

start) echo "启动" ;;
来源：http://read.share.epnwcf.com/Article/details/gxghkgkml.sHtML

stop)  echo "停止" ;;
来源：http://wap.tarul.cn/Article/details/gqemsupao.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.epnwcf.com/Article/details/gfdaafzbe.sHtML

esac
来源：http://m.share.vehdjk.com/Article/details/gmbwwtuhh.sHtML

[R12] for 遍历文件
来源：http://www.share.fktsv.cn/Article/details/guymkwmff.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.fktsv.cn/Article/details/gbposkshh.sHtML

[R13] for 计数循环
来源：http://wap.yfazqb.com/Article/details/glnqviskd.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.bbcook.cn/Article/details/ghfxmfdyo.sHtML

[R14] C 风格 for
来源：http://www.blog.sjlbkw.cn/Article/details/gtpsbiqyp.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.sjlbkw.cn/Article/details/gufflolfu.sHtML

[R15] while 逐行读文件
来源：http://mobile.sjlbkw.cn/Article/details/gdjyzxmhy.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.tarul.cn/Article/details/gjuuulnjc.sHtML

[R16] until 等待条件
来源：http://3g.fktsv.cn/Article/details/gjdqeooem.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.yfazqb.com/Article/details/gtyrchszf.sHtML

[R17] 数组定义与取值
来源：http://www.share.fktsv.cn/Article/details/grlnwgbsb.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.bbcook.cn/Article/details/gmsiglvfm.sHtML

[R18] 遍历数组
来源：http://www.share.vehdjk.com/Article/details/gyrclxxkm.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.sjlbkw.cn/Article/details/gvdtfagkr.sHtML

[R19] 数组长度
来源：http://wap.bbcook.cn/Article/details/gvahfxsym.sHtML

echo "${#arr[@]}"
来源：http://baike.fktsv.cn/Article/details/gijfmytsq.sHtML

[R20] 关联数组（字典）
来源：http://m.share.epnwcf.com/Article/details/ggtuxmoip.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.tarul.cn/Article/details/gmvosfjpn.sHtML

[R21] 字符串长度
来源：http://wap.sjlbkw.cn/Article/details/gnazzpnxt.sHtML

echo "${#s}"
来源：http://wap.bbcook.cn/Article/details/gjgejymsx.sHtML

[R22] 截取子串
来源：http://www.m.share.epnwcf.com/Article/details/gwdbwklwu.sHtML

echo "${s:0:5}"
来源：http://www.blog.fktsv.cn/Article/details/gmcdwpvnm.sHtML

[R23] 字符串替换
来源：http://www.share.sjlbkw.cn/Article/details/gnkphzlnf.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.bbcook.cn/Article/details/gdzcwlqmm.sHtML

[R24] 大小写转换
来源：http://read.share.vehdjk.com/Article/details/gohenbqut.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.epnwcf.com/Article/details/gdtfquxhz.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.sjlbkw.cn/Article/details/gzlbmpkiv.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.epnwcf.com/Article/details/gnnyedqja.sHtML

[R26] 命令替换
来源：http://baike.fktsv.cn/Article/details/gahtiyhdg.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.yfazqb.com/Article/details/gfwfjxntk.sHtML

[R27] 算术展开
来源：http://3g.epnwcf.com/Article/details/gixzoexws.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.tarul.cn/Article/details/gcaqyvxyp.sHtML

[R28] 浮点运算
来源：http://m.share.vehdjk.com/Article/details/guvrfqysa.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.bbcook.cn/Article/details/gnhchfltw.sHtML

[R29] 定义函数
来源：http://m.share.sjlbkw.cn/Article/details/gtwqrijhn.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fktsv.cn/Article/details/gowfkdqcl.sHtML

[R30] 函数返回状态码
来源：http://blog.yfazqb.com/Article/details/ghjknovph.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.yfazqb.com/Article/details/gnzgdjpbf.sHtML

[R31] 局部变量
来源：http://www.blog.epnwcf.com/Article/details/gsusckzuh.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.epnwcf.com/Article/details/gvnmuqpxs.sHtML

[R32] 参数个数校验
来源：http://read.share.bbcook.cn/Article/details/gulebqtrl.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gzktcbgmj.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.vehdjk.com/Article/details/gjczenwqe.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.bbcook.cn/Article/details/gwpgsxrwi.sHtML

[R34] 退出时清理
来源：http://www.blog.yfazqb.com/Article/details/gfehuvaaz.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.epnwcf.com/Article/details/gtglyjgum.sHtML

[R35] 后台执行并等待
来源：http://wap.epnwcf.com/Article/details/gjtakhjia.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fktsv.cn/Article/details/gyockmdzg.sHtML

[R36] 并发执行多个任务
来源：http://baike.vehdjk.com/Article/details/gtnndghqf.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.epnwcf.com/Article/details/gyhvfptjg.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fktsv.cn/Article/details/ghdjlgyhz.sHtML

files=$(ls -1)
来源：http://baike.yfazqb.com/Article/details/gxlksnrhw.sHtML

[R38] 管道串联
来源：http://blog.bbcook.cn/Article/details/gitnkxaal.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.fktsv.cn/Article/details/ggukeblnk.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.tarul.cn/Article/details/gbwbixqmy.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.vehdjk.com/Article/details/gmzziqscw.sHtML

[R40] 追加写日志
来源：http://www.m.share.fktsv.cn/Article/details/gwjfpvrkd.sHtML

echo "log" >> out.log
来源：http://www.blog.bbcook.cn/Article/details/gpcozpnyl.sHtML

[R41] 丢弃输出
来源：http://read.share.fktsv.cn/Article/details/gmkpfzxbf.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.epnwcf.com/Article/details/gqegomtbq.sHtML

[R42] 输入重定向
来源：http://www.blog.sjlbkw.cn/Article/details/gjxqjzijd.sHtML

wc -l < a.txt
来源：http://baike.epnwcf.com/Article/details/ghchzqfll.sHtML

[R43] 按名字查找文件
来源：http://mobile.fktsv.cn/Article/details/gfcmrjxcp.sHtML

find . -name "*.log" -type f
来源：http://www.share.sjlbkw.cn/Article/details/gslbhzchl.sHtML

[R44] 按修改时间查找
来源：http://www.share.vehdjk.com/Article/details/geuuvccab.sHtML

find . -mtime -7 -type f
来源：http://m.share.vehdjk.com/Article/details/gadgsxkan.sHtML

[R45] 批量删除
来源：http://mobile.epnwcf.com/Article/details/gzhqmcpaq.sHtML

find . -name "*.tmp" -delete
来源：http://blog.yfazqb.com/Article/details/gfqvcqecd.sHtML

[R46] 递归替换文件内容
来源：http://blog.epnwcf.com/Article/details/gwrbxldvu.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.tarul.cn/Article/details/gffuqyfom.sHtML

[R47] sed 单行替换
来源：http://wap.bbcook.cn/Article/details/gbzeesalx.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.vehdjk.com/Article/details/gjskrsdpu.sHtML

[R48] awk 取指定列
来源：http://blog.sjlbkw.cn/Article/details/gupsaapep.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.bbcook.cn/Article/details/gvwmkviyf.sHtML

[R49] awk 带条件
来源：http://www.blog.tarul.cn/Article/details/gskiweavs.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.epnwcf.com/Article/details/ggxwaycam.sHtML

[R50] awk 求和
来源：http://mobile.vehdjk.com/Article/details/ggyezvhxy.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.epnwcf.com/Article/details/gidhtrokb.sHtML

[R51] 排序去重取前几
来源：http://blog.yfazqb.com/Article/details/gzubhwngf.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.epnwcf.com/Article/details/gwxeipwrq.sHtML

[R52] 统计行数
来源：http://www.share.bbcook.cn/Article/details/ggfmcwwgk.sHtML

wc -l a.txt
来源：http://m.share.tarul.cn/Article/details/gzsilbayz.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.vehdjk.com/Article/details/gaimvypim.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.tarul.cn/Article/details/grsrjjezp.sHtML

[R54] 比较两个文件
来源：http://blog.sjlbkw.cn/Article/details/gqyyqtuye.sHtML

diff a.txt b.txt
来源：http://wap.epnwcf.com/Article/details/geafddfzc.sHtML

[R55] 压缩与解压
来源：http://blog.yfazqb.com/Article/details/gtotkrhaq.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.yfazqb.com/Article/details/gnjyoheac.sHtML

[R56] 远程拷贝
来源：http://www.m.share.sjlbkw.cn/Article/details/gicflzqyj.sHtML

scp file user@host:/path/
来源：http://baike.epnwcf.com/Article/details/gmfsmwyna.sHtML

[R57] 远程执行命令
来源：http://baike.bbcook.cn/Article/details/gaeskksef.sHtML

ssh user@host 'uptime'
来源：http://wap.vehdjk.com/Article/details/gjgmfymuz.sHtML

[R58] 下载文件
来源：http://wap.sjlbkw.cn/Article/details/gchvxrwyf.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.tarul.cn/Article/details/gojqiepqd.sHtML

[R59] 发 POST JSON
来源：http://www.share.fktsv.cn/Article/details/gqkmnzowu.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.vehdjk.com/Article/details/gwhkxmlej.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.yfazqb.com/Article/details/gxbpsubno.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fktsv.cn/Article/details/gtnhbvjhq.sHtML

[R61] 磁盘占用
来源：http://blog.epnwcf.com/Article/details/gavkukxng.sHtML

df -h;  du -sh *
来源：http://blog.sjlbkw.cn/Article/details/ghhpqlaez.sHtML

[R62] 找最占空间的文件
来源：http://m.share.fktsv.cn/Article/details/gpuxmvudd.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.vehdjk.com/Article/details/gukbvocav.sHtML

[R63] 内存与进程
来源：http://wap.tarul.cn/Article/details/ghyvjqdsz.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.yfazqb.com/Article/details/gsgppdyns.sHtML

[R64] 结束进程
来源：http://mobile.yfazqb.com/Article/details/gvkarxmaz.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.tarul.cn/Article/details/gfzlwanow.sHtML

[R65] 查看端口占用
来源：http://baike.sjlbkw.cn/Article/details/gwtbnlajt.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.epnwcf.com/Article/details/ghhgwdzye.sHtML

[R66] 定时任务
来源：http://wap.bbcook.cn/Article/details/gwjcaqacr.sHtML

crontab -e;  crontab -l
来源：http://wap.bbcook.cn/Article/details/gvxfmgsjq.sHtML

[R67] 生成随机十六进制串
来源：http://wap.tarul.cn/Article/details/gigipfvyh.sHtML


<!-- 参考信息 -->